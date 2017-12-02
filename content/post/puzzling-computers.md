+++
date = 2014-12-22
draft = false
tags = []
title = "Puzzling Computers"
math = true
+++

#### Sudoku
<p style="text-align:center">
<img src="../../images/sudoku_9x9.png" width="200px" /> <img src="../../images/sudoku_9x9_solved.png" width="200px" />
</p>

Above is an *instance* of the [sudoku](http://en.wikipedia.org/wiki/Sudoku)
puzzle. The goal is to fill in numbers from $1$ to $9$ in the blanks such that,
every  row, column and $3 \times 3$ block has all the $9$ different numbers. 
Beside is a solution for the puzzle instance and it is easy to verify that the
*constraints* on the rows, columns and sub blocks are *satisfied*.

 Since very few numbers are given, it is difficult to solve.
Nevertheless a person might solve it in a few
hours. But what if the puzzle instance was "larger".
That is instead of a $9\times 9$, it is a $16\times 16$ version,
where numbers from $1$ to $16$ could be filled in.
It has similar *constraints* on having all
numbers in rows and columns and $4\times 4$ sub blocks.

<p style="text-align:center">
<img src="../../images/sudoku_16x16.png" width="400px" style="margin: 10px 20px"/> </p>

Such a puzzle would be mind boggling for
humans to handle. But, may be there is a 
clever computer program, to do the job for
us. There is some hope, since a solution
given below for the above sudoku instance is very
easy to verify. 


<p style="text-align:center">
<img src="../../images/sudoku_16x16_solved.png" width="400px" style="margin: 10px 20px"/> </p>

One just needs to check if every row, column and
sub block has all the numbers from $1$ to $16$. So
 an *algorithm* (a computer program) would be to 
go over all *assignments* of numbers from $1$ to $16$, to the blanks
and check if the *constraints* on rows, columns and
sub blocks are *satisfied*. This might look
like a simple thing to do, except when one tries
to run the program. 


#### Polynomial Time Algorithms

Suppose half the blanks in the above $16\times 16$
 puzzle instance were
already filled, the number of possibilities
the program has to try is $16^{16 \times 16/2}$ (try all the $16$ possibilities
for each of the $16\times 16/2$ blanks). This number is
more than the [number](http://en.wikipedia.org/wiki/Chronology_of_the_universe)
 of seconds since the Big Bang and
more than the [number](http://www.physicsoftheuniverse.com/numbers.html)
 of particles in the universe. No
matter how fast or large a computer we have, it will
keep running (if we can maintain it that way) [till](http://image.gsfc.nasa.gov/poetry/ask/a10395.html)
our sun goes dead.

Hence the "try all possibilities" algorithm is definitely not
acceptable. We want an algorithm which, lets say
finds the solution in a day. As we saw, we would
also like to solve "larger" $n\times n$ versions of the puzzle.
$9\times 9$ was the case for $n=9$ and $16\times 16$ for $n=16$. 

> The try
all possibilities algorithm that we saw, needs to try (at least)
$n^n$ possibilities. Algorithms with such a bad running time are called
*exponential time* algorithms. Even for $n=16$, $n^n$ is a humongous number,
because n is in the *[exponent](http://en.wikipedia.org/wiki/Exponentiation)*.

 Suppose the number of steps
the algorithm runs is $n^c$ for some constant $c$, it would not
be that bad. Such an algorithm is called a  *polynomial time*  algorithm. 
Finding a polynomial time algorithm for sudoku is a long standing
challenge for programmers, which remains unsolved till this date. 
All the algorithms known so far can
take $n^n$ time on some sudoku instances.

#### NP-Completeness

In the 1970's, Stephen Cook, Leonid Levin and Richard Karp found that sudoku is not just a one off
case, for which polynomial time algorithms cannot be found. They showed 
that the same mystery exists for a whole class of puzzles, called NP-Complete (NPC).

They showed this, by devising a way of solving any one puzzle in NPC, by
using solutions to any other puzzle in NPC. That is for any pair of puzzles,
say sudoku and [kakuro](http://en.wikipedia.org/wiki/Kakuro) in NPC,
 they showed how to convert an instance of
sudoku to an instance of kakuro such that a solution to the kakuro instance
can be converted back to a solution to the sudoku instance. If that was confusing,
what it means is that,

>if there is a polynomial time algorithm for any one puzzle
in NPC, that would mean there is a polynomial time algorithm for all puzzles in NPC.

Till today, thousands of problems has been found to be NP-Complete and we dont have algorithms
that runs in time much better than $n^n$ for all of them. By the result mentioned above, if there
was a better algorithm for any one of them, then there is an algorithm with very similar running time
for each NP-Complete problem.

#### Why Care?

Who cares about solving puzzles when there are
more pressing problems in the world. These might appear to be
questions that a jobless unrealistic philosopher might ponder
about. Though it is not so. A lot depends on finding answers
to these questions. 

Nobody would disagree that internet is one of the greatest things
 to happen in end of the previous century.  An
underlying technology that makes it possible is encryption.
That is, a way of sending messages so that only the intended person
is able to read it.

All the existing methods of encryption are based on the assumption
that NPC problems does not have polynomial time algorithms. That is

>if somebody comes up with a fast polynomial time algorithm for solving 
sudoku puzzles, he can break all the codes in the internet.

Dont panic!. Your internet banking accounts are safe. We
dont expect this to happen. However, we need to know what other
problems are in NPC. This will help us design better encryption
systems and many other [things](http://en.wikipedia.org/wiki/Zero-knowledge_proof).

#### A Philosophical Detour

Though most people are interested in solving those pressing problems
of the world, there are still some stupid harmless philosophers
who find it interesting to think about these for the sake of curiosity.
They find a "deeper" meaning to this silly question about solving
puzzles.

> Mathematical proofs, sudoku solutions are all easy to verify. Does that
mean they are easy to come up with? Can human creativity be truly
automated?

If NPC puzzles had fast polynomial time algorithms, then in many cases 
humans can be replaced by computers in solving problems. The concepts of
puzzles and NPC described in this article could be
defined unambiguously in the language of maths. Scientists have been
hard at work for over 40 years either trying show NPC does not have polynomial time
algorithms or finding fast algorithms for these problems. Some day, hopefully
soon, we will have an answer.


#### Conclusion

The results mentioned above increases our faith in the conjecture that NP-Complete problems does not
have polynomial time algorithms. 

>This conjecture could be disproved if any one of the thousands of NP-Complete problems has a polynomial time algorithm, but yet it has stood the test of time for over 40 years. Assuming this conjecture gives a singular explanation for our inability to design good algorithms 
for many problems. 


#### Further Reading

- [What to do, when a puzzle is NP-Complete?](/2014/approximation-limits.html)

