<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiating $f(\mu,\sigma)=\mathbb E[U(\mu+\sigma Z)]$ twice gives the [Hessian matrix](../../../../../../hessian-matrix.md)

$$
\operatorname{Hess}f
=\begin{pmatrix}
\mathbb E[U''(X)]&\mathbb E[ZU''(X)]\\
\mathbb E[ZU''(X)]&\mathbb E[Z^2U''(X)]
\end{pmatrix}
=\mathbb E\left[U''(X)
\begin{pmatrix}1\\Z\end{pmatrix}
\begin{pmatrix}1&Z\end{pmatrix}\right].
$$

For every vector $(a,b)$,

$$
\begin{pmatrix}a&b\end{pmatrix}
(\operatorname{Hess}f)
\begin{pmatrix}a\\b\end{pmatrix}
=\mathbb E[U''(X)(a+bZ)^2]\leq0.
$$

Thus the Hessian is a [negative semidefinite matrix](../../../../../../negative-semidefinite-matrix.md), and

$$
\boxed{f\text{ is jointly concave in }(\mu,\sigma)}.
$$

Equivalently, with $W=-U''(X)\geq0$, its determinant is

$$
\mathbb EW\,\mathbb E[Z^2W]-(\mathbb E[ZW])^2\geq0
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), while both diagonal entries are nonpositive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
