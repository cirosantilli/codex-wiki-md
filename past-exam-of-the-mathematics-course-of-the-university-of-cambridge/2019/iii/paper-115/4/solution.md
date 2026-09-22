<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Levi-Civita connection](../../../../../levi-civita-connection.md) of a [Riemannian manifold](../../../../../riemannian-manifold.md) $(M,g)$ is the unique [connection on a vector bundle](../../../../../connection-vector-bundle.md) on $TM$ that is [torsion-free](../../../../../torsion-free-connection.md) and compatible with the [Riemannian metric](../../../../../riemannian-metric.md). Any such connection must satisfy the [Koszul formula](../../../../../koszul-formula.md)

$$
\begin{aligned}
2g(\nabla_XY,Z)={}&Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)\\
&-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
\end{aligned}
$$

Nondegeneracy of $g$ determines $\nabla_XY$ uniquely from the right-hand side. Conversely, define $\nabla$ by this formula. Direct substitution shows that it is $C^\infty$-linear in $X$, satisfies the [Leibniz rule](../../../../../leibniz-rule.md) in $Y$, preserves $g$, and obeys $\nabla_XY-\nabla_YX=[X,Y]$. It is therefore a torsion-free metric connection. This proves the [existence and uniqueness of the Levi-Civita connection](../../../../../existence-and-uniqueness-of-the-levi-civita-connection.md).

For the metric vector bundle $E$, choose the stated orthonormal local frame $(e_1,\ldots,e_m)$ and write $d_Ae_j=A^i{}_j e_i$. Since $\langle e_i,e_j\rangle=\delta_{ij}$, metric compatibility gives

$$
0=d\langle e_i,e_j\rangle
=\langle d_Ae_i,e_j\rangle+\langle e_i,d_Ae_j\rangle
=A^j{}_i+A^i{}_j.
$$

Hence the [connection matrix in an orthonormal frame is skew-symmetric](../../../../../connection-matrix-in-an-orthonormal-frame-is-skew-symmetric.md):

$$
\boxed{A^i{}_j=-A^j{}_i.}
$$

On an oriented Riemannian $d$-manifold, the [Hodge star operator](../../../../../hodge-star-operator.md) is defined by

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle\,d\operatorname{vol}_g.
$$

It is an orthogonal map $*:\Lambda^rT_x^*M\to\Lambda^{d-r}T_x^*M$ and satisfies $*^2=(-1)^{r(d-r)}$. In dimension $d=2n$ on middle-degree forms, the [Adjoint of the Hodge star on middle-degree forms](../../../../../adjoint-of-the-hodge-star-on-middle-degree-forms.md) is

$$
*^\dagger=*^{-1}=(-1)^{n^2}*.
$$

Thus it is self-adjoint when $n$ is even, but **it is not always self-adjoint**. For $n=1$ on the oriented Euclidean plane,

$$
*dx=dy,
\qquad *dy=-dx,
$$

so its matrix in the orthonormal basis $(dx,dy)$ is skew-adjoint.

The [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) on differential forms is the [Hodge Laplacian](../../../../../hodge-laplacian.md)

$$
\Delta=d\delta+\delta d,
$$

where the [codifferential](../../../../../codifferential.md) $\delta$ is the formal $L^2$ adjoint of the [exterior derivative](../../../../../exterior-derivative.md). On a compact manifold without boundary, if $\Delta\omega=\lambda\omega$ for a nonzero differential form $\omega$, then [integration by parts](../../../../../integration-by-parts.md) gives

$$
\lambda\lVert\omega\rVert_{L^2}^2
=\langle\Delta\omega,\omega\rangle_{L^2}
=\lVert d\omega\rVert_{L^2}^2+\lVert\delta\omega\rVert_{L^2}^2\geq0.
$$

Therefore the [nonnegativity of the Hodge Laplacian](../../../../../nonnegativity-of-the-hodge-laplacian.md) yields

$$
\boxed{\lambda\geq0.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
