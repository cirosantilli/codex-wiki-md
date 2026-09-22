<h1 id="1/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $u^\dagger=K^\dagger f$. Every [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) is $u^\dagger+w$ for some $w\in\mathcal N(K)$, while $u^\dagger\in\mathcal N(K)^\perp$. Decompose $u_0=P_{\mathcal N(K)}u_0+P_{\mathcal N(K)^\perp}u_0$ using [orthogonal projections](../../../../../../../orthogonal-projection.md). Then the [Pythagorean identity](../../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|u^\dagger+w-u_0\|^2
=\|u^\dagger-P_{\mathcal N(K)^\perp}u_0\|^2
+\|w-P_{\mathcal N(K)}u_0\|^2.
$$

The first term is independent of $w$, and the second vanishes at exactly one point. Hence the unique [nearest least-squares solution](../../../../../../../nearest-least-squares-solution.md) is

$$
\boxed{u_0^\dagger=K^\dagger f+P_{\mathcal N(K)}u_0.}
$$

Geometrically this is the [orthogonal projection](../../../../../../../orthogonal-projection.md) of $u_0$ onto the closed [affine subspace](../../../../../../../affine-subspace.md) of [least-squares solutions](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
