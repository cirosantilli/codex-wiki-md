<h1 id="19i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A continuous homomorphism $G\to O(n)$ is immediately an $n$-dimensional real [group representation](../../../../../../group-representation.md) by composing with the inclusion $O(n)\subset GL_n(\mathbb R)$.

Conversely, let $\pi:G\to GL(V)$ be a continuous real representation with $\dim_{\mathbb R}V=n$. Choose any positive-definite inner product $(\ ,\ )_0$ on $V$ and normalized [Haar measure](../../../../../../haar-measure.md) $dg$ on $G$. Define

$$
(v,w)_G=\int_G(\pi(g)v,\pi(g)w)_0\,dg.
$$

This is bilinear and symmetric. It is positive definite because the continuous nonnegative integrand $(\pi(g)v,\pi(g)v)_0$ is positive at every $g$ whenever $v\ne0$. Right invariance of normalized Haar measure on a compact group gives

$$
(\pi(h)v,\pi(h)w)_G
=\int_G(\pi(gh)v,\pi(gh)w)_0\,dg
=(v,w)_G.
$$

Choose an orthonormal basis for this averaged form. In that basis every $\pi(h)$ lies in $O(n)$, proving the [orthogonalization of a compact-group representation](../../../../../../orthogonalization-of-a-compact-group-representation.md) and the stated equivalence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19I](../../19i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
