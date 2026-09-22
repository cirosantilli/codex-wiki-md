<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

There is a small domain issue in the printed notation. If $\mathbb R^3/\mathbb R^2$ means a [quotient vector space](../../../../../quotient-vector-space.md) by the horizontal plane, the displayed formula does not descend to that [quotient vector space](../../../../../quotient-vector-space.md): $(0,0,0)$ and $(1,0,0)$ represent the same class but give different values. The intended construction is [stereographic projection](../../../../../stereographic-projection.md), restricted to the unit [sphere](../../../../../sphere.md) with the north pole removed. Interpreting the slash as removal of the plane $z=1$ also supplies a suitable ambient domain. The [holomorphic stereographic atlas of the sphere](../../../../../holomorphic-stereographic-atlas-of-the-sphere.md) is obtained as follows.

Write $N=(0,0,1)$ and $S=(0,0,-1)$. On $U_N=S^2\setminus\{N\}$ use $\zeta=(x+iy)/(1-z)$. Its inverse, with $\zeta=u+iv$, is

$$
x=\frac{2u}{1+u^2+v^2},\qquad
y=\frac{2v}{1+u^2+v^2},\qquad
z=\frac{u^2+v^2-1}{1+u^2+v^2}.
$$

These formulas give a smooth [manifold chart](../../../../../manifold-chart.md) from $U_N$ onto $\mathbb C$. On $U_S=S^2\setminus\{S\}$ choose the second [manifold chart](../../../../../manifold-chart.md)

$$
\eta=\frac{x-iy}{1+z}.
$$

Its inverse is $x=2\operatorname{Re}\eta/(1+|\eta|^2)$, $y=-2\operatorname{Im}\eta/(1+|\eta|^2)$ and $z=(1-|\eta|^2)/(1+|\eta|^2)$, so this is also a smooth [manifold chart](../../../../../manifold-chart.md) onto $\mathbb C$. The conjugation in this second [stereographic projection](../../../../../stereographic-projection.md) is essential. On the overlap, $x^2+y^2=1-z^2$, so

$$
\zeta\eta=\frac{x^2+y^2}{1-z^2}=1,\qquad
\boxed{\eta=\zeta^{-1}}.
$$

Both directions of this transition are [holomorphic maps](../../../../../holomorphic-map.md) on $\mathbb C^\times$, with nonzero derivative. The two [manifold charts](../../../../../manifold-chart.md) cover the [sphere](../../../../../sphere.md), hence define a [holomorphic atlas](../../../../../holomorphic-atlas.md), giving precisely the [Riemann sphere](../../../../../riemann-sphere.md). If one instead used $x+iy$ in both [manifold charts](../../../../../manifold-chart.md), the transition would be $1/\bar\zeta$ and would not be [holomorphic](../../../../../complex-differentiability-at-a-point.md).

Orient the [sphere](../../../../../sphere.md) by this [holomorphic atlas](../../../../../holomorphic-atlas.md). The given [volume form](../../../../../volume-form.md) is smooth at infinity: replacing $\zeta$ by $1/\eta$ in its [exterior product](../../../../../exterior-product.md) gives the same expression

$$
\Omega=\frac{i\,d\eta\wedge d\bar\eta}{(1+|\eta|^2)^2}.
$$

Moreover, $i\,d\zeta\wedge d\bar\zeta=2\,du\wedge dv$, so the normalization of this [volume form](../../../../../volume-form.md) is

$$
\int_{S^2}\Omega
=2\int_0^{2\pi}\int_0^\infty\frac{r}{(1+r^2)^2}\,dr\,d\theta
=2\pi.
$$

Thus the printed [volume form](../../../../../volume-form.md) has half the area of the standard round unit [sphere](../../../../../sphere.md); replacing its integral by $4\pi$ would introduce an erroneous factor of two.

For $k\ge1$, the [holomorphic map](../../../../../holomorphic-map.md) $f(\zeta)=\zeta^k$ extends over infinity, since the target reciprocal coordinate is $\eta^k$ when the source reciprocal coordinate is $\eta$. Its [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) is

$$
f^*\Omega=\frac{i\,k^2|\zeta|^{2k-2}\,d\zeta\wedge d\bar\zeta}
{(1+|\zeta|^{2k})^2}.
$$

Using $s=r^{2k}$ gives

$$
\int_{S^2}f^*\Omega
=4\pi k^2\int_0^\infty\frac{r^{2k-1}}{(1+r^{2k})^2}\,dr
=2\pi k\int_0^\infty\frac{ds}{(1+s)^2}
=2\pi k.
$$

The [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) is therefore

$$
\boxed{\deg f=\frac{\int_{S^2}f^*\Omega}{\int_{S^2}\Omega}=k}.
$$

For $k=0$, the formula on the finite [manifold chart](../../../../../manifold-chart.md) is the constant $1$. Its unique continuous extension is also $1$ at infinity, rather than an undefined expression $\infty^0$. Its [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) is zero and its [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) is **zero**.

For the preimage calculation when $k\ge1$, choose a [regular value](../../../../../regular-value.md) $w\in\mathbb C^\times$. There are exactly $k$ distinct roots of $\zeta^k=w$. At each root the real [Jacobian determinant](../../../../../jacobian-determinant.md) is $|k\zeta^{k-1}|^2>0$, so every local contribution to the [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) is $+1$. Their sum is $k$, agreeing with the integral. The exceptional values $0$ and infinity are avoided because they are branch values when $k>1$. For the constant map, any $w\ne1$ is a [regular value](../../../../../regular-value.md) with no preimages, giving the same answer zero. This establishes the [degree of a power map of the Riemann sphere](../../../../../degree-of-a-power-map-of-the-riemann-sphere.md) for every allowed $k$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
