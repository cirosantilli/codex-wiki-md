# Critically damped RLC response

↑ **Parent:** [Series RLC circuit](series-rlc-circuit.md)

A [critically damped RLC response](critically-damped-rlc-response.md) is the boundary between [underdamped RLC response](underdamped-rlc-response.md) and [overdamped RLC response](overdamped-rlc-response.md). The free [series RLC circuit](series-rlc-circuit.md) has a repeated [characteristic root](characteristic-root-of-a-constant-coefficient-differential-equation.md) $-\omega_0$, with general solution

$$
q(t)=(A+Bt)e^{-\omega_0t}.
$$

For [initial conditions](initial-condition.md) $q(0)=q_0$, $i(0)=0$,

$$
q(t)=q_0(1+\omega_0t)e^{-\omega_0t},\qquad
i(t)=-q_0\omega_0^2t e^{-\omega_0t}.
$$

In the plotted normalization, $q(1)=2/e\approx0.735759$ and $i(1)=-1/e\approx-0.367879$. The [electric charge](electric-charge-split.md) returns without ringing; the [polynomial](polynomial-split.md) factor $1+\omega_0t$ matters, so a single [exponential function](exponential-function.md) does not give the whole response.

For fixed $L,C$ and these [initial conditions](initial-condition.md), [critical damping](critical-damping.md) avoids ringing while giving a faster asymptotic return than any larger $R$: the [overdamped RLC response](overdamped-rlc-response.md) has a root closer to zero. This makes [critical damping](critical-damping.md) a useful tuning target for settling after switching. An MIT laboratory exercise makes the distinction observable by asking students to compare all three cases with $L=47\,\mathrm{mH}$ and $C=47\,\mathrm{nF}$. Those values give $R_{\mathrm{crit}}=2\sqrt{L/C}=2000\,\Omega$ and $\omega_0\approx21276.6\,\mathrm{s}^{-1}$. [MIT 6.071, Spring 2006, Laboratory 15, exercise 2](https://ocw.mit.edu/courses/6-071j-introduction-to-electronics-signals-and-measurement-spring-2006/491e7e50ee65521c601ee51d3c6f7e5f_lab15_transients.pdf).

## ↑ Ancestors (7)

1. [Series RLC circuit](series-rlc-circuit.md)
2. [RLC circuit](rlc-circuit.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Critically damped RLC response](critically-damped-rlc-response.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/5c/c/ii/solution.md)
- [Series RLC circuit](series-rlc-circuit.md)
- [Underdamped RLC response](underdamped-rlc-response.md)
