+++
date = 2014-12-22
draft = false
tags = []
title = "Approximation and its Limits "
+++


In the previous [blog post](/2014/puzzles.html), we saw that a computer as we know it, cannot help in 
solving many puzzles. But some of these puzzles need to be solved, routinely in real life programs.
So should we give up hope? Is there another way out?

One way out, is to relax the conditions that is required of the solutions. 
For the sudoku puzzle, we might say that, we are happy with solutions with
just the rows and columns having all distinct numbers and not the blocks.
If we further remove the condition that every column has distinct elements,
then the puzzle becomes easy to solve (since for every row, we can fill
in the blanks without worrying about the other rows). For every puzzle, 
we would ideally like to do minimal relaxation and come up with
a polynomial time algorithm.  

#### $3$-SAT

Now lets consider a problem which has very wide practical application. It
is called the $3$-SAT problem. An instance of the problem has a collection
of *clauses* $C_1,\cdots,C_m$ of the following form. 

<p style="text-align:center">
<img src="../../images/3SAT.png" width="600px" /> </p>

Here $x_1,\cdots, x_n$ are *variables* which takes  $0,1$ values. Here $\neg x_3$ is to be 
read as NOT of $x_3$, which is the value of $1- x_3$ and $\vee$ is the OR.
An assignment to the variables *satisfies* a clause if one among the $3$ values
associated with the OR ($\vee$) is $1$. If it satisfies all clauses then it is said
to *satisfy* the instance and such an instance is called a *satisfiable* instance.
 The goal is, when given a satisfiable instance,  find an
assignment of $0,1$ to the variables that satisfies the instance. This was the
first problem that was proved to be NP-Complete by Cook and Levin.

#### Approximation

A natural way to relax the problem, is to only ask for an algorithm that
finds an assignment, if it exists, that satisfies 
99% of the clauses. Such an algorithm is called an *approximation
algorithm* for the original $3$-SAT problem with *approximation factor*   $ 0.99$.


Instead of $0.99$, if we only require the *approximation factor* to be $7/8$,
then there is a very stupid approximation algorithm, which does not
even need to look at instance of the problem. But this algorithm uses some
randomness and answers correctly only most of the time. Most programming
languages allow algorithms to choose random numbers during execution. Hence
these can be implemented in computers.

>All the algorithm does is for every variable, assign a random $0,1$ value. Since
a clause is the OR of $3$ values, it will not be satisfied only
when all the values are $0$, the chances of which are $1/8$. Hence this
stupid algorithm gives an assignment which satisfies $7/8$ fraction of the 
clauses (most of the time).

#### Limits

The algorithm above is very trivial. We might think that there may be an algorithm 
 which, by cleverly looking at the clauses in a satisfiable problem instance, finds an assignment
 that satisfies more than a $7/8$ fraction of the clauses. 

>However in 1998, Hastad <a href="http://dl.acm.org/citation.cfm?id=502098&dl=ACM&coll=DL&CFID=468122525&CFTOKEN=86867583">proved</a> that if there is a polynomial time algorithm with
factor better than $7/8$, then NP-Complete problems have polynomial time
solutions. This is not expected to happen. Hence that trivial algorithm 
cannot be improved.

Hastad proved similar results for many other problems. For every problem there is a magic constant
($7/8$ for $3$-SAT), such that there are simple polynomial time algorithms having factor equal to it. But
all known algorithms with a better approximation factor requires exponential time.

#### Probabilistically Checkable Proofs
Lets come back to sudoku puzzles. Some sudoku puzzle instances cannot be competed such that all 
the constraints about rows, columns and sub blocks are satisfied. If it can be completed
then the instance is said to be *satisfiable*. Then a completion that satisfies all the constraints
is a *proof* for the fact that the instance is satisfiable. We can verify this proof easily,
but nevertheless we still need to check all the constraints about rows, columns and sub blocks
to be completely sure. 

>A probabilistically checkable proof (PCP) is a way of writing proofs,
such that it can be checked by making a few random queries in to the proof.

PCP was discovered by Feige, Goldwasser, Lund, Safra, and Szegedy (1991), and Arora and Safra (1992).
Hastad's result mentioned previously, showed that for any puzzle that is NP-Complete, 
we can convert an instance of that puzzle to a $3$-SAT instance such that:

- satisfiable instances of the puzzle are converted to satisfiable instances of $3$-SAT.

- unsatisfiable instances are converted to $3$-SAT instances for which any assignment can satisfy only a $7/8$ fraction of the clauses.

This gives a PCP for satisfiable sudoku instances as follows. First we will convert the sudoku instance
to a $3$-SAT instance and the proof will be a satisfying assignment for the $3$-SAT instance. We
will check this proof by choosing a random clause in the $3$-SAT instance, querying the $3$ variables
in it and checking if the clause is satisfied. 

- If the sudoku instance is indeed satisfiable, then there is a proof which is the satisfying assignment for the $3$-SAT
instance that is accepted with probability $1$.

- Otherwise all proofs are accepted with probability at most $7/8$, since any assignment can satisfy only $7/8$ fraction of clauses in the $3$-SAT instance.

In the above PCP, wrong proofs might get accepted with probability $7/8$. But this error can be brought
down by repeatedly doing the above checks using independent random choices and rejecting the proof if any one of the
checks fails.

#### Conclusion

One way to cop with NP-Complete puzzles, is to relax the constraints on the solutions. A
natural way to do the relaxation, for many problems like $3$-SAT, is to only look for approximation
algorithms. If the approximation factor required is small, then there are often
simple polynomial time algorithms. When the factor required is larger than a threshold ($7/8$ for $3$-SAT),
then polynomial time algorithms could not be found. An explanation for our inability for doing
this could be obtained from the conjecture that NP-Complete problems does not have polynomial time algorithms.
Research on this has lead to the discovery of fascinating objects like  probabilistically checkable proofs.
 