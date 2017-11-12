+++
date = 2014-12-25
draft = false
tags = []
title = "Hardness of Coloring Problems"
+++



This is the third part, of a series of <a href="/2014/puzzles.html">blog</a> <a href="/2014/approximation-limits.html">posts</a>,
on the impossibility of finding efficient algorithms for certain problems.

In the <a href="/2014/puzzles.html">first</a>, we saw that for sudoku and many other puzzles, there is a single explanation for
our inability to find polynomial time algorithms. The explanation is that, any one problem (say sudoku) that is
NP-Complete, does not have a polynomial time algorithm. This is commonly known as the P $\neq$ NP assumption. 
If assuming this, a certain problem  does not have a polynomial time algorithm, then we say that it is *hard*.
When a problem has a polynomial time algorithm, we say it is *easy*.

In the <a href="/2014/approximation-limits.html">second post</a>, we saw that for the $3$-SAT problem, even a relaxed version of the problem, of getting an
approximation factor better than $7/8$, is hard. We also saw a very silly polynomial time algorithm, which gives a $7/8$ approximation
factor. Such pair of results are called *optimal*, since we know the exact value of the approximation factor below which the problem is easy and above which the problem is hard.


The purpose of this post is to explain some
recent developments in the hardness results for a particular problem called coloring (to which I have contributed).
It is a very common problem, for which we do not have optimal results yet. 

#### Graph Coloring


<p style="text-align:center">
<img src="../../images/highlight/graph_coloring.png" width="300px" /> </p>

A *graph* is an object like the uncolored figure above. It consists of a set of *vertices*, which are the round things and a set of
*edges*, which are the lines connecting the round things. The colored figure above is a *$3$-coloring* of the graph on the left, 
because for every edge, the vertices at the end points have different color and only $3$ colors (red, blue and green) are used.

The graph coloring problem is, when given a graph (an arbitrary figure like the one on the left), find a *coloring* (assignment of 
colors to the vertices, such that the end points of every edge has different colors), using the least number of colors. In particular,
we will be looking at the following question:

**Given a $3$-colorable graph, can you find a $C$-coloring?**

The best polynomial time algorithm known for this problem, only guarantee $C = n^{0.199\cdots}$, where $n$ is the number of vertices. It is known 
that finding a $4$-coloring  is *hard*.  We want to know where exactly between $n^{0.199\cdots}$ and $4$, the transition from easy to hard
happens.

##### Khot's Unique Games Conjecture (UGC)
Khot observed that PCP with $2$ random queries and unique checks, will imply more  hardness of approximation results.

 
##### Our Results

>In <a href="http://arxiv.org/abs/1411.3517">joint work</a> with Irit Dinur, Prahladh Harsha, Srikanth Srinivasan, 
we showed that assuming a version of UGC, $C=2^{poly(\log \log n)}$ is hard, an improvement over $C=poly(\log \log n)$ 
hardness result of Dinur and Shinkar, using similar assumption.

**Puzzle:** $N$ switches each of which can take $3$ positions, control a bulb which glows as red, blue and green. 
Changing the position of all the switches changes the color of the bulb. Show that the bulb is controlled
by exactly one switch.
   
Even if the number of colors the bulbs can take is $100$, for $N=1000$ this is still (al most) true. 
We show that even if the switches where not allowed to move independently, such statements are still true.



#### Hypergraph Coloring

<p style="text-align:center">
<img src="../../images/highlight/hypergraph_coloring.png" /> </p>

**$r$-Uniform Hypergraph:** A vertex set $V$ and a
collection of subsets of $V$ of size $r$. Assign colors to 
vertices such that no set is monochromatic.Graphs corresponds to the 
setting of $r=2$. 

Known algorithms only guarantee $C=n^\alpha$ for some $\alpha < 1$. The state of the art results  showed that $C= poly( \log n)$ is hard.
 
##### Our Results

In <a href="http://arxiv.org/abs/1311.7407">joint work</a> with Venkat Guruswami,
Johan Hastad, Prahladh Harsha and Srikanth Srinivasan, we show $C > > poly(\log n)$ is also hard.
Subsequent to our work, Khot and
Saket  showed $C=2^{(\log
n)^{1/19}}$ is hard. Though their result was
for $12$-uniform hypergraphs. 
I further observed that
by combining their methods with ours, the same  hardness can be
obtained for $4$-uniform hypergraphs~\cite{Varma2014}. 

>Hence  we improved the hardness results from $C=poly(\log n)$ to $C=2^{(\log n)^{1/19}}$ for the
case of $4$-colorable $4$-uniform hypergraphs.


#### Covering Problems
Covering problems are a generalization of the 
coloring problem. Motive for studying them is to develop
techniques which might later be adapted to graph coloring. 

An instance of the problem
consists of a hypergraph $G=(V,E)$ along with a *predicate* $P
\subseteq \{0,1\}^r$ and a *literal* function $L:E\rightarrow
\{0,1\}^r$. An *assignment* $f:V \rightarrow \{0,1\}$
*covers* an edge $e\in E$, if $f|_e \oplus L(e) \in P$. 
A *cover* for an instance is a set of 
assignments such that every edge is covered by one of the assignments.

**The covering problem is, given a $2$-coverable instance, find a $C$-covering?**

**Theorem:** $G$ has a cover of size $C$ with the not-all-equal predicate
$\{0,1\}^r \setminus \{ \overline 0, \overline 1\}$ iff it is
$2^C$-colorable. 

Some predicates like $3$-SAT which has an
*oddness* property (for every $x\in \{0,1\}^r, x\in P \vee \bar x \in P$). Then $C=2$ is easy, since any assignment and its complement
covers the instance.

Dinur and Kol asked the question
whether the covering problem is hard  for all non-odd
predicates for any constant $C$. Assuming a slightly modified form of UGC, they proceeded to show that if a non-odd predicate has a
pairwise independent distribution in its support, then this is indeed
the case.

##### Our Results
 >In <a href="http://arxiv.org/abs/1411.7747">joint work</a> with Amey Bhangale and Prahladh Harsha, we show  
- hardness for all non-odd predicates and for all constants $C$ (making same assumptions as Dinur and Kol),  
- NP-hardness under some mild conditions on the predicate for $C= \log \log n$,   
- improved hardness of $C=\log \log n$ (Dinur and Kol proved $\log \log \log n$.).


