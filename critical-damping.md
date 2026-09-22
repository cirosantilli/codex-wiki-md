# Critical damping

↑ **Parent:** [Damping](damping.md)

[Critical damping](critical-damping.md) is the repeated-root case of the [viscous damping](viscous-damping.md) model: its two [characteristic roots](characteristic-root-of-a-constant-coefficient-differential-equation.md) coincide at $r=-\omega_0$. The solution with arbitrary [initial conditions](initial-condition.md) is

$$
x(t)=\bigl[x_0+(v_0+\omega_0x_0)t\bigr]e^{-\omega_0t}.
$$

The extra factor $t$ is essential: one [exponential function](exponential-function.md) alone cannot fit arbitrary initial [displacement](displacement.md) and [velocity](velocity.md) when the [characteristic equation](characteristic-equation-of-a-constant-coefficient-differential-equation.md) has a double [polynomial root](root-of-a-polynomial.md). Substitution, or taking the limit of the [underdamped](underdamping.md) formula as its [angular frequency](angular-frequency.md) tends to zero, gives the displayed expression.

The precise fastest-return statement is this: hold $m$, $k$, $x_0>0$ and $v_0=0$ fixed, and compare all $\zeta\geq1$. Every response decreases positively toward [equilibrium](equilibrium-point-of-a-dynamical-system.md); the [critically damped](critical-damping.md) response

$$
x_{\mathrm c}(t)=x_0(1+\omega_0t)e^{-\omega_0t}
$$

is smaller than every [overdamped](overdamping.md) response at each $t>0$. It therefore reaches and stays within any specified band $|x|\leq\epsilon x_0$, $0<\epsilon<1$, sooner than those responses. Exact arrival at rest takes infinite [time](time-in-physics.md). This is a comparison among nonoscillatory regimes for these particular [initial conditions](initial-condition.md), not a universal minimum of every possible settling-time criterion.

One short comparison argument uses $q=\partial X/\partial\zeta$. Its [initial conditions](initial-condition.md) are zero and $q''+2\zeta q'+q=-2X'$. For release from rest, $X'<0$ at $\tau>0$; the [causal Green function of a damped oscillator](causal-green-function-of-a-damped-oscillator.md) is positive at positive [time](time-in-physics.md) for $\zeta\geq1$. Its [convolution](convolution.md) with $-2X'$ gives $q>0$: increasing [damping](damping.md) beyond the critical value increases the remaining [displacement](displacement.md).

There is no repeated [oscillation](oscillation.md) at [critical damping](critical-damping.md), but there can be overshoot once. For $x_0>0$, the factor in square brackets crosses zero precisely when $v_0<-\omega_0x_0$, at

$$
t_*=-\frac{x_0}{v_0+\omega_0x_0}>0.
$$

For example, $v_0=-2\omega_0x_0$ gives $x=x_0(1-\omega_0t)e^{-\omega_0t}$, crossing [equilibrium](equilibrium-point-of-a-dynamical-system.md) at $t=1/\omega_0$ as shown above. An [overdamped](overdamping.md) response can also cross once for suitable [initial conditions](initial-condition.md). Conversely, specially chosen [initial conditions](initial-condition.md) can remove its slow [exponential decay](exponential-decay.md) entirely. Thus the generic slow-root argument must not be applied to a response whose slow-root coefficient is zero.

## ↑ Ancestors (7)

1. [Damping](damping.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Critical damping](critical-damping.md)
- [Critically damped RLC response](critically-damped-rlc-response.md)
- [Damping](damping.md)
- [Damping measurement from free decay](damping-measurement-from-free-decay.md)
- [Damping ratio](damping-ratio.md)
- [Logarithmic decrement](logarithmic-decrement.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/12d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/12d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2/8b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/13b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-321/3/d/solution.md)
- [Velocity-impulse Green function for a damped string](velocity-impulse-green-function-for-a-damped-string.md)
