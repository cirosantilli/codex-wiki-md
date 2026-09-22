<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\mu=GM/c^2$ and $r_0=R_E+h$. The [Christoffel symbols](../../../../christoffel-symbol.md) follow from

$$
\Gamma^\alpha_{\beta\gamma}=\frac12g^{\alpha\delta}
(\partial_\beta g_{\delta\gamma}+\partial_\gamma g_{\delta\beta}-\partial_\delta g_{\beta\gamma}).
$$

The relevant time and radial entries, using $x^0=ct$, are

$$
\Gamma^r_{00}=\frac12ff'=\frac{\mu f}{r^2},\qquad
\Gamma^0_{0r}=\Gamma^0_{r0}=\frac{f'}{2f}=\frac{\mu}{r^2f},\qquad
\Gamma^r_{rr}=-\frac{\mu}{r^2f},\qquad
\Gamma^0_{00}=\Gamma^\theta_{00}=\Gamma^\phi_{00}=0.
$$

For the angular [geodesic equations](../../../../geodesic-equation.md), $\Gamma^\theta_{r\theta}=\Gamma^\phi_{r\phi}=1/r$, $\Gamma^\theta_{\phi\phi}=-\sin\theta\cos\theta$, and $\Gamma^\phi_{\theta\phi}=\cot\theta$. Thus, with primes on coordinates here denoting [proper time](../../../../proper-time.md) [derivatives](../../../../derivative.md),

$$
\theta''+\frac{2r'}r\theta'-\sin\theta\cos\theta\,(\phi')^2=0,\qquad
\phi''+\frac{2r'}r\phi'+2\cot\theta\,\theta'\phi'=0.
$$

Initial conditions $\theta'=\phi'=0$ are preserved by these [ordinary differential equations](../../../../ordinary-differential-equation.md). The motion is therefore radial, with constant angular coordinates. Choose the polar axis so the apple is away from the angular coordinate singularities.

The exact remaining radial [geodesic equation](../../../../geodesic-equation.md) and [four-velocity](../../../../four-velocity.md) normalization are

$$
r''+\frac{GMf}{r^2}\left(\frac{dt}{d\tau}\right)^2
-\frac{\mu}{r^2f}(r')^2=0,\qquad
fc^2\left(\frac{dt}{d\tau}\right)^2-\frac{(r')^2}{f}=c^2.
$$

Eliminating $dt/d\tau$ gives the particularly simple exact result $r''=-GM/r^2$. The supported observer's [proper time](../../../../proper-time.md) $T$ differs from the apple's [proper time](../../../../proper-time.md) by relative corrections of order $GM/(R_Ec^2)$ and $v^2/c^2$. Consequently, to leading order in the [weak-field approximation](../../../../weak-field-approximation.md) and $h/R_E$, $d^2r/dT^2\simeq-GM/R_E^2=-g$, with $r(0)=r_0$ and zero initial radial [velocity](../../../../velocity.md). Hence

$$
\boxed{r(T)\simeq R_E+h-\frac12gT^2,\qquad g=\frac{GM}{R_E^2},\qquad T_{\rm fall}\simeq\sqrt{\frac{2h}{g}}.}
$$

The proper height measured along a static radial ruler is $\int_{R_E}^r dr/\sqrt f\simeq r-R_E$ at this accuracy. The use of $T$ means the ground clock's elapsed time, with propagation delays corrected; raw visual arrival times include the changing light travel time.

If variation of $g$ over the fall is retained but relativistic corrections are neglected, a useful parametric solution is

$$
r=r_0\cos^2\eta,\qquad
T\simeq\sqrt{\frac{r_0^3}{2GM}}(\eta+\sin\eta\cos\eta),\qquad \eta\ge0.
$$

Its small-$\eta$ expansion gives the same constant-$g$ result. For an exact check on the choice of clock, the initial coordinate [acceleration](../../../../acceleration.md) measured using $T$ is $-GMf(r_0)/[r_0^2f(R_E)]$, which reduces to the displayed approximation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
