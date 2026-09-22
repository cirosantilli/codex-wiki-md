<h1 id="20f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $L$ is a [simplicial subcomplex](../../../../../../simplicial-subcomplex.md) of $K$, every face of a simplex of $L$ also belongs to $L$. The simplicial [boundary operator](../../../../../../boundary-operator.md) therefore satisfies

$$
\partial C_k(L)\subseteq C_{k-1}(L),
$$

so $C_\bullet(L)$ is a [chain subcomplex](../../../../../../chain-subcomplex.md) of the [simplicial chain complex](../../../../../../simplicial-chain-complex.md) $C_\bullet(K)$.

Define a map on the [quotient groups](../../../../../../quotient-group.md) by

$$
\bar\partial_k:C_k(K,L)\longrightarrow C_{k-1}(K,L),
\qquad
\bar\partial_k(c+C_k(L))
=\partial c+C_{k-1}(L).
$$

If $c'=c+\ell$ with $\ell\in C_k(L)$, then $\partial c'-\partial c=\partial\ell\in C_{k-1}(L)$, so this definition is independent of the representative. Moreover,

$$
\bar\partial_{k-1}\bar\partial_k[c]
=[\partial^2c]=0.
$$

**Thus $C_\bullet(K,L)$ is the [relative simplicial chain complex](../../../../../../relative-simplicial-chain-complex.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
