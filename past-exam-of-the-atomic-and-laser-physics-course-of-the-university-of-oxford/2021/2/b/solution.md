<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume an initially unexcited [chemical atom](../../../../atom-physics.md), two nonoverlapping square pulses starting at $0,T$, and a common coherent field phase. In the weak-excitation limit $|\Omega|\tau_p\ll1$, substitute $c_1=1+O(\Omega^2)$ into the second [probability amplitude](../../../../probability-amplitude.md) equation. After the second pulse,

$$
\begin{aligned}
c_2&=-\frac{i\Omega}{2}\left(\int_0^{\tau_p}e^{-i\delta t}\,dt+\int_T^{T+\tau_p}e^{-i\delta t}\,dt\right)+O(\Omega^3)\\
&=-i\Omega\tau_p\,e^{-i\delta(T+\tau_p)/2}\operatorname{sinc}(\delta\tau_p/2)\cos(\delta T/2)+O(\Omega^3),
\end{aligned}
$$

where the [sinc function](../../../../sinc-function.md) means $\operatorname{sinc}u=\sin u/u$, with value one at zero. Squaring gives

$$
\boxed{P_2=(\Omega\tau_p)^2\operatorname{sinc}^2(\delta\tau_p/2)\cos^2(\delta T/2)+O((\Omega\tau_p)^4).}
$$

The printed prefactor is a factor of four too small for the supplied equations and pulse durations. A direct counterexample is $\delta=0$: the exact resonant [Rabi oscillation](../../../../rabi-cycle.md) gives $P_2=\sin^2(\Omega\tau_p)$ for two pulses of duration $\tau_p$, because the intervening resonant rotating-frame evolution is trivial. Its small-area limit is $(\Omega\tau_p)^2$, rather than $(\Omega\tau_p/2)^2$. The latter is the single-pulse result before coherent addition.

The condition $\omega\tau_p\ll1$ printed in the source also does not justify the derivation from a physical carrier field. A consistent [rotating-wave approximation](../../../../rotating-wave-approximation.md) pulse regime is

$$
\boxed{\omega_0^{-1}\ll\tau_p\ll|\Omega|^{-1},\qquad |\delta|\ll\omega_0.}
$$

If the supplied equations are treated as the mathematical model regardless, their weak-excitation integral remains valid for any $\tau_p$; subcycle pulses of the original real field require the discarded counter-rotating term and depend on carrier phase. $T$ here is the separation of pulse starts, as specified, rather than the dark interval $T-\tau_p$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
