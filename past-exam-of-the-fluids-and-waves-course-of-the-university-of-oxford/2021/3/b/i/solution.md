<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The denominator of the travelling response vanishes at

$$
\boxed{c^*=\sqrt{g\tanh h}}.
$$

For the positive speeds in the paper, a finite travelling response exists whenever $c\ne c^*$. At $c=c^*$, the dynamic condition would reduce to $p_1/\rho=0$, which is impossible. The finite-depth [dispersion relation](../../../../../dispersion-relation-split.md) of a [surface gravity wave](../../../../../surface-gravity-wave.md) with [wavenumber](../../../../../wavenumber.md) $k$ is $\omega^2=gk\tanh(kh)$. At $k=1$, its [phase speed](../../../../../phase-speed.md) $\omega/k$ equals $c^*$: the moving [pressure](../../../../../pressure-split.md) pattern drives a natural [surface gravity wave](../../../../../surface-gravity-wave.md) at its own speed, producing [resonance](../../../../../resonance.md).

The restriction concerns a bounded travelling response. To distinguish this from existence of a solution of an [initial value problem](../../../../../initial-value-problem.md), set $T=\tanh h$, $P=p_1/\rho$, and $\omega_*^2=gT$. If

$$
\eta(x,t)=\operatorname{Re}(H(t)e^{ix}),\qquad
\phi(x,y,t)=\operatorname{Re}\!\left(
\frac{\dot H(t)}{\sinh h}\cosh(y+h)e^{ix}\right),
$$

the [linearized free-surface boundary conditions](../../../../../linearized-free-surface-boundary-conditions.md) reduce to the [forced harmonic oscillator](../../../../../forced-harmonic-oscillator.md)

$$
\boxed{\ddot H+\omega_*^2H=-PT\,e^{-ict}}.
$$

For example, if the forcing is switched on at $t=0$ from a flat surface with zero initial [velocity](../../../../../velocity.md), then, for $c\ne\omega_*$,

$$
H(t)=\frac{PT}{\omega_*^2-c^2}
\left[\cos(\omega_*t)-i\frac c{\omega_*}\sin(\omega_*t)-e^{-ict}\right].
$$

This satisfies $H(0)=\dot H(0)=0$ and contains both free oscillations and the forced component. At $c=\omega_*$ a solution of the [initial value problem](../../../../../initial-value-problem.md) still exists, but its [particular solution](../../../../../particular-solution.md) contains

$$
H_{\rm sec}(t)=-\frac{iPT}{2\omega_*}\,t e^{-i\omega_*t},
$$

which grows linearly with time. Thus the ideal [inviscid flow](../../../../../inviscid-flow.md) model predicts resonant growth rather than a finite constant [amplitude](../../../../../wave-amplitude.md). Additional free oscillations can set the [initial conditions](../../../../../initial-condition.md) but cannot remove that secular growth.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
