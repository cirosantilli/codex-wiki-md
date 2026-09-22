<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the standard [Hermitian inner product](../../../../../hermitian-inner-product.md) $\langle w,v\rangle=w^\dagger v$. Since $W$ is invariant under every $D_2(g)$, it is in particular invariant under

$$
D_2(g^{-1})=[D_1(g)]^\dagger.
$$

Let $v\in W^\perp$ and $w\in W$. Then

$$
\langle w,D_1(g)v\rangle
=\langle D_1(g)^\dagger w,v\rangle=0,
$$

because $D_1(g)^\dagger w\in W$ and $v$ is orthogonal to $W$. Thus $D_1(g)v$ is orthogonal to every $w\in W$, proving

$$
\boxed{D_1(g)W^\perp\subseteq W^\perp\quad(g\in G)}.
$$

Therefore $W^\perp$ is an [invariant subspace](../../../../../invariant-subspace.md) for $D_1$. If $D_1$ is irreducible, $W^\perp$ is either $\{0\}$ or $\mathbb C^n$. In finite-dimensional [inner product space](../../../../../inner-product-space.md), $(W^\perp)^\perp=W$, so these alternatives force $W=\mathbb C^n$ or $W=\{0\}$. Hence

$$
\boxed{D_1\ \text{irreducible}\ \Longrightarrow\ D_2\ \text{irreducible}}.
$$

No unitarity of $D_1$ was assumed; the [inverse-adjoint representation](../../../../../inverse-adjoint-representation.md) is exactly what makes this [orthogonal complement](../../../../../orthogonal-complement.md) argument work.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
