+++
# Date this page was created.
date = "2017-06-01"

# Project title.
title = "Complexity Theory"

# Project summary to display on homepage.
summary = "Surveying Deep learning methods used in Reinforcement Learning"

# Optional image to display on homepage (relative to `static/img/` folder).
#image_preview = "bubbles.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["complexity-theory"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = true

# Optional featured image (relative to `static/img/` folder).
[header]
#image = "headers/bubbles-wide.jpg"
#caption = "My caption :smile:"

+++

Complexity theory studies what problems can and cannot be solved by computers given limited running time and memory resources.  


Students are expected to read the corresponding chapter from the textbook (mentioned under readings), before attending the lecture. 
The lecture is mainly for clearing doubts and covering the most confusing parts.

The is a short course with 13 lectures for students who might not have
taken a Theory of Computation course. However sufficient knowledge of 
discrete maths and algorithms is assumed. It is not supposed to be a 
rigorous one, for research student, but rather an introduction to field 
of complexity theory.

### Timings

- Wednesday (10:00 a.m.-11:25 a.m., Venue: 205)
- Saturday (10:00 a.m.-11:25 a.m., Venue: 205)
- Tutorial : Saturday (3:30 p.m.-4:30 p.m., Venue: 204)

### Lectures
Short notes are available with additional references : [Consolidated Notes HTML](notes).

1.  **Introduction** \\
    Decision Problems | Turing Machines | Efficient Algorithms

2.  **Paradox's, Diagonalization, Undecidablility** \\
    Russell's Paradox and Diagonalization | Universal Turing Machines | Halting Problem 

3.  **Nondeterminism, NP and Search Problems** \\
    Non Deterministic Turing Machines | Nondeterministic Polynomial Time : NP | NP : Verifier Definition | Descision vs Search Problems 

4.  **Reductions, NP-Completenesss & Cooks Theorem** \\
    Polynomial Time Reductions | Cook-Levin Theorem | NP Compeleness / Hardness 

5.  **More Time Complexity** \\
    NP-completeness of Vertex Cover and Subset Sum | EXP and Time Heirachy Theorem | coNP and Map of Complexity classes 

6.  **Space Compleixty** \\
    Space Complexity classes and some Relationships | Non Determinism and Space : NL-complete, Savith's Theorem | Overview of next part of course 

7.  **NL = coNL, Randomization** \\
    Recapping Nondeterminism | Immerman-Szelepcsenyi Theorem : NL = coNL | Randomized TMs and Complexity Classes 

9.  **Randomized Algorithms** \\
    BPP and Amplification | Approx MAX-CUT | Undirected REACHABILITY in RL 

8.  **Random Walks, Derandomization and Polynomial Identity Testing** \\
    Analysis of Random Walks | Derandomizing MaxCUT | Randomization: PIT and Schwartz-Zippel Lemma 
    
10.  **Streaming Algorithms and Lowerbounds**  \\
    Schwartz Zippel Lemma Proof | Lowerbound for Bracket Matching | Randomized Streaming Algorithm for Bracket Matching 
    
11. **Property Testing** \\
    Property Testing Model | Linearity Test by Blum, Luby and Rubinfield 

12. **PAC Learning**\\
hugo 


### Grading

This part of the course will have a total of 50 marks + 5 bonus marks.

- 25 marks for the end sem.
- 15 marks for the mid sem.
- 10 marks for assignments.
- 5 marks for quiz.

2-3 question will be given out at the end of every lecture. There will be one tutorial 
session per week (to be scheduled), where the assignments for the previous week will be collected, and 
solutions will be discussed.


### Textbook and References

**[Notes](notes)**



**Textbook : Computational Complexity by Christos Papadimitriou**


Some courses offered elsewhere:

- [Sud] A course on complexity theory (offered by Madhu Sudan) at MIT: 6.841/18.405J Advanced Complexity Theory (Spring 2003).
- [Tre1] A course on complexity theory (offered by Luca Trevisan) at UC, Berkeley: CS 278 - Computational Complexity (Fall 2002).
- [Tre2] A course on complexity theory (offered by Luca Trevisan) at UC, Berkeley: CS 278 - Computational Complexity (Fall 2004).
- [Vad] A course of complexity theory (offered by Salil Vadhan) at Harvard: CS221: Computational Complexity (Spring 2010).
