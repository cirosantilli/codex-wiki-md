<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Landau description.** Introduce a macroscopic [order parameter](../../../../order-parameter.md) and expand an appropriate [free energy](../../../../thermodynamic-free-energy.md) analytically in that parameter, retaining terms permitted by the physical symmetries. Stable equilibrium minimizes this [free energy](../../../../thermodynamic-free-energy.md) globally; a [local minimum](../../../../local-minimum.md) with larger [free energy](../../../../thermodynamic-free-energy.md) is metastable. Coefficient changes with [temperature](../../../../temperature-split.md) can exchange the preferred minima. A continuous emergence from zero can produce a continuous transition, while competing separated minima can produce a first-order transition. Stability requires a positive highest retained even-power term. This local mean-field description neglects spatial fluctuations and [nucleation](../../../../nucleation.md) dynamics unless gradient and dynamical terms are added; near a [critical point](../../../../critical-point.md) those omissions can matter.

For this [temperature-dependent cubic-quartic Landau free energy](../../../../temperature-dependent-cubic-quartic-landau-free-energy.md), abbreviate $B=a/(12\pi)>0$ and $A(T)=c(T^2-T_0^2)$, so $F=A\phi^2/2-BT\phi^3+\lambda\phi^4/4$ and $\gamma=2B^2/(\lambda c)$.

**Local behavior at the origin.** To determine [constrained order-parameter boundary stability](../../../../constrained-order-parameter-boundary-stability.md), note that $F'(0)=0$ and $F''(0)=c(T^2-T_0^2)$, the origin is a [local minimum](../../../../local-minimum.md) for $T>T_0$ and a [local maximum](../../../../local-maximum.md) for $0\leq T<T_0$. At $T=T_0$, the quadratic term vanishes, but $F=-BT_0\phi^3+O(\phi^4)<0$ for small positive $\phi$. Therefore

$$
\boxed{\phi=0\text{ is locally stable for }T>T_0,\quad
\text{a one-sided <local maximum> for }0\leq T\leq T_0.}
$$

The equality case uses the stipulated domain $\phi\geq0$. On an unrestricted real line, the nonzero cubic term would instead make it a stationary inflection point.

**Global stability in both inline cases.** For $\phi>0$, complete the square in $F/\phi^2$:

$$
\frac{F}{\phi^2}
=\frac{\lambda}{4}\left(\phi-\frac{2BT}{\lambda}\right)^2
+\frac c2\left[(1-\gamma)T^2-T_0^2\right].
$$

The quartic coefficient guarantees a bounded [global minimum](../../../../global-minimum.md). A negative value exists precisely when the minimum of this quadratic factor is negative. Hence case a, $\gamma>1$, has a nonzero globally stable phase with $F<0$ for every physical [temperature](../../../../temperature-split.md). Case b, $0<\gamma<1$, has such a phase exactly for

$$
\boxed{T<T^*=\frac{T_0}{\sqrt{1-\gamma}}}.
$$

At $T=0$, the square's centre is at the boundary, but its negative constant still gives $F<0$ for small positive $\phi$, so this endpoint is included.

At $T=T^*$,

$$
F(\phi,T^*)=\frac{\lambda}{4}\phi^2(\phi-\phi^*)^2,\qquad
\boxed{\phi^*=\frac{2BT^*}{\lambda}=\frac{aT^*}{6\pi\lambda}}.
$$

The two global minima $\phi=0,\phi^*$ have equal [free energy](../../../../thermodynamic-free-energy.md), and $F''(\phi^*)=\lambda(\phi^*)^2/2>0$. The [coexistence barrier of a cubic-quartic Landau transition](../../../../coexistence-barrier-of-a-cubic-quartic-landau-transition.md) has its maximum at $\phi^*/2$, with barrier height $\lambda(\phi^*)^4/64$.

For locating the extrema away from coexistence,

$$
\phi_\pm(T)=\frac{3BT\pm\sqrt{9B^2T^2-4\lambda c(T^2-T_0^2)}}{2\lambda}.
$$

