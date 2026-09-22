<h1 id="b/8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $f=1-2m/r$, use [proper time](../../../../../proper-time.md) $s$, and denote its [derivatives](../../../../../derivative.md) by dots. The [timelike geodesic](../../../../../timelike-geodesic.md) equations, away from the Schwarzschild coordinate singularity, are

$$
\boxed{\begin{aligned}
\ddot t+\frac{f'}f\dot r\dot t&=0,\\
\ddot r+\frac{ff'}2\dot t^2-\frac{f'}{2f}\dot r^2-rf(\dot\theta^2+\sin^2\theta\dot\phi^2)&=0,\\
\ddot\theta+\frac{2\dot r}r\dot\theta-\sin\theta\cos\theta\dot\phi^2&=0,\\
\ddot\phi+\frac{2\dot r}r\dot\phi+2\cot\theta\dot\theta\dot\phi&=0,
\end{aligned}}
$$

with [normalization](../../../../../normalization.md) $f\dot t^2-f^{-1}\dot r^2-r^2\dot\theta^2-r^2\sin^2\theta\dot\phi^2=1$. [Spherical symmetry](../../../../../spherical-symmetry.md) permits an [equatorial plane](../../../../../equatorial-plane.md), $\theta=\pi/2$, and the cyclic coordinates give $\boxed{E=f\dot t,\quad J=r^2\dot\phi}$. [Normalization](../../../../../normalization.md) then gives $\dot r^2=E^2-f(1+J^2/r^2)$.

For $J\ne0$ and $u=m/r$, $du/d\phi=-m\dot r/J$. Thus

$$
\boxed{(u')^2=\frac{(E^2-1)m^2}{J^2}+\frac{2m^2}{J^2}u-u^2+2u^3.}
$$

At $E=1$, $J=4m$, the right side factors as $2u(u-1/4)^2$. Set $q=2\sqrt u$, so $u=q^2/4$ and $(q')^2=(q^2-1)^2/8$. Integrating the regions $0<q<1$ and $q>1$ gives, up to angular shifts and time reversal,

$$
\boxed{u=\tfrac14\tanh^2\!\left(\frac{\phi-\phi_0}{2\sqrt2}\right),\qquad
u=\tfrac14\coth^2\!\left(\frac{\phi-\phi_0}{2\sqrt2}\right).}
$$

The constant $u=1/4$, or $r=4m$, is the corresponding circular timelike orbit. The hyperbolic-tangent branch lies at $r>4m$ and approaches that orbit from outside as $|\phi|\to\infty$; the hyperbolic-cotangent branch lies at $0<r<4m$ and approaches it from inside. Near the limit $u-1/4$ decays exponentially as $e^{-|\phi|/\sqrt2}$. Since $\dot\phi$ tends to $J/(4m)^2=1/(4m)$, the limiting approach also takes infinite [proper time](../../../../../proper-time.md). Neither nonconstant branch reaches and joins the [circular orbit](../../../../../circular-orbit.md) at a finite angular parameter.

Differentiating the orbit equation gives $u''=m^2/J^2-u+3u^2$. A perturbation about $u=1/4$ obeys $\delta u''=\delta u/2$, showing that the [circular orbit](../../../../../circular-orbit.md) is unstable. The two explicit curves are its [separatrix](../../../../../separatrix.md) branches, not ordinary small stable oscillations. For $E=1$ the energy is marginally bound, so the outer critical branch is the limiting orbit between [scattering](../../../../../scattering.md) and [Schwarzschild marginally bound capture](../../../../../schwarzschild-marginally-bound-capture.md) from infinity. Time-reversed inner and outer branches describe the corresponding approach or departure from that unstable orbit. These are the [Explicit separatrices of the marginally bound Schwarzschild orbit](../../../../../explicit-separatrices-of-the-marginally-bound-schwarzschild-orbit.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the mathematical physics course of the University of Oxford](../../../../split.md)
6. [Mathematical physics course of the University of Oxford](../../../../../mathematical-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
