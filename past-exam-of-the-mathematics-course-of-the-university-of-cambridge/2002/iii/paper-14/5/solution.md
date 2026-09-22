<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Riemannian metric](../../../../../riemannian-metric.md) is a smooth positive-definite symmetric [inner product](../../../../../inner-product.md) $g_x$ on every [tangent space](../../../../../tangent-space.md). A [Levi-Civita connection](../../../../../levi-civita-connection.md) is a connection on the [tangent bundle](../../../../../tangent-bundle.md) which is torsion-free, $\nabla_XY-\nabla_YX=[X,Y]$, and metric-compatible,

$$
Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

Apply this identity with the cyclic triples $(X,Y,Z)$, $(Y,Z,X)$ and $(Z,X,Y)$, add the first two and subtract the third, and replace differences of covariant derivatives by [Lie brackets](../../../../../lie-bracket.md). The result is the [Koszul formula](../../../../../koszul-formula.md)

$$
\boxed{\begin{aligned}
2g(\nabla_XY,Z)={}&Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)\\
&-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
\end{aligned}}
$$

Its right side depends only on $g$ and the [vector fields](../../../../../vector-field.md); nondegeneracy of $g$ determines $\nabla_XY$ uniquely. This proves uniqueness.

For existence, in a coordinate chart define

$$
\Gamma^k_{ij}=\frac12g^{k\ell}(\partial_i g_{j\ell}+\partial_jg_{i\ell}-\partial_\ell g_{ij}),\qquad
(\nabla_XY)^k=X^i\partial_iY^k+\Gamma^k_{ij}X^iY^j.
$$

This is linear over smooth functions in $X$ and obeys the Leibniz rule in $Y$. Symmetry $\Gamma^k_{ij}=\Gamma^k_{ji}$ proves zero torsion, and direct substitution gives

$$
\partial_i g_{jk}=g_{\ell k}\Gamma^\ell_{ij}+g_{j\ell}\Gamma^\ell_{ik},
$$

which proves [metric compatibility](../../../../../metric-compatibility.md). On chart overlaps the two resulting connections satisfy the same intrinsic Koszul identity and therefore agree by uniqueness. They glue globally. Thus the [existence and uniqueness of the Levi-Civita connection](../../../../../existence-and-uniqueness-of-the-levi-civita-connection.md) holds on every [Riemannian manifold](../../../../../riemannian-manifold.md).

Fix the curvature convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

For coordinate vectors $e_i$, define the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) components by $R_{ij,kl}=g(R(e_i,e_j)e_l,e_k)$. In these indices the Ricci and scalar contractions are

$$
\boxed{\operatorname{Ric}_{jl}=g^{ik}R_{ij,kl},\qquad
s=g^{jl}\operatorname{Ric}_{jl}=g^{ik}g^{jl}R_{ij,kl}}.
$$

Explicitly, $R_{ij,kl}=g_{ka}R^a{}_{l ij}$, where

$$
R^a{}_{l ij}=\partial_i\Gamma^a_{jl}-\partial_j\Gamma^a_{il}
+\Gamma^a_{ip}\Gamma^p_{jl}-\Gamma^a_{jp}\Gamma^p_{il}.
$$

These expressions define [Ricci curvature](../../../../../ricci-curvature.md) and [scalar curvature](../../../../../scalar-curvature.md) without ambiguity about which indices are contracted. With this convention a round unit $m$-sphere has $\operatorname{Ric}=(m-1)g$ and $s=m(m-1)$.

If $\operatorname{Ric}=\lambda g$ with a constant real $\lambda$, tracing gives $\boxed{s=m\lambda}$, so every [Einstein metric](../../../../../einstein-metric.md) has constant [scalar curvature](../../../../../scalar-curvature.md). The converse is not valid in arbitrary dimension. On $S^2\times S^1$ with the [product Riemannian metric](../../../../../product-riemannian-metric.md) of the unit round sphere and a circle, the connection splits between factors. The mixed curvatures and circle curvature vanish, while the sphere has curvature one. Hence

$$
\boxed{\operatorname{Ric}=g_{S^2}\oplus0,\qquad s=2\text{ everywhere}}.
$$

A scalar multiple of the whole metric would require $\lambda=1$ on the sphere directions and $\lambda=0$ on the circle direction, which is impossible. This proves that [constant scalar curvature does not imply an Einstein metric](../../../../../constant-scalar-curvature-does-not-imply-an-einstein-metric.md), and supplies a counterexample to the unrestricted requested equivalence.

In dimension two, the curvature tensor is determined by the [Gaussian curvature](../../../../../gaussian-curvature.md) $K$:

$$
R_{ij,kl}=K(g_{ik}g_{jl}-g_{il}g_{jk}),\qquad
\operatorname{Ric}=Kg,\qquad s=2K.
$$

There the valid equivalence is

$$
\boxed{s\text{ constant}\iff\operatorname{Ric}=\lambda g\text{ with constant }\lambda=s/2}.
$$

In dimension one both curvature and [scalar curvature](../../../../../scalar-curvature.md) vanish identically. Without a two-dimensional restriction or another added geometric hypothesis, the general converse cannot be proved.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
