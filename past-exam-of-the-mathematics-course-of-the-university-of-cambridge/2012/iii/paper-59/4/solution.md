<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $M=M_1+M_2$ and $\alpha=M_2/M$, with $0<\alpha<1$. In the [centre of mass](../../../../../center-of-mass.md) frame the two primary distances are $r_1=\alpha R$ and $r_2=(1-\alpha)R$. Applying [Newton's law of universal gravitation](../../../../../newton-s-law-of-universal-gravitation.md) and circular [centripetal acceleration](../../../../../centripetal-acceleration.md) to the first primary gives $M_1\omega^2\alpha R=GM_1M_2/R^2$, and hence

$$
\boxed{\omega^2=\frac{GM}{R^3}.}
$$

The same result follows from the second primary or from the relative two-body [equation of motion](../../../../../equation-of-motion.md).

A rotating-frame equilibrium has zero rotating-frame [velocity](../../../../../velocity.md), so its [Coriolis force](../../../../../coriolis-force.md) vanishes. Above the orbital plane both primaries have downward gravitational components; below it both have upward components. The centrifugal [force](../../../../../force.md) has no $z$ component. More explicitly,

$$
a_z=-Gz\left(\frac{M_1}{|\mathbf r-\mathbf r_1|^3}+\frac{M_2}{|\mathbf r-\mathbf r_2|^3}\right),
$$

which vanishes only at $z=0$ for finite nonsingular points. Thus **all equilibria lie in the orbital plane**.

The [equation of motion in a rotating frame](../../../../../equation-of-motion-in-a-rotating-frame.md) for the dwarf is

$$
m\ddot{\mathbf r}=-\nabla U-2m\boldsymbol\omega\mathbin{\times}\dot{\mathbf r}-m\boldsymbol\omega\mathbin{\times}(\boldsymbol\omega\mathbin{\times}\mathbf r),\qquad U=-\frac{GmM_1}{|\mathbf r-\mathbf r_1|}-\frac{GmM_2}{|\mathbf r-\mathbf r_2|}.
$$

On the orbital plane the centrifugal contribution is $m\omega^2\mathbf r$. Thus the [rotating-frame effective potential](../../../../../rotating-frame-effective-potential.md) is $E=U-m\omega^2(x^2+y^2)/2$; equilibria are exactly its stationary points. The [Coriolis force](../../../../../coriolis-force.md) affects motion about those equilibria but not their positions. This is the [circular restricted three-body problem](../../../../../circular-restricted-three-body-problem.md), with the dwarf treated as a test [mass](../../../../../mass.md).

**The printed energy unit has the wrong dimensions.** The correct total [energy](../../../../../energy.md) unit is $mGM/R$, or $GM/R$ for specific [energy](../../../../../energy.md); $GM/R^2$ is an [acceleration](../../../../../acceleration.md). Dividing $E$ by $mGM/R$ and measuring lengths in units of $R$ gives the dimensionless [effective potential](../../../../../effective-potential.md)

$$
\mathcal E(x,y)=-\frac{x^2+y^2}{2}-\frac{1-\alpha}{\sqrt{(x+\alpha)^2+y^2}}-\frac{\alpha}{\sqrt{(x-1+\alpha)^2+y^2}}.
$$

The primary coordinates are $(-\alpha,0)$ and $(1-\alpha,0)$. Restricting to $y=0$ gives $F(x)=\mathcal E(x,0)$ and

$$
F'(x)=-x+\frac{(1-\alpha)(x+\alpha)}{|x+\alpha|^3}+\frac{\alpha(x-1+\alpha)}{|x-1+\alpha|^3},\qquad F''(x)=-1-\frac{2(1-\alpha)}{|x+\alpha|^3}-\frac{2\alpha}{|x-1+\alpha|^3}<0.
$$

The absolute values are essential; dropping them would reverse the attraction on the left of a primary. On each of the intervals separated by the two primaries, $F'$ decreases strictly from $+\infty$ to $-\infty$. There is exactly one [Collinear Lagrange point](../../../../../collinear-lagrange-point.md) on each interval, a maximum along the $x$ direction.

For the [inner Lagrange point](../../../../../inner-lagrange-point.md), write $x=1-\alpha-\delta$ with $\delta>0$. For the [L2 Lagrange point](../../../../../l2-lagrange-point.md), write $x=1-\alpha+\delta$. The respective equations are

$$
0=-(1-\alpha-\delta)+\frac{1-\alpha}{(1-\delta)^2}-\frac{\alpha}{\delta^2}=3\delta-\frac{\alpha}{\delta^2}+O(\delta^2+\alpha\delta),
$$



$$
0=-(1-\alpha+\delta)+\frac{1-\alpha}{(1+\delta)^2}+\frac{\alpha}{\delta^2}=-3\delta+\frac{\alpha}{\delta^2}+O(\delta^2+\alpha\delta).
$$

Balancing the leading terms gives $\delta=(\alpha/3)^{1/3}+O(\alpha^{2/3})$. Therefore the [small-mass-ratio collinear Lagrange points](../../../../../small-mass-ratio-collinear-lagrange-points.md) obey

$$
\boxed{x_{L_1}=1-(\alpha/3)^{1/3}+O(\alpha^{2/3}),\qquad x_{L_2}=1+(\alpha/3)^{1/3}+O(\alpha^{2/3}).}
$$

The omitted $-\alpha$ displacement of the secondary is smaller than the stated error. The leading distance from the secondary is the dimensionless [Hill radius](../../../../../hill-radius.md).

For the [L3 Lagrange point](../../../../../l3-lagrange-point.md) put $x=-1+c\alpha+O(\alpha^2)$. It lies to the left of both primaries, so

$$
F'=-x-\frac{1-\alpha}{(x+\alpha)^2}-\frac{\alpha}{(x-1+\alpha)^2}.
$$

Expanding the two positive inverse-square factors gives $(1-\alpha)/(x+\alpha)^2=1+(2c+1)\alpha+O(\alpha^2)$ and $\alpha/(x-1+\alpha)^2=\alpha/4+O(\alpha^2)$. Thus $F'=-(3c+5/4)\alpha+O(\alpha^2)$, so

$$
\boxed{x_{L_3}=-1-\frac5{12}\alpha+O(\alpha^2).}
$$

All three have $y=z=0$. The small-$\alpha$ equalities in the paper are asymptotic expressions, not exact coordinates for finite mass ratio.

For the remaining [Lagrange points](../../../../../lagrange-point.md), introduce plane [polar coordinates](../../../../../polar-coordinates.md) about the first primary: $x=-\alpha+s\cos\theta$, $y=s\sin\theta$. Its distance to the second primary is $d=(s^2+1-2s\cos\theta)^{1/2}$, and

$$
\mathcal E=-\frac12(s^2-2\alpha s\cos\theta+\alpha^2)-\frac{1-\alpha}{s}-\frac\alpha d.
$$

The angular stationary condition is $\partial_\theta\mathcal E=\alpha s\sin\theta(d^{-3}-1)=0$. For an off-axis point $s>0$ and $\sin\theta\ne0$, so $d=1$. The radial stationary condition becomes

$$
\partial_s\mathcal E=-s+\alpha\cos\theta+\frac{1-\alpha}{s^2}+\frac{\alpha(s-\cos\theta)}{d^3}=(1-\alpha)(s^{-2}-s)=0.
$$

Hence $s=1$, and $d=1$ implies $\cos\theta=1/2$. The [Triangular Lagrange points](../../../../../triangular-lagrange-point.md) are exactly

$$
\boxed{L_4=(\tfrac12-\alpha,\tfrac{\sqrt3}{2},0),\qquad L_5=(\tfrac12-\alpha,-\tfrac{\sqrt3}{2},0).}
$$

Both triangles are equilateral. The collinear and off-axis calculations together exhaust the stationary points.

For the requested sketch, $\mathcal E$ tends to $-\infty$ at either primary and at large in-plane radius. Each [Collinear Lagrange point](../../../../../collinear-lagrange-point.md) is a saddle of the planar [effective potential](../../../../../effective-potential.md): its $x$ curvature is negative and its $y$ curvature is positive. To see the latter, let $d_1=|x+\alpha|$, $d_2=|x-1+\alpha|$ and $D=(1-\alpha)/d_1^3+\alpha/d_2^3$. At an inner point both distances are below one, so $D>1$. At an exterior stationary point, use barycentric positions $a_1=-\alpha$, $a_2=1-\alpha$ and weights $1-\alpha,\alpha$: the equation implies $x(D-1)=\sum w_i a_i/|x-a_i|^3$. To the right, the weighted sum is positive because the positive primary is closer; to the left it is negative because the negative primary is closer. Thus $D>1$ there as well, and $\mathcal E_{yy}=D-1>0$.

At either [Triangular Lagrange point](../../../../../triangular-lagrange-point.md), the planar [Hessian](../../../../../hessian-matrix.md) is

$$
D^2\mathcal E=-3\begin{pmatrix}1/4&\pm\sqrt3(1-2\alpha)/4\\\pm\sqrt3(1-2\alpha)/4&3/4\end{pmatrix}.
$$

Its trace is $-3$ and determinant $27\alpha(1-\alpha)/4>0$, so these are local maxima. Their height is $\mathcal E=-3/2+\alpha(1-\alpha)/2$. The sketch below uses a finite mass ratio to separate the five points clearly; its singular wells are clipped only for display. These curvature labels concern the [effective potential](../../../../../effective-potential.md), not a stability test that ignores the [Coriolis force](../../../../../coriolis-force.md).

<a id="4/image-rotating-binary-effective-potential-surface-and-contours-at-mass-fraction-0-10-with-all-five-lagrange-points-marked"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-59-effective-potential.png)

**[Figure 2](#4/image-rotating-binary-effective-potential-surface-and-contours-at-mass-fraction-0-10-with-all-five-lagrange-points-marked). Rotating binary effective-potential surface and contours at mass fraction 0.10, with all five Lagrange points marked**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
