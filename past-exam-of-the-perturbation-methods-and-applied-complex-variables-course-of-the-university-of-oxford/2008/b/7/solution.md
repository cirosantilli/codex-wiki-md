<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Orient $\Gamma$ and label its left side plus and its right side minus. Assume the density is [Hölder continuity](../../../../holder-condition.md) near the point in question, or has sufficient regularity for the boundary limits below. The source does not explicitly state this regularity assumption. Parametrize locally by oriented arclength $\gamma(s)$, with $\gamma(0)=t$. Define the [Cauchy principal value](../../../../cauchy-principal-value.md) by removing equal arclengths on the two sides:

$$
\operatorname{PV}\int_\Gamma\frac{f(\zeta)}{\zeta-t}\,d\zeta
:=\lim_{\eta\downarrow0}
\int_{\Gamma\setminus\gamma((-\eta,\eta))}
\frac{f(\zeta)}{\zeta-t}\,d\zeta.
$$

Subtract $f(t)$ from the numerator near $t$. The [Hölder continuity](../../../../holder-condition.md) remainder is locally bounded in absolute value by a constant times $|s|^{\nu-1}$ for some $\nu>0$, so its integral has the same limit from the two sides. The constant part contributes half the [residue](../../../../residue.md), with sign determined by the side of the small [semicircle](../../../../semicircle.md). This proves the [Sokhotski–Plemelj theorem](../../../../sokhotski-plemelj-theorem.md)

$$
\boxed{w_\pm(t)=\pm\frac{f(t)}2+
\frac1{2\pi i}\operatorname{PV}\int_\Gamma
\frac{f(\zeta)}{\zeta-t}\,d\zeta.}
$$

In particular $f=w_+-w_-$ and the [Cauchy principal value](../../../../cauchy-principal-value.md) term with coefficient $1/(\pi i)$ equals $w_++w_-$. Substituting these two identities into the [singular integral equation](../../../../singular-integral-equation.md) gives

$$
\boxed{(a+b)w_++(b-a)w_-=c.}
$$

Choose a canonical homogeneous solution $\widetilde w$ whose boundary values do not vanish, and account for any permitted zeros or [poles](../../../../pole.md) when forming a quotient. The assumptions $a\pm b\neq0$ alone do not ensure that an arbitrary homogeneous solution has this property. Its jump relation is

$$
(a+b)\widetilde w_+=(a-b)\widetilde w_-.
$$

Dividing the inhomogeneous relation by $(a+b)\widetilde w_+$ therefore gives

$$
\left(\frac w{\widetilde w}\right)_+
-\left(\frac w{\widetilde w}\right)_-
=\rho,\qquad
\rho=\frac{c}{(a+b)\widetilde w_+}.
$$

The [Cauchy integral](../../../../cauchy-transform.md) solves this additive jump. More generally every solution in the chosen analytic class has

$$
w(z)=\widetilde w(z)
\left[\frac1{2\pi i}\int_\Gamma
\frac{\rho(\zeta)}{\zeta-z}\,d\zeta+H(z)\right],
$$

where $H$ has no jump across $\Gamma$ and obeys the applicable growth, endpoint and divisor conditions. Setting $H=0$ gives exactly the intermediate formula printed in the source.

Let $C\rho=(2\pi i)^{-1}\operatorname{PV}\int_\Gamma\rho(\zeta)/(\zeta-t)d\zeta$. Applying [Sokhotski–Plemelj theorem](../../../../sokhotski-plemelj-theorem.md) to the displayed solution and subtracting boundary values yields

$$
f=(\widetilde w_+-\widetilde w_-)C\rho
+\tfrac12(\widetilde w_++\widetilde w_-)\rho
+(\widetilde w_+-\widetilde w_-)H.
$$

Use

$$
\widetilde w_+-\widetilde w_-
=-\frac{2b\widetilde w_+}{a-b},
\qquad
\widetilde w_++\widetilde w_-
=\frac{2a\widetilde w_+}{a-b}.
$$

The normalized particular solution is consequently

$$
f_{\rm p}(t)=
-\frac{b(t)\widetilde w_+(t)}{a(t)-b(t)}
\frac1{\pi i}\operatorname{PV}\int_\Gamma
\frac{c(\zeta)}{(a(\zeta)+b(\zeta))\widetilde w_+(\zeta)}
\frac{d\zeta}{\zeta-t}
+\frac{a(t)c(t)}{a(t)^2-b(t)^2},
$$

and the full solution is

$$
\boxed{f=f_{\rm p}-\frac{2b\widetilde w_+}{a-b}H.}
$$

Thus the printed expression is a **particular solution; homogeneous terms need separate normalization**. To see why “general” cannot hold without qualification, take the positively oriented [unit circle](../../../../complex-unit-circle.md), $a=(1+z)/2$, $b=(1-z)/2$, and $c=0$. Then $a+b=1$ and $a-b=z$ are nonzero on the [contour](../../../../complex-integration-contour.md). The analytic pair $\widetilde w_+=1$, $\widetilde w_-=1/z$ satisfies the homogeneous jump and decays on the exterior side. Its nonzero density $f=1-1/z$ has these very Cauchy boundary values and solves the original homogeneous equation, whereas the source formula with $c=0$ gives zero. This is [homogeneous freedom in a scalar singular integral equation](../../../../homogeneous-freedom-in-a-scalar-singular-integral-equation.md); endpoint and index conditions determine which jump-free additions are permitted.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../split.md)
5. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
