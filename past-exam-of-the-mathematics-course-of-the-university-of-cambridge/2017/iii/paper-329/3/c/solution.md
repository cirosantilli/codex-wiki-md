<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put the fixed outer centre at the origin, and let the moving inner centre be $\mathbf d=(x,z)$. This reverses the sign of the vertical offset used in the previous parts: now $h=\Delta-\mathbf d\cdot\mathbf n$. At concentricity rotation produces no [force](../../../../../../force.md) and translation has isotropic resistance $R_0=12\pi\mu a^3/\Delta^3$. Balancing the external load gives

$$
\boxed{\dot x(0)=0,\qquad \dot z(0)=-\frac{F\Delta^3}{12\pi\mu a^3}.}
$$

There is no inertial acceleration in this [Stokes flow](../../../../../../stokes-flow-split.md) model; [velocity](../../../../../../velocity.md) is determined instantaneously by [force](../../../../../../force.md) balance.

For the subsequent motion, the [full-film journal bearing](../../../../../../full-film-journal-bearing.md) assumption matters: [pressure](../../../../../../pressure.md) is single-valued around the whole annulus, with no specified [cavitation](../../../../../../cavitation.md) boundary. Let $r=|\mathbf d|$, $e=r/\Delta$, $\phi=\arg(x+iz)$, and $\mathbf e_r,\mathbf e_\phi$ be its radial and tangential unit [vectors](../../../../../../vector.md). The [squeeze resistance of an eccentric journal bearing](../../../../../../squeeze-resistance-of-an-eccentric-journal-bearing.md) has radial and tangential coefficients

$$
R_r=\frac{R_0}{(1-e^2)^{3/2}},\qquad
R_t=\frac{R_0}{\sqrt{1-e^2}(1+e^2/2)}.
$$

For completeness, rotate coordinates until $\mathbf d$ points along $x$, so $h=\Delta(1-e\cos\theta)$. Radial translation gives squeezing flux $q=av_r\sin\theta$ and resistance proportional to $\int\sin^2\theta/(1-e\cos\theta)^3=\pi/(1-e^2)^{3/2}$. Tangential translation gives $q=av_t[-\cos\theta+3e/(2+e^2)]$; the constant enforces periodic [pressure](../../../../../../pressure.md). Its resistance uses

$$
\int\frac{\cos^2\theta}{(1-e\cos\theta)^3}d\theta
-\frac{\left[\int\cos\theta/(1-e\cos\theta)^3d\theta\right]^2}{I_3}
=\frac{\pi}{\sqrt{1-e^2}(1+e^2/2)}.
$$

These expressions supply both translation directions; retaining only the vertical squeezing formula would miss the moving axle's horizontal dynamics.

The rotational fluid [force](../../../../../../force.md) from the earlier calculation points along $\mathbf e_\phi$, with magnitude $R_t\Omega r/2$. Superposing rotation and translation by [Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md), and resolving the load, gives

$$
\boxed{R_r\dot r=-F\sin\phi,\qquad
R_t r\left(\dot\phi-\frac\Omega2\right)=-F\cos\phi.}
$$

For positive $\Omega$ the axle initially moves down, then to the right because the rotation-generated [force](../../../../../../force.md) is perpendicular to the downward eccentricity. The equilibrium is displaced horizontally to the right, at the same height as the outer axis. Its eccentricity $0<e_*<1$ is the unique solution

$$
\boxed{x_* =\Delta e_*,\quad z_*=0,\qquad
F=\frac{6\pi\mu\Omega a^3}{\Delta^2}\frac{e_*}{\sqrt{1-e_*^2}(1+e_*^2/2)}.}
$$

The rotational [force](../../../../../../force.md) then points upwards and balances the load. For negative $\Omega$ the displacement is to the left, using $|\Omega|$ in the magnitude equation. Uniqueness follows because the logarithmic derivative of $e/[\sqrt{1-e^2}(1+e^2/2)]$ has positive numerator $1-e^2/2+e^4$ after a common positive denominator. If $\Omega=0$ and $F>0$, no separated static equilibrium exists in this ideal model. If $F=0$, concentricity remains a solution.

One should not assert that this full-film model necessarily settles to the equilibrium. It predicts [full-film journal-bearing whirl](../../../../../../full-film-journal-bearing-whirl.md). For $F,\Omega>0$, eliminate time from the two boxed evolution equations and put $K=6\pi\mu\Omega a^3/\Delta^2$. The orbit starting at concentricity obeys

$$
\frac d{de}x+\frac{3e}{2(1-e^2)}x=\frac{\Omega\Delta^2R_0}{2F}\frac e{(1-e^2)^{3/2}},
$$

so, with its zero initial horizontal displacement,

$$
\boxed{\frac x\Delta=\frac{2K}{5F}\left[(1-e^2)^{-1/2}-(1-e^2)^{3/4}\right],\qquad
z=\pm\Delta\sqrt{e^2-(x/\Delta)^2}.}
$$

The orbit begins on the lower branch, turns at $z=0$ before contact, and returns along the upper branch, forming a closed orbit through concentricity. The ratio of the right-hand side to $e$ increases from zero to infinity, giving a unique turning eccentricity below one. Linearizing at equilibrium likewise gives $\delta\dot r=-(F/R_{r,*})\delta\phi$ and $\delta\dot\phi=c_*\delta r$ with $c_*>0$: the [eigenvalues](../../../../../../eigenvalue.md) are imaginary, not damped. Thus the equilibrium position exists, but the initially concentric axle circulates around it in the stated ideal full-film approximation. [Cavitation](../../../../../../cavitation.md) or additional mechanical constraints would change the model; none were specified.

The normalized centre trajectory below illustrates the full-film prediction for $K/F=1$. The dashed circle is the contact locus of the axle centre, not either cylinder wall.

<a id="3/c/image-journal-bearing-geometry-and-whirl"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-329-bearing-whirl.png)

**[Figure 1](#3/c/image-journal-bearing-geometry-and-whirl). Journal-bearing geometry and whirl**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
