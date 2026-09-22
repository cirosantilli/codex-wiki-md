<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Levi-Civita connection](../../../../../levi-civita-connection.md) is a connection on the [tangent bundle](../../../../../tangent-bundle.md) which is [torsion-free](../../../../../torsion-free-connection.md) and compatible with the [Riemannian metric](../../../../../riemannian-metric.md). Its defining identities are

$$
\nabla_XY-\nabla_YX=[X,Y],\qquad
Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

To obtain uniqueness, write the metric identity for $(X,Y,Z)$, $(Y,Z,X)$ and $(Z,X,Y)$, add the first two and subtract the third, and use the torsion identity to interchange the derivatives. This gives the [Koszul formula](../../../../../koszul-formula.md)

$$
\begin{aligned}
2g(\nabla_XY,Z)
={}&Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)\\
&-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
\end{aligned}
$$

The metric is nondegenerate, so these [inner products](../../../../../inner-product.md) determine $\nabla_XY$ uniquely.

For existence, let $K(X,Y,Z)$ denote the right-hand side. The bracket rules $[X,fY]=f[X,Y]+X(f)Y$ and $[fX,Y]=f[X,Y]-Y(f)X$ give, by cancellation of all extra derivatives,

$$
\begin{aligned}
K(fX,Y,Z)&=fK(X,Y,Z),\\
K(X,fY,Z)&=fK(X,Y,Z)+2X(f)g(Y,Z),\\
K(X,Y,fZ)&=fK(X,Y,Z).
\end{aligned}
$$

Thus the nondegenerate metric defines a unique smooth [vector field](../../../../../vector-field.md) $\nabla_XY$ from $2g(\nabla_XY,Z)=K(X,Y,Z)$, and these identities give the connection rules. In coordinates the construction reads

$$
\boxed{\Gamma^k_{ij}=\frac12g^{k\ell}
\big(\partial_i g_{j\ell}+\partial_jg_{i\ell}-\partial_\ell g_{ij}\big).}
$$

The coefficients are smooth and symmetric in $i,j$, proving zero torsion. Substituting them gives

$$
g_{\ell k}\Gamma^\ell_{ij}+g_{j\ell}\Gamma^\ell_{ik}=\partial_i g_{jk},
$$

which is exactly [metric compatibility](../../../../../metric-compatibility.md). Since the construction was given intrinsically by $K$, the local formulas agree on overlaps. This proves [existence and uniqueness of the Levi-Civita connection](../../../../../existence-and-uniqueness-of-the-levi-civita-connection.md) on every [Riemannian manifold](../../../../../riemannian-manifold.md).

Define the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) by

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

The connection rules make this expression tensorial in all three arguments. To fix the component convention, throughout this solution use

$$
R_{ijkl}=g\big(R(e_i,e_j)e_l,e_k\big).
$$

With this convention, the unit [sphere](../../../../../sphere.md) has $R_{ijkl}=g_{ik}g_{jl}-g_{il}g_{jk}$ and positive [Ricci curvature](../../../../../ricci-curvature.md). In a coordinate frame, the components are obtained from

$$
\big(R(\partial_i,\partial_j)\partial_l\big)^a
=\partial_i\Gamma^a_{jl}-\partial_j\Gamma^a_{il}
+\Gamma^a_{ib}\Gamma^b_{jl}-\Gamma^a_{jb}\Gamma^b_{il}.
$$

The algebraic curvature symmetries are

$$
\boxed{R_{ijkl}=-R_{jikl}=-R_{ijlk},\qquad R_{ijkl}=R_{klij},}
$$

together with the [first Bianchi identity](../../../../../first-bianchi-identity.md)

$$
R(X,Y)Z+R(Y,Z)X+R(Z,X)Y=0,
\qquad R_{ijkl}+R_{jlki}+R_{likj}=0.
$$

The first antisymmetry follows from the definition. [Metric compatibility](../../../../../metric-compatibility.md) gives $g(R(X,Y)Z,W)+g(Z,R(X,Y)W)=0$, giving the second. Torsion-freeness reduces the cyclic sum to the [Jacobi identity](../../../../../jacobi-identity.md) for [Lie brackets of vector fields](../../../../../lie-bracket-of-vector-fields.md); pair interchange follows algebraically from these antisymmetries and the cyclic identity. These explain the identities rather than choosing unrelated sign conventions.

Define the [Ricci curvature](../../../../../ricci-curvature.md) by the [tensor contraction](../../../../../tensor-contraction.md)

$$
\operatorname{Ric}(Y,Z)=\operatorname{tr}\{X\mapsto R(X,Y)Z\},
\qquad \operatorname{Ric}_{jl}=g^{ik}R_{ijkl}.
$$

This is a [bilinear form](../../../../../bilinear-form.md), since $R$ is tensorial and [trace](../../../../../matrix-trace.md) is linear. At a point choose an orthonormal [basis](../../../../../basis.md). Pair interchange gives

$$
\operatorname{Ric}_{lj}=\sum_iR_{ilij}
=\sum_iR_{ijil}=\operatorname{Ric}_{jl},
$$

so **[Ricci curvature](../../../../../ricci-curvature.md) is symmetric**.

For the final determination in dimension three, an algebraic curvature tensor is determined by its entries in the three unordered index pairs $12,13,23$: antisymmetry removes repeated indices, and pair interchange makes the resulting $3\times3$ array symmetric. It therefore has at most six independent entries. Write

$$
K_{12}=R_{1212},\quad K_{13}=R_{1313},\quad K_{23}=R_{2323}.
$$

The diagonal Ricci components give

$$
\operatorname{Ric}_{11}=K_{12}+K_{13},\quad
\operatorname{Ric}_{22}=K_{12}+K_{23},\quad
\operatorname{Ric}_{33}=K_{13}+K_{23},
$$

so, for example, $K_{12}=(\operatorname{Ric}_{11}+\operatorname{Ric}_{22}-\operatorname{Ric}_{33})/2$, and the other two follow cyclically. The three off-diagonal entries are also recovered explicitly:

$$
R_{1323}=\operatorname{Ric}_{12},\qquad
R_{1223}=-\operatorname{Ric}_{13},\qquad
R_{1213}=\operatorname{Ric}_{23}.
$$

Thus every independent curvature entry is determined by Ricci; this proves injectivity, not merely a dimension count.

An invariant formula making the reconstruction explicit is, with $S=\operatorname{tr}_g\operatorname{Ric}$,

$$
\boxed{\begin{aligned}
R_{ijkl}={}&g_{ik}\operatorname{Ric}_{jl}+g_{jl}\operatorname{Ric}_{ik}
-g_{il}\operatorname{Ric}_{jk}-g_{jk}\operatorname{Ric}_{il}\\
&-\frac S2(g_{ik}g_{jl}-g_{il}g_{jk}).
\end{aligned}}
$$

To verify it, the right-hand side has the two antisymmetries, pair interchange and the cyclic identity by symmetry of $g$ and Ricci. Contracting its first and third indices in dimension three gives

$$
3\operatorname{Ric}_{jl}+Sg_{jl}-2\operatorname{Ric}_{jl}-Sg_{jl}
=\operatorname{Ric}_{jl}.
$$

Subtract it from the original tensor. The difference has zero Ricci contraction, and the six recovered-entry formulas above force it to vanish. This completes the proof of [three-dimensional curvature from the Ricci tensor](../../../../../three-dimensional-curvature-from-the-ricci-tensor.md) in arbitrary coordinates.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
