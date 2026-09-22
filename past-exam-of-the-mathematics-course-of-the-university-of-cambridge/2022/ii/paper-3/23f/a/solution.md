<h1 id="23f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a local coordinate $w$ with $w(p)=0$. Differentiation at $p$ gives a homomorphism

$$
\lambda:H\to\mathbb C^\times,
\qquad \lambda(h)=h'(p).
$$

It is injective. Indeed, a nonidentity [Möbius transformation](../../../../../../mobius-transformation.md) fixing $p$ and having derivative one there is parabolic, hence conjugate to a nonzero translation and of infinite order; no such element can belong to the finite group $H$. Every finite subgroup of $\mathbb C^\times$ is a cyclic group of roots of unity, so $H$ is cyclic. Write $n=|H|$.

The averaged coordinate

$$
z(q)=\frac1n\sum_{h\in H}\lambda(h)^{-1}w(hq)
$$

has derivative one at $p$, so it is a coordinate on a smaller neighbourhood. For $g\in H$, reindexing by $k=hg$ gives

$$
z(gq)=\lambda(g)z(q).
$$

After shrinking to an $H$-invariant disc $U$, the group therefore acts as all rotations $z\mapsto\zeta^jz$, where $\zeta$ is a primitive $n$th root of unity. The invariant coordinate

$$
u=z^n
$$

identifies $H\backslash U$ with a disc and gives it a [Riemann-surface](../../../../../../riemann-surfaces.md) chart. In these coordinates the quotient map is exactly

$$
\boxed{z\longmapsto z^n}.
$$

This is the [local cyclic quotient of a Riemann surface](../../../../../../local-cyclic-quotient-of-a-riemann-surface.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23F](../../23f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
