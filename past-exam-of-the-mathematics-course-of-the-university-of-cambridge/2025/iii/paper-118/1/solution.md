<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Hermitian metric on a holomorphic vector bundle](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) $E\to X$ is a smoothly varying family of positive-definite [Hermitian forms](../../../../../hermitian-form.md) $h_x$ on its fibers. A [Chern connection](../../../../../chern-connection.md) is a [connection on a vector bundle](../../../../../connection-vector-bundle.md) $\nabla$ that is compatible with $h$ and whose $(0,1)$ part is the bundle's [Dolbeault partial connection](../../../../../dolbeault-partial-connection.md), $\nabla^{0,1}=\bar\partial_E$.

Choose a local holomorphic frame $e$ and write $h=h(e,e)>0$. The connection form in this frame is

$$
\theta=h^{-1}\partial h=\partial\log h,
\qquad \nabla e=\theta\otimes e.
$$

If $e'=ge$ for a nowhere-zero [holomorphic function](../../../../../holomorphic-function.md) $g$, then $h'=|g|^2h$ and

$$
\theta'=\partial\log h'=\theta+g^{-1}\partial g,
$$

which is exactly the [connection-form transformation law](../../../../../connection-vector-bundle.md). The local formulas therefore define a global connection.

Identify $\mathcal O(-1)$ with the [tautological bundle](../../../../../tautological-bundle.md) over [Complex projective space](../../../../../complex-projective-space.md). The standard [Hermitian inner product](../../../../../hermitian-form.md) of $\mathbb C^{n+1}$ restricts to each tautological line. On the affine chart $U_i=\{Z_i\ne0\}$, put $w_j=Z_j/Z_i$ for $j\ne i$ and use the holomorphic frame

$$
s_i(w)=(w_0,\ldots,w_{i-1},1,w_{i+1},\ldots,w_n).
$$

Then

$$
h_i(s_i,s_i)=1+\sum_{j\ne i}|w_j|^2,
\qquad
\theta_i=\frac{\sum_{j\ne i}\overline w_j\,dw_j}{1+\sum_{j\ne i}|w_j|^2}.
$$

The [curvature form of a connection](../../../../../curvature-form.md) is

$$
F_\nabla=\bar\partial\theta_i=-\partial\bar\partial\log(1+|w|^2).
$$

Consequently [Chern-Weil theory](../../../../../first-chern-class.md) gives the closed representative

$$
c_1(\mathcal O(-1))=\left[\frac{iF_\nabla}{2\pi}\right]
=\left[-\frac{i}{2\pi}\partial\bar\partial\log(1+|w|^2)\right]
=-\left[\frac{\omega_{FS}}{2\pi}\right],
$$

where $\omega_{FS}$ is the [Fubini-Study form](../../../../../fubini-study-form.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
