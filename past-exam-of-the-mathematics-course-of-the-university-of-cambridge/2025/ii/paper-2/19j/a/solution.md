<h1 id="19j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start with any positive-definite Hermitian inner product $\langle-,-\rangle$ on $\mathbb C^n$ and average it over the finite group:

$$
\langle v,w\rangle_G=
\frac1{|G|}\sum_{g\in G}
\langle\rho(g)v,\rho(g)w\rangle.
$$

This remains positive definite. For $h\in G$, reindexing $g\mapsto gh$ gives

$$
\langle\rho(h)v,\rho(h)w\rangle_G
=\langle v,w\rangle_G,
$$

so the form is $G$-invariant.

Choose an orthonormal basis for $\langle-,-\rangle_G$. In this basis every $\rho(g)$ preserves the standard Hermitian form and is therefore unitary. If $P$ is the change-of-basis matrix, then

$$
\rho'(g)=P^{-1}\rho(g)P
$$

defines an isomorphic representation with $\rho'(G)\leq U_n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19J](../../19j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
