<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

Let $D_n\in\{1,2,3\}$ be the shorter circular separation after $n$ swaps, so $D_0=1$. There are $\binom62=15$ equally likely unordered swaps. Six swap only guests, one swaps the distinguished pair, and eight swap one distinguished diner with a guest. Rotations, reflections and exchangeability of the guests ensure that the next-separation probabilities depend only on $D_n$. Thus this is the [separation chain for two labels in a circular transposition shuffle](../../../../../separation-chain-for-two-labels-in-a-circular-transposition-shuffle.md), a [lumped Markov chain](../../../../../lumped-markov-chain.md).

Counting all swaps gives the [transition matrix](../../../../../stochastic-matrix.md)

$$
P=\frac1{15}\begin{pmatrix}9&4&2\\4&9&2\\4&4&7\end{pmatrix},
$$

with states ordered $1,2,3$. To verify the counts, fix one distinguished diner at seat $0$ and the other at seat $d$. For $d=1$, swaps moving the diner at $0$ to seats $2,3,4,5$ give separations $1,2,3,2$; swaps moving the diner at $1$ to those seats give $2,3,2,1$. Along with the seven separation-preserving swaps this gives $(9,4,2)$. For $d=2$, moving the first diner to seats $1,3,4,5$ gives $1,1,2,3$, while moving the second gives $1,3,2,1$; the total is $(4,9,2)$. For $d=3$, each distinguished diner has two moves to separation $1$ and two to separation $2$, giving $(4,4,7)$.

If $r_n=\Pr(D_n=3)$, the last column yields

$$
r_{n+1}=\frac2{15}(1-r_n)+\frac7{15}r_n
=\frac2{15}+\frac13r_n,\qquad r_0=0.
$$

Subtracting the fixed point $1/5$ and iterating solves the [affine recurrence](../../../../../affine-recurrence.md):

$$
\boxed{\Pr(\text{opposite on night }n+1)=r_n=\frac15(1-3^{-n})}.
$$

For one swap this gives $2/15$, agreeing with direct counting. The limit $1/5$ also agrees with the [stationary distribution](../../../../../stationary-distribution.md) $(2/5,2/5,1/5)$ of the separation [Markov chain](../../../../../markov-chain.md): given one diner's seat, one of the five remaining seats is opposite. The complete permutation shuffle alternates parity, but that does not prevent this lumped separation probability from converging.

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
