<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Levi-Civita connection](../../../../../levi-civita-connection.md) on a [Riemannian manifold](../../../../../riemannian-manifold.md) is a [covariant derivative](../../../../../covariant-derivative.md) $D$ that is a [torsion-free connection](../../../../../torsion-free-connection.md), $D_XY-D_YX=[X,Y]$, and a [metric connection](../../../../../metric-connection.md), $Xg(Y,Z)=g(D_XY,Z)+g(Y,D_XZ)$. A [covariant derivative](../../../../../covariant-derivative.md) is $C^\infty(M)$-linear in $X$, real linear in $Y$, and obeys $D_X(fY)=X(f)Y+fD_XY$.

Combining metric compatibility for the cyclic triples and eliminating reversed derivatives with the torsion identity gives the [Koszul formula](../../../../../koszul-formula.md)

$$
2g(D_XY,Z)=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

Since $g$ is nondegenerate, this determines $D_XY$ uniquely. For existence, use the right-hand side to define $D_XY$: expansion of the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) shows it is $C^\infty(M)$-linear in $Z$, hence defines a smooth one-form, which the [musical isomorphism](../../../../../musical-isomorphism.md) converts to a smooth [vector field](../../../../../vector-field.md). The same expansion shows $D_{fX}Y=fD_XY$ and $D_X(fY)=X(f)Y+fD_XY$. Subtracting the formula with $X,Y$ exchanged gives torsion zero; adding its versions for $Y,Z$ exchanged gives metric compatibility. Thus it is a [Levi-Civita connection](../../../../../levi-civita-connection.md). Equivalently its coefficients in a [manifold chart](../../../../../manifold-chart.md) are the [Christoffel symbols](../../../../../christoffel-symbol.md)

$$
\Gamma^k_{ij}=\frac12 g^{k\ell}(\partial_i g_{j\ell}+\partial_j g_{i\ell}-\partial_\ell g_{ij}).
$$

The intrinsically defined [Koszul formula](../../../../../koszul-formula.md) ensures these local expressions fit together. This proves the [fundamental theorem of Riemannian geometry](../../../../../fundamental-theorem-of-riemannian-geometry.md).

The [product Riemannian metric](../../../../../product-riemannian-metric.md) on $M\times N$ is

$$
g_{(m,n)}((u,v),(u',v'))=(g_M)_m(u,u')+(g_N)_n(v,v').
$$

The two factor tangent spaces are orthogonal, and the sum is positive definite. Lift $X$ from $M$ and $Y$ from $N$. We check $D_XY$ against lifted local frame fields from both factors, which together span each product tangent space.

If $Z$ is lifted from $M$, then $g(Y,Z)=g(X,Y)=0$, while $g(Z,X)$ depends only on $m$, so $Yg(Z,X)=0$. Also $[Y,Z]=[X,Y]=0$ and $[Z,X]$ is horizontal, hence orthogonal to $Y$. Every term in the [Koszul formula](../../../../../koszul-formula.md) is zero. If $W$ is lifted from $N$, $g(W,X)=g(X,Y)=0$ and $g(Y,W)$ depends only on $n$, so $Xg(Y,W)=0$. Now $[W,X]=[X,Y]=0$ and $[Y,W]$ is vertical, hence orthogonal to $X$. Again every term is zero. Thus $D_XY$ is orthogonal to both spanning frame families, and positive definiteness yields

$$
\boxed{D_XY=0.}
$$

This calculation uses the lifts' independence of the other factor coordinates; a vector field with varying coefficients in those coordinates can have a nonzero mixed derivative.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
