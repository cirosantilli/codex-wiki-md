<h1 id="20h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a planar [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) write its coordinates as $(S_n,T_n)$ and rotate to $(S_n+T_n,S_n-T_n)$. Each step now has four equally likely values $(1,1),(1,-1),(-1,1),(-1,-1)$. Thus the two rotated coordinates are independent one-dimensional [simple symmetric random walks](../../../../../../simple-symmetric-random-walk.md).

A return is impossible at odd times, and at time $2n$ its probability is

$$
p_{2n}(0,0)=\left(2^{-2n}\binom{2n}{n}\right)^2.
$$

For $n\geq2$, the supplied estimate gives $1/(4n)<p_{2n}(0,0)<1/n$. At $n=1$ the lower bound is actually equality, $p_2(0,0)=1/4$; this harmless strict-endpoint typo does not affect the argument. The [harmonic series](../../../../../../harmonic-series.md) diverges, so the criterion proved above shows that the origin is recurrent, in the terminology of a [recurrent Markov chain](../../../../../../recurrent-markov-chain.md). Translation invariance gives the same conclusion for every state. The [Markov chain](../../../../../../markov-chain.md) is [irreducible](../../../../../../irreducible-representation.md), so from any starting point it hits any fixed state almost surely and revisits it infinitely often. One can see the hitting assertion directly: repeated returns to the starting point give repeated positive-probability opportunities to follow a finite path to the target.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
