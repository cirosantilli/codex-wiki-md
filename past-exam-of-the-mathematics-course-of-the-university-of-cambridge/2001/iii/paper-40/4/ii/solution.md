<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take constant [kinematic viscosity](../../../../../../kinematic-viscosity.md) $\nu$ and the inner [specific angular momentum](../../../../../../specific-angular-momentum.md) found above. The [Angular velocity of a circular Schwarzschild geodesic](../../../../../../angular-velocity-of-a-circular-schwarzschild-geodesic.md) gives $-\Omega'=3c\sqrt m/(2r^{5/2})$. Hence the inward radial component of [four-velocity](../../../../../../four-velocity.md) in the stated viscous model is

$$
u=\frac{3\nu/2}{\sqrt r\,[r/\sqrt{r-3m}-\sqrt{12m}]}.
$$

To convert [proper time](../../../../../../proper-time.md) to [Schwarzschild time](../../../../../../schwarzschild-time.md), neglect $\dot r^2$ in the normalization as prescribed and insert the circular value of $h$. One obtains

$$
\frac{dt}{d\tau}\simeq\sqrt{\frac{1+h^2/(c^2r^2)}{1-2m/r}}
=\sqrt{\frac r{r-3m}}.
$$

The change in observed [Schwarzschild time](../../../../../../schwarzschild-time.md) equals this coordinate-time change when differential light travel time is neglected. Since $dr/d\tau=-u$,

$$
\Delta t=\int_{6m}^{r_1}\frac{dt/d\tau}{u}\,dr
=\boxed{\frac2{3\nu}\int_{6m}^{r_1}\left[r-\sqrt{12m(r-3m)}\right]\frac r{r-3m}\,dr.}
$$

This time is nonnegative: $r^2-12m(r-3m)=(r-6m)^2\geq0$ on the integration interval.

Put $x=r/(3m)$ and $X=r_1/(3m)$. The integral becomes

$$
\Delta t=\frac{6m^2}{\nu}\int_2^X\left[\frac{x^2}{x-1}-\frac{2x}{\sqrt{x-1}}\right]dx.
$$

Polynomial division gives $x^2/(x-1)=x+1+1/(x-1)$. Separately, writing $y=x-1$ gives $\int2x/\sqrt{x-1}\,dx=(4/3)(x-1)^{3/2}+4\sqrt{x-1}$. Therefore the antiderivative inside the integral is

$$
\frac{x^2}{2}+x+\log(x-1)-\frac43(x-1)^{3/2}-4\sqrt{x-1}.
$$

Its value at $x=2$ is $-4/3$. Subtracting this lower endpoint yields the [formal viscous inspiral time in Schwarzschild spacetime](../../../../../../formal-viscous-inspiral-time-in-schwarzschild-spacetime.md)

$$
\boxed{\Delta t=\frac{m^2}{\nu}\left[3X^2+6X+6\log(X-1)-8(X-1)^{3/2}-24\sqrt{X-1}+8\right].}
$$

**The logarithm has a positive coefficient.** The minus sign in the printed final expression is inconsistent with its preceding integral. Differentiating the corrected bracket gives $6X[X-2\sqrt{X-1}]/(X-1)$, precisely the positive integrand after rescaling. The bracket vanishes at $X=2$; replacing $+6\log(X-1)$ by its negative would give derivative $-12$ there and a negative elapsed time for $X$ just above $2$. This is a sign error, not a choice of potential or time convention.

The result assumes constant [kinematic viscosity](../../../../../../kinematic-viscosity.md); if $\nu$ varies with radius it remains inside the time integral. There is also a physical limitation to the stipulated approximation: $h-h_0$ vanishes quadratically at $6m$, so its formal $u$ diverges and eventually violates the neglected-radial-motion condition. The finite integral is the formal extrapolation of the nearly circular viscous model. A real [accretion disk](../../../../../../accretion-disk.md) must instead match to its [plunging region of a black-hole accretion disk](../../../../../../plunging-region-of-a-black-hole-accretion-disk.md); this approximation cannot describe that transition arbitrarily closely.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
