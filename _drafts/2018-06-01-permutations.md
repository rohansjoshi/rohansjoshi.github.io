---
layout: post
author: rohan
tags: [algebra, group theory]
---
A permutation is a way of rearranging an ordered set.  Formally, a permutation of a set $$X$$ is just a bijection $$X \to X$$. The set of permutations naturally forms a group.  This group is called the symmetric group on X.

We will focus only on finite sets.  For simplicity we will work with the set $$\{1, \dots n\}$$. The symmetric group of this set is called $$S_n$$.

### Transpositions

An adjacent transposition is a permutation which just swaps two adjacent elements.  For example, consider the permutation which rearranges (1,2,3,4,5) to (1,2,4,3,5).

Theorem. Every permutation is a product of adjacent transpositions.
Proof. Insertion sort.  Specifically, since the insertion sort algorithm rearranges a (finite) list by performing repeated adjacent transpositions, we can insertion sort the list into the permuted list, which gives us the permutation as a product of adjacent transpositions.If  a  permutation  can  we  be  written  as  the  product  of  an  odd  number  of transpositions, it is called an odd permutation.  Likewise, if it can be written as the product of an even number of transpositions, it is an even permutation.  We will prove that these labels define a partition of $$S_n$$

###  Inversions
Definition. Let $$\sigma \in S_n$$.  An inversion of $$\sigma$$ is a pair $$x,y$$ such that $$x \leq y$$ and $$\sigma(x)> \sigma(y)$$.   We  define $$N(\sigma)$$  to  be  the  number  of  inversions  of $$\sigma$$ (this is a number between 0 and $$n \choose 2$$).

Theorem. If $$\sigma, \tau \in S_n$$ and $$\tau$$ is an adjacent transposition, then $$N(\tau\sigma)$$ is  $$N(\sigma) + 1$$ or $$N(\sigma) - 1$$.

Proof. Suppose $$\tau$$ swaps adjacent elements $$x$$ and $$y$$.  Since the positions of all the  elements  relative  to $$x$$ and $$y$$ are  unchanged  byτ(there  are  no  elements between them), every inversion ofσthat is not $$(x,y)$$ is an inversion ofτσ, and vice-versa.  Furthermore, $$(x,y)$$ is an inversion of σ if and only if it is not an inversion of τσ.  So, N(τσ) is eitherN(σ) + 1 orN(σ)−1. $$\square$$

Theorem. A permutation cannot be both odd and even.

Proof. Multiplying a permutationσby an adjacent transposition switches the parity ofσ, by the above theorem.  So $\sigma$ is odd if and only if N(σ) is odd (and not even) if and only if σis not even.

Thus  we  have  a  homomorphism $$S_n \to \mathbb{Z}/2\mathbb{Z}$$. Its  kernel  is  the  set  of  even permutations, called the alternating group; it is denoted $$A_n$$  

### References
1.  Hug, J. Sorting I (Basic Sorts).https://sp18.datastructur.es/materials/lectures/lec32/lec322.  
2. Pinter,  Charles  C.  A  book  of  abstract  algebra.   Bonner  MathematischeSchriften [Bonn Mathematical Publications], 135.  McGraw-Hill Book Co.,New York, 1982.  xv+351 pp.  ISBN: 0-07-050130-0 (Reviewer:  James K.Deveney
