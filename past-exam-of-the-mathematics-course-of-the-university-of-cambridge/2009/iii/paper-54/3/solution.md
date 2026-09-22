<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $f(r)=1-2M/r$, with $M>0$, and let a dot denote differentiation with respect to an [affine parameter](../../../../../affine-parameter.md) $\lambda$. The [geodesic Lagrangian](../../../../../geodesic-lagrangian.md) is one half the squared tangent norm. Its Euler–Lagrange equations give

$$
\frac{d}{d\lambda}(f\dot t)=0,\qquad
\frac{d}{d\lambda}(r^2\sin^2\theta\,\dot\phi)=0,
$$



$$
\ddot\theta+\frac{2\dot r}{r}\dot\theta-\sin\theta\cos\theta\,\dot\phi^2=0,
$$



$$
\ddot r+\frac{ff'}2\dot t^2-\frac{f'}{2f}\dot r^2-fr\bigl(\dot\theta^2+\sin^2\theta\,\dot\phi^2\bigr)=0,
$$

where $f'=df/dr$ in these formulas only. The constants from time translation and axial rotation are

$$
E=f\dot t,\qquad L_z=r^2\sin^2\theta\,\dot\phi.
$$

They are the [Killing energy](../../../../../killing-energy.md) and axial [angular momentum](../../../../../angular-momentum.md) per chosen affine normalization. A rescaling of $\lambda$ rescales both, while their ratio is invariant. More generally the rotational Killing fields conserve the full angular-momentum vector: differentiating any Killing contraction along an affine [geodesic](../../../../../geodesic.md) gives $k^ak^b\nabla_{(a}\xi_{b)}=0$. Thus its direction can be chosen as the polar axis.

Equivalently rotate the initial position and angular tangent into one plane through the centre. The angular [geodesic equation](../../../../../geodesic-equation.md) then has initial data $\theta=\pi/2$, $\dot\theta=0$, for which $\theta=\pi/2$ solves the equation identically. Uniqueness keeps the [geodesic](../../../../../geodesic.md) in that plane. A radial [geodesic](../../../../../geodesic.md) has no distinguished orbital plane but can be placed in any equatorial plane. Hence no physical restriction is imposed by setting $\theta=\pi/2$.

Write $L=L_z$ in that plane. For a [null geodesic](../../../../../null-geodesic.md) the tangent norm vanishes, giving

$$
\boxed{\dot t=E/f,\qquad \dot\phi=L/r^2,\qquad
\dot r^2=E^2-\frac{L^2}{r^2}\left(1-\frac{2M}{r}\right).}
$$

The full radial equation also gives $\ddot r=L^2(r-3M)/r^4$. These equations are used away from the coordinate singularity $r=2M$; the [geodesics](../../../../../geodesic.md) themselves extend across the horizon in regular coordinates. For radial rays $L=0$, $\dot r=\pm E$ and azimuth is not an orbit parameter.

For the nonradial case $L\ne0$, set $u=M/r$ and now use a prime for $d/d\phi$. Since $u'=-M\dot r/L$, the null first integral becomes

$$
\boxed{(u')^2=\alpha^2-u^2+2u^3,\qquad \alpha=\frac{ME}{L}=\frac M b,\quad b=\frac L E.}
$$

Here $b$ is the signed [impact parameter](../../../../../impact-parameter.md); its magnitude is the ordinary positive impact parameter for an exterior future-directed ray. The second-order orbit equation is $u''+u=3u^2$. It follows from the radial [geodesic equation](../../../../../geodesic-equation.md) and therefore holds even where $u'=0$; differentiation of the squared first integral alone would not establish a circular solution at a turning point.

A finite circular photon orbit has $u'=u''=0$ and nonzero $u$. Hence $u=1/3$, while the first integral fixes $\alpha^2=1/27$:

$$
\boxed{r=3M,\qquad |b|=3\sqrt3M.}
$$

The null radial potential $L^2f/r^2$ has second derivative $-2L^2/(81M^4)$ there, so the [photon sphere](../../../../../photon-sphere.md) is unstable. The formal root $u=0$ lies at infinite radius, not a finite orbit. Radial null generators of the event horizon have fixed angles and are not circular photon orbits.

At the critical impact parameter the first integral factors as

$$
(u')^2=\left(u-\frac13\right)^2\left(2u+\frac13\right).
$$

Choose the oriented branch $u'=(u-1/3)\sqrt{1+6u}/\sqrt3$. Put $w=\sqrt{1+6u}$; then $w'=(w^2-3)/(2\sqrt3)$. The function

$$
Q(u)=\frac{1-3u}{(\sqrt3+\sqrt{1+6u})^2}
=\frac{\sqrt3-w}{2(\sqrt3+w)}
$$

satisfies $dQ/d\phi=Q$ by direct differentiation. Integrating gives

$$
\boxed{\frac{1-3u}{(\sqrt3+\sqrt{1+6u})^2}=Ae^\phi.}
$$

This establishes the displayed family as actual critical-impact-parameter [geodesics](../../../../../geodesic.md). Reversing the azimuthal orientation gives the complementary $Ae^{-\phi}$ parametrization.

To expose the geometry, put $x=Ae^\phi$. Solving for the positive square root gives

$$
\sqrt{1+6u}=\sqrt3\frac{1-2x}{1+2x},\qquad
u=\frac13-\frac{4x}{(1+2x)^2}.
$$

For physical $r>0$ this branch uses $-1/2<x<(2-\sqrt3)/2$, with the upper endpoint corresponding to infinite radius. As $\phi\to-\infty$,

$$
u=\frac13-4Ae^\phi+O(e^{2\phi}),\qquad
r=3M+36MAe^\phi+O(e^{2\phi}).
$$

Thus the [critical photon orbits of Schwarzschild spacetime](../../../../../critical-photon-orbits-of-schwarzschild-spacetime.md) wind around the photon circle infinitely many times with an exponentially shrinking radial displacement. **For $A>0$ the approach is from outside $r=3M$; for $A<0$ it is from inside; for $A=0$ the orbit is the circle itself.** Increasing $\phi$ along the chosen orientation sends the positive branch outward toward infinity and the negative branch inward, through the horizon toward the singularity. The limiting description at $\phi\to-\infty$ concerns the asymptotic photon sphere rather than a finite-angle radial turning point.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
