<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $D$ be the [Levi-Civita connection](../../../../../levi-civita-connection.md) of the [Riemannian metric](../../../../../riemannian-metric.md). We use the curvature sign specified in the question, the negative of the usual vector-bundle curvature convention in Question 4. Extend $D$ to the [covariant exterior derivative](../../../../../exterior-covariant-derivative.md) on tangent-bundle-valued forms and define the curvature two-form by $R=-D^2$. In a local frame with [connection matrix](../../../../../connection-one-form.md) $A$, it is the endomorphism-valued two-form $-(dA+A\wedge A)$. The transformation law for $A$ makes this transform by conjugation, so it is an intrinsic tensor. It measures the infinitesimal failure of parallel derivatives to commute, with this chosen sign.

For a tangent-bundle-valued one-form $\eta$, the covariant exterior derivative is

$$
(D\eta)(X,Y)=D_X(\eta(Y))-D_Y(\eta(X))-\eta([X,Y]).
$$

Apply this to the one-form $DZ$, for which $(DZ)(Y)=D_YZ$. This calculation proves, rather than just renames, the operator expression

$$
\boxed{R(X,Y)Z=D_{[X,Y]}Z-D_XD_YZ+D_YD_XZ,\qquad
R(X,Y)=D_{[X,Y]}-[D_X,D_Y].}
$$

It is linear over smooth functions in $Z$: the extra first- and second-derivative terms in $R(X,Y)(fZ)$ cancel by $[X,Y]f=X(Yf)-Y(Xf)$. The connection's linearity in its vector-field argument similarly shows linearity over smooth functions in $X$ and $Y$. Thus $R(X,Y)$ is an [endomorphism](../../../../../endomorphism.md) of the [tangent bundle](../../../../../tangent-bundle.md), not a differential operator on its sections, and $R$ is a well-defined endomorphism-valued two-form.

The torsion-free identity is $D_XY-D_YX=[X,Y]$. Expand the cyclic curvature sum and use this identity to obtain

$$
\begin{aligned}
\sum_{\mathrm{cyc}}R(X,Y)Z
&=\sum_{\mathrm{cyc}}D_{[X,Y]}Z-
\sum_{\mathrm{cyc}}D_X(D_YZ-D_ZY)\\
&=\sum_{\mathrm{cyc}}\big(D_{[Y,Z]}X-D_X[Y,Z]\big)\\
&=\sum_{\mathrm{cyc}}[[Y,Z],X]=0.
\end{aligned}
$$

The last equality is the [Jacobi identity](../../../../../jacobi-identity.md) for the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md). This proves the [first Bianchi identity](../../../../../first-bianchi-identity.md)

$$
\boxed{R(X,Y)Z+R(Y,Z)X+R(Z,X)Y=0.}
$$

Lower the output index with the metric and define the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) by

$$
\mathcal R(X,Y,Z,W)=g(R(X,Y)Z,W),\qquad
R_{ij,kl}=\mathcal R(e_i,e_j,e_k,e_l).
$$

This is a covariant four-tensor, because the curvature endomorphism is tensorial in all three inputs. Skew-symmetry of the curvature two-form immediately gives $R_{ji,kl}=-R_{ij,kl}$.

Metric compatibility gives the second skew-symmetry. Apply the scalar operator $[X,Y]-XY+YX$, which is zero, to $g(Z,W)$. Expanding each derivative using $Dg=0$ cancels the mixed products of first derivatives and leaves

$$
0=g(R(X,Y)Z,W)+g(Z,R(X,Y)W).
$$

Thus $R_{ij,lk}=-R_{ij,kl}$.

For a direct proof of pair interchange, choose the [geodesic coordinates](../../../../../normal-coordinates.md) of Question 5 at an arbitrary point $p$. There $\Gamma(p)=0$ and $\partial g(p)=0$. Write $D_{\partial_i}\partial_k=\Gamma^a{}_{ik}\partial_a$. The operator formula gives, at $p$,

$$
R_{ij,kl}=g_{al}\big(\partial_j\Gamma^a{}_{ik}-\partial_i\Gamma^a{}_{jk}\big).
$$

The Levi-Civita formula is $g_{al}\Gamma^a{}_{jk}=\tfrac12(\partial_jg_{kl}+\partial_kg_{jl}-\partial_lg_{jk})$. Differentiating at $p$, the products involving first derivatives of the metric and Christoffel coefficients vanish. The terms $\partial_i\partial_jg_{kl}$ cancel, leaving

$$
\boxed{R_{ij,kl}(p)=\tfrac12
\big(g_{jk,il}+g_{il,jk}-g_{jl,ik}-g_{ik,jl}\big)(p).}
$$

Here a comma denotes ordinary coordinate derivatives at the normal-coordinate center. Swapping $(i,j)$ with $(k,l)$ leaves this expression unchanged, by symmetry of $g$ and commutation of its second partial derivatives. This is the [pair symmetry from the normal-coordinate curvature formula](../../../../../pair-symmetry-from-the-normal-coordinate-curvature-formula.md). Since $p$ was arbitrary and the equality is tensorial, it holds in every frame. We have proved all the requested symmetries:

$$
\boxed{-R_{ji,kl}=R_{ij,kl}=-R_{ij,lk},\qquad R_{ij,kl}=R_{kl,ij}.}
$$

Changing the overall curvature sign would change the displayed coordinate formula's sign, but would not change the first Bianchi identity or any of these algebraic symmetries.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
