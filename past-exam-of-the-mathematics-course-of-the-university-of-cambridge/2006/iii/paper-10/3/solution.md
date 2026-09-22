<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $Y=\mathbb P^1\setminus\{0,1,\infty\}$. One concrete uniformization uses the image in $\operatorname{PSL}_2(\mathbb R)$ of the level-two [principal congruence subgroup](../../../../../principal-congruence-subgroup.md)

$$
\Gamma(2)=\left\{\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\operatorname{SL}_2(\mathbb Z):
a,d\text{ odd},\ b,c\text{ even}\right\}/\{\pm I\}.
$$

It acts on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) by [Möbius transformations](../../../../../mobius-transformation.md). Integer matrix entries make the group discrete, and the action is [properly discontinuous](../../../../../properly-discontinuous-group-action.md). There are no nonidentity elliptic stabilizers: an elliptic element would have integer even trace with absolute value less than two, hence trace zero. But then $d=-a$ gives $bc=-(a^2+1)\equiv2\pmod4$, contradicting the evenness of $b,c$. Thus the quotient is an ordinary [Riemann surface](../../../../../riemann-surfaces.md), with no orbifold points.

A fundamental region is the ideal quadrilateral

$$
\mathcal F=\{\tau\in\mathbb H:-1\leq\operatorname{Re}\tau\leq1,
\ |\tau-\tfrac12|\geq\tfrac12,
\ |\tau+\tfrac12|\geq\tfrac12\}.
$$

Its vertical sides are identified by $T(\tau)=\tau+2$, and its semicircular sides by $U(\tau)=\tau/(1-2\tau)$. The ideal vertices are $-1,0,1,\infty$; $-1$ and $1$ represent one puncture, while zero and infinity give two others. Filling these three punctures gives genus zero: the identified quadrilateral has three vertices, two paired edges and one face, so its compactification has Euler characteristic $3-2+1=2$. Its complex compactification is a sphere, and a [Möbius transformation](../../../../../mobius-transformation.md) puts the punctures at $0,1,\infty$. Hence

$$
\boxed{Y\cong\mathbb H/\Gamma(2).}
$$

This is the [thrice-punctured sphere as a modular quotient](../../../../../thrice-punctured-sphere-as-a-modular-quotient.md). Equivalently, the [uniformization theorem](../../../../../uniformization-theorem.md) applied to its [universal covering map](../../../../../universal-cover.md) produces the upper-half-plane model: the sphere cannot cover this noncompact surface, and an entire covering from $\mathbb C$ would contradict [Little Picard theorem](../../../../../little-picard-theorem.md) by omitting both zero and one.

The curvature-minus-one metric $ds_{\mathbb H}=|d\tau|/\operatorname{Im}\tau$ is invariant under every real [Möbius transformation](../../../../../mobius-transformation.md) preserving $\mathbb H$. Indeed, for determinant-one coefficients,

$$
\operatorname{Im}\frac{a\tau+b}{c\tau+d}
=\frac{\operatorname{Im}\tau}{|c\tau+d|^2},\qquad
\left|\frac{d}{d\tau}\frac{a\tau+b}{c\tau+d}\right|
=\frac1{|c\tau+d|^2}.
$$

Thus it descends to the [hyperbolic metric](../../../../../hyperbolic-metric.md) on $Y$. This defines its distance by the infimum of path lengths; a choice of local lift does not affect lengths.

For the [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md), first prove the [Schwarz lemma](../../../../../schwarz-lemma.md). If $h:\mathbb D\to\mathbb D$ is a [holomorphic function](../../../../../holomorphic-function.md) and $h(0)=0$, the function $h(z)/z$ extends as a [holomorphic function](../../../../../holomorphic-function.md) across zero. On $|z|=r$ its modulus is at most $1/r$. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) and $r\uparrow1$ yield $|h(z)|\leq|z|$ and $|h'(0)|\leq1$. Equality at a nonzero point or in the derivative makes $h(z)/z$ a constant of modulus one, again by the [maximum modulus principle](../../../../../maximum-modulus-principle.md), so $h$ is a rotation.

For a general [holomorphic function](../../../../../holomorphic-function.md) $F:\mathbb D\to\mathbb D$, conjugate by the [automorphisms of the unit disk](../../../../../automorphism-of-the-unit-disk.md) $A_a(z)=(z-a)/(1-\overline a z)$, putting $a$ and $F(a)$ at zero. Applying the proved [Schwarz lemma](../../../../../schwarz-lemma.md) gives

$$
\boxed{\left|\frac{F(z)-F(a)}{1-\overline{F(a)}F(z)}\right|
\leq\left|\frac{z-a}{1-\overline a z}\right|},
\qquad
\boxed{\frac{|F'(a)|}{1-|F(a)|^2}\leq\frac1{1-|a|^2}}.
$$

The disk [hyperbolic metric](../../../../../hyperbolic-metric.md) is $2|dz|/(1-|z|^2)$, and its distance is twice the inverse hyperbolic tangent of the displayed pseudohyperbolic distance. Both forms of [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) therefore express metric contraction. Equality in the derivative at one point makes $F$ a disk automorphism by the equality case already proved.

For $X=\mathbb D\setminus\{0\}$ and a [holomorphic function](../../../../../holomorphic-function.md) $f:X\to Y$, compose with a [universal covering map](../../../../../universal-cover.md) of $X$ and lift to a [universal covering map](../../../../../universal-cover.md) of $Y$. The simply connected source of the lift is a disk or half-plane. [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) there bounds the lifted metric derivative, and the covering maps are local [isometries](../../../../../isometry.md), so

$$
f^*ds_Y\leq ds_X,\qquad
\boxed{d_Y(f(z_0),f(z_1))\leq d_X(z_0,z_1)}.
$$

The second inequality follows by applying the length inequality to every joining path and taking the infimum. The [hyperbolic metric on the punctured disk](../../../../../hyperbolic-metric-on-the-punctured-disk.md) is its own intrinsic metric,

$$
ds_X=\frac{|dz|}{|z|\log(1/|z|)},
$$

obtained from the covering $z=e^{i\tau}$. It is not merely the ordinary disk metric restricted to the punctured disk.

**Yes, equality can occur for distinct points.** The cyclic subgroup $\langle T\rangle$ lies in $\Gamma(2)$. Its quotient is conformally the punctured disk, using $z=e^{\pi i\tau}$, because this identifies precisely $\tau\sim\tau+2$. The subgroup inclusion induces a [covering map](../../../../../covering-space.md) that is a [holomorphic function](../../../../../holomorphic-function.md)

$$
\mathbb D^*\cong\mathbb H/\langle T\rangle
\longrightarrow\mathbb H/\Gamma(2)\cong Y.
$$

It is a local [isometry](../../../../../isometry.md). Choose a sufficiently small geodesically convex ball around any target point that is evenly covered. Two distinct sufficiently close points in one lift of that ball are joined by the lift of its minimizing target [geodesic](../../../../../geodesic.md). The lift has the same length, giving $d_X\leq d_Y$ for this pair, while contraction gives the reverse inequality. Thus equality holds.

For context, if the lifted map is not an automorphism, the derivative inequality is strict at every point; integrating along a minimizing [geodesic](../../../../../geodesic.md) in the complete punctured-disk metric gives a strict distance inequality for every distinct pair. Equality forces the covering-map case, but even a [covering map](../../../../../covering-space.md) need not preserve all distances globally because shorter paths can pass through other sheets. This is the distinction captured by [equality in hyperbolic Schwarz-Pick contraction](../../../../../equality-in-hyperbolic-schwarz-pick-contraction.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