Retain only real positive roots; when both are positive, $\phi_-$ is a [local maximum](../../../../local-maximum.md) and $\phi_+$ a [local minimum](../../../../local-minimum.md). For $T<T_0$, only $\phi_+$ is positive. If $\gamma<8/9$, the pair first appears on cooling at $T_{\rm sp}=T_0/\sqrt{1-9\gamma/8}>T^*$; if $8/9\leq\gamma<1$, a higher-free-energy nonzero minimum already exists at arbitrarily high [temperature](../../../../temperature-split.md). These local-stability limits must not be mistaken for the global coexistence condition. The boundary $\gamma=1$ also favors a nonzero minimum at every finite [temperature](../../../../temperature-split.md), but has no finite $T^*$.

<a id="4/image-original-cubic-quartic-free-energy-curves-above-at-and-below-the-relevant-stability-regimes"></a>
![](../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1-landau-potentials.png)

**[Figure 3](#4/image-original-cubic-quartic-free-energy-curves-above-at-and-below-the-relevant-stability-regimes). Original cubic-quartic free-energy curves above, at and below the relevant stability regimes**.

**Cooling and transition [temperature](../../../../temperature-split.md).** For $\gamma<1$, equilibrium starts at the zero minimum at high [temperature](../../../../temperature-split.md) and switches to the nonzero minimum at $T^*$. The jump is finite, $0\to\phi^*>0$, and there is a barrier between the coexisting states. This is a first-order transition. The [latent heat of a temperature-dependent cubic-quartic Landau transition](../../../../latent-heat-of-a-temperature-dependent-cubic-quartic-landau-transition.md) follows from differentiating the minimized [free energy](../../../../thermodynamic-free-energy.md): the heat released on cooling is

$$
L=T^*(S_0-S_+)
=c(1-\gamma)(T^*)^2(\phi^*)^2
=cT_0^2(\phi^*)^2>0.
$$

If $F$ is an [energy](../../../../energy-split.md) density rather than total [energy](../../../../energy-split.md), $L$ is likewise a density. An actual system can supercool below $T^*$ before [nucleation](../../../../nucleation.md), so $T^*$ is the equilibrium transition [temperature](../../../../temperature-split.md).

For [thermal symmetry nonrestoration in a cubic-quartic model](../../../../thermal-symmetry-nonrestoration-in-a-cubic-quartic-model.md), with $\gamma>1$, the equilibrium [global minimum](../../../../global-minimum.md) is nonzero already at arbitrarily high [temperature](../../../../temperature-split.md). Following it does not force a transition. A system initially prepared in the [metastable](../../../../metastability.md) zero minimum can still leave it by [nucleation](../../../../nucleation.md) while $T>T_0$; that minimum loses local stability at $T_0$. This is the sense in which a change is possible rather than inevitable. **There is no equilibrium coexistence temperature for $\gamma>1$ in this model.** A kinetic transition can depend on preparation and [nucleation](../../../../nucleation.md) dynamics; $T_0$ is the limiting loss of local stability of the zero state, not a second coexistence temperature. Continuing $T^*$ to an imaginary value does not define a physical transition [temperature](../../../../temperature-split.md).

**Mass window in the specified [electroweak phase transition](../../../../electroweak-phase-transition.md) model.** For the [mass window in a cubic electroweak transition model](../../../../mass-window-in-a-cubic-electroweak-transition-model.md), put $x=m_H^2/m_0^2>0$. The supplied ratios imply

$$
\gamma=\frac1{72\pi^2x(A+x)},\qquad
\frac{\phi^*}{T^*}=\frac1{6\pi x}.
$$

The two strict conditions therefore require

$$
x(A+x)>\frac1{72\pi^2},
\qquad
x<\frac1{6\pi}.
$$

Since $x(A+x)$ is increasing for $x>0$, the finite window is

$$
\boxed{\frac{-A+\sqrt{A^2+1/(18\pi^2)}}2
<x<\frac1{6\pi}}.
$$

Using the specified $A$ and $m_0$ gives

$$
0.00147900<x<0.05305165,\qquad
\boxed{8.61\ \mathrm u<m_H<51.57\ \mathrm u}.
$$

At $m_H=134$ u, $x=0.3581801$, $\gamma\simeq0.0030033<1$ but $\phi^*/T^*\simeq0.1481<1$. Thus **134 u lies outside the required window**, failing the order-parameter-strength condition. This does not remove the [polynomial](../../../../polynomial-split.md) model's finite first-order jump; it fails the additional requirement $\phi^*>T^*$. The result is a bound within the specified simplified model, not a model-independent Higgs-mass bound.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
