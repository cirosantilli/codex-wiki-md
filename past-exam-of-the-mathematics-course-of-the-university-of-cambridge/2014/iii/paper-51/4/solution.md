<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $w=x^1+ix^2$, $z=x^3+ix^4$. The [Euclidean metric](../../../../../euclidean-metric.md) is $\sum_a(dx^a)^2$, and the printed four-form is $4\,dx^1\wedge dx^2\wedge dx^3\wedge dx^4$, so it specifies the usual positive [orientation](../../../../../orientation-of-a-simplex.md). The normalized metric [volume form](../../../../../volume-form.md) is one quarter of that expression. The [self-dual frame in complex Euclidean coordinates](../../../../../self-dual-frame-in-complex-euclidean-coordinates.md) is

$$
\begin{aligned}
\omega_1&=dx^1\wedge dx^3-dx^2\wedge dx^4,\\
\omega_2&=dx^1\wedge dx^4+dx^2\wedge dx^3,\\
\omega_3&=2(dx^1\wedge dx^2+dx^3\wedge dx^4).
\end{aligned}
$$

These are real and have the required complex combinations. For the [Hodge star operator](../../../../../hodge-star-operator.md) with this [orientation](../../../../../orientation-of-a-simplex.md),

$$
*(dx^1\wedge dx^2)=dx^3\wedge dx^4,\qquad
*(dx^1\wedge dx^3)=-dx^2\wedge dx^4,\qquad
*(dx^1\wedge dx^4)=dx^2\wedge dx^3,
$$

and applying $*$ again gives the reverse relations. Thus $*\omega_i=\omega_i$. They are linearly independent, while the $+1$ eigenspace of $*$ on [2-forms](../../../../../2-form.md) has dimension three, proving **they span $\Lambda^2_+$**. The TeX aid incorrectly reads the subscript as $1$.

The [ASDYM equations](../../../../../anti-self-dual-yang-mills-equations.md) require the self-dual projection of the [gauge field strength](../../../../../gauge-field-strength.md) to vanish. Orthogonality to $\omega_1,\omega_2$ sets its $(2,0)$ and $(0,2)$ parts to zero; orthogonality to $\omega_3$ removes the trace of its $(1,1)$ part. Explicitly, if $F=\sum_{a<b}f_{ab}\,dx^a\wedge dx^b$, these conditions are $f_{13}-f_{24}=0$, $f_{14}+f_{23}=0$ and $f_{12}+f_{34}=0$. Since

$$
F_{wz}=\tfrac14\{f_{13}-f_{24}-i(f_{14}+f_{23})\},\qquad
F_{w\bar w}+F_{z\bar z}=\tfrac i2(f_{12}+f_{34}),
$$

and the conjugate equation supplies the other complex component for a real [curvature form of a connection](../../../../../curvature-form.md), the equivalent system is

$$
\boxed{F_{wz}=0,\qquad F_{w\bar w}+F_{z\bar z}=0,\qquad F_{\bar w\bar z}=0.}
$$

To obtain the [complex potential reduction of anti-self-dual Yang-Mills](../../../../../complex-potential-reduction-of-anti-self-dual-yang-mills.md), set $D_w=\partial_w+A_w$, $D_z=\partial_z+A_z$. The first equation is the integrability condition $[D_w,D_z]=0$. Locally it allows an invertible complex matrix $s$ satisfying $\partial_ws=-A_ws$ and $\partial_zs=-A_zs$. The [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) $A\mapsto s^{-1}As+s^{-1}ds$ consequently gives $A_w=A_z=0$. This is a complex gauge; a real compact [gauge group](../../../../../gauge-group.md) alone generally cannot implement it.

In this gauge the second equation becomes

$$
\partial_wA_{\bar w}+\partial_zA_{\bar z}=0.
$$

Thus the one-form $A_{\bar w}\,dz-A_{\bar z}\,dw$ is closed with respect to the exterior derivative in the $(w,z)$ directions. The local complex version of the [Poincaré lemma](../../../../../poincare-lemma.md) gives a potential $K$ such that

$$
\boxed{A_w=A_z=0,\qquad A_{\bar w}=\partial_zK,\qquad A_{\bar z}=-\partial_wK.}
$$

Because the gauge transformation is complex, $K$ is generally valued in the [complexification of a Lie algebra](../../../../../complexification-of-a-lie-algebra.md) $\mathfrak g_{\mathbb C}$; the printed $\mathfrak g$ must be understood in that sense. The elementary reduction is local, and the transformed fields retain a reality condition inherited from the original real connection. For the usual compact matrix gauge groups and smooth fields on all of $\mathbb R^4=\mathbb C^2$, the gauge and potential can also be chosen globally if no condition at infinity is imposed. The flat partial connection defines a holomorphic [principal bundle](../../../../../principal-bundle.md) on the conjugate complex space. That base is a contractible [Stein manifold](../../../../../stein-manifold.md), so the [Oka-Grauert principle](../../../../../oka-grauert-principle.md) gives a global trivialization and hence a global complex gauge. After that trivialization, the conjugate of [Stein vanishing for the Dolbeault cohomology of functions](../../../../../stein-vanishing-for-the-dolbeault-cohomology-of-functions.md) gives a global primitive $K$, component by component in $\mathfrak g_{\mathbb C}$. Prescribed framing or decay at infinity requires a separate compatibility check and is not automatically preserved by this gauge.

Substitute the potential into the remaining [ASDYM equations](../../../../../anti-self-dual-yang-mills-equations.md) component:

$$
\begin{aligned}
F_{\bar w\bar z}
&=\partial_{\bar w}(-K_w)-\partial_{\bar z}K_z+[K_z,-K_w]\\
&=-K_{w\bar w}-K_{z\bar z}+[K_w,K_z].
\end{aligned}
$$

Therefore all three [ASDYM equations](../../../../../anti-self-dual-yang-mills-equations.md) reduce to the single [ASDYM potential equation](../../../../../complex-potential-reduction-of-anti-self-dual-yang-mills.md)

$$
\boxed{K_{w\bar w}+K_{z\bar z}-[K_w,K_z]=0.}
$$

The sign follows directly from $A_{\bar z}=-K_w$; changing a potential convention would change the displayed commutator sign. Conversely, this equation and the displayed gauge reconstruction make all three curvature conditions vanish, subject to the inherited reality condition when a real [gauge field](../../../../../gauge-field.md) is required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
