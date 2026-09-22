<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the constant in the integrated [Reynolds equation](../../../../reynolds-equation.md) be $C$:

$$
\frac{H^3}{12}\frac{dp'}{dx'}+\frac H2=C,
\qquad \frac{dp'}{dx'}=12C H^{-3}-6H^{-2},
\qquad H=1+\frac{x'^2}{2}.
$$

Both endpoint [pressures](../../../../pressure-split.md) are zero, so the [integral](../../../../integral-split.md) of $dp'/dx'$ on the real line vanishes. Define

$$
I_m=\int_{-\infty}^{\infty}\frac{dx'}{(1+x'^2/2)^m}.
$$

The substitution $x'=\sqrt2\tan\theta$ gives

$$
I_m=\sqrt2\int_{-\pi/2}^{\pi/2}\cos^{2m-2}\theta\,d\theta,
\qquad I_2=\frac{\pi}{\sqrt2},\qquad
I_3=\frac{3\pi\sqrt2}{8}.
$$

The second value follows by integrating the supplied identity for $\cos^4\theta$; the nonconstant cosine terms have zero [integral](../../../../integral-split.md) over this interval. Hence $12CI_3-6I_2=0$, giving

$$
\boxed{C=\frac{I_2}{2I_3}=\frac23,\qquad q=-C=-\frac23.}
$$

The [pressure gradient](../../../../pressure-gradient.md) is now

$$
\frac{dp'}{dx'}=\frac{8-6H}{H^3}
=\frac{2-3x'^2}{(1+x'^2/2)^3}.
$$

Direct differentiation shows

$$
\frac d{dx'}\left(\frac{2x'}{H^2}\right)
=\frac2{H^2}-\frac{4x'^2}{H^3}
=\frac{2-3x'^2}{H^3}.
$$

The candidate tends to zero at both ends, so the additive constant is zero and

$$
\boxed{p'(x')=\frac{2x'}{(1+x'^2/2)^2}.}
$$

Together with the local [Couette-Poiseuille flow](../../../../couette-poiseuille-flow.md) profile, this solves the [sliding-plate flow through a parabolic gap](../../../../sliding-plate-flow-through-a-parabolic-gap.md).

To restore dimensions, integrate $u=Uu'$ across $dz=h_0\,dz'$. The signed dimensional [volume flux per unit width](../../../../volume-flux-per-unit-width.md), positive in the $+x$ direction, is

$$
\boxed{Q=Uh_0q=-\frac23Uh_0.}
$$

Thus the magnitude drawn in the direction of the moving plate is $2Uh_0/3$. For a plate width $B$ large enough to neglect side-wall effects, the total [volumetric flow rate](../../../../volumetric-flow-rate.md) is $-2BUh_0/3$; without a specified width the answer is per unit width.

The [Couette flow](../../../../couette-flow.md) and [plane Poiseuille flow](../../../../plane-poiseuille-flow.md) contributions to the dimensional [volume flux per unit width](../../../../volume-flux-per-unit-width.md) are respectively

$$
Q_C=-\frac{Uh(x)}2<0,\qquad
Q_P=-\frac{h(x)^3}{12\mu}\frac{dp}{dx}
=Uh_0\left(\frac H2-\frac23\right)
=Uh_0\left(\frac{x'^2}{4}-\frac16\right).
$$

They point in the same direction precisely when $Q_P<0$, giving

$$
\boxed{-\sqrt{\frac{2Rh_0}{3}}<x<\sqrt{\frac{2Rh_0}{3}}.}
$$

At the endpoints the [plane Poiseuille flow](../../../../plane-poiseuille-flow.md) contribution is zero. Outside that interval it opposes the [Couette flow](../../../../couette-flow.md) contribution, while their sum remains the constant negative [volume flux per unit width](../../../../volume-flux-per-unit-width.md) $-2Uh_0/3$. Thus **pressure assists the moving plate near the narrowest gap** and drives a compensating return contribution farther away.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the viscous flow course of the University of Oxford](../../../split.md)
5. [Viscous flow course of the University of Oxford](../../../../viscous-flow-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
