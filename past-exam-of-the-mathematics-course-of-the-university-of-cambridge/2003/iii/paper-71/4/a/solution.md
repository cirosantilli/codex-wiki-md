<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $v=\dot x$, $\zeta=6\pi\mu a$, and $\tau=m/\zeta$. To keep dimensions and the thermal amplitude explicit, write the [force](../../../../../../force.md) covariance as $\langle F(t)F(s)\rangle=A\delta(t-s)$. The printed unit coefficient is a choice of noise normalization, not a general dimensional thermal [force](../../../../../../force.md). Assume the initial [velocity](../../../../../../velocity.md) is independent of the future [white noise](../../../../../../white-noise.md). The [Underdamped Langevin dynamics](../../../../../../underdamped-langevin-dynamics.md) has integrating-factor solution

$$
v(t)=v_0e^{-t/\tau}+\frac1m\int_0^t e^{-(t-s)/\tau}F(s)\,ds.
$$

Taking its [expectation](../../../../../../expected-value.md) and using the delta covariance in the double integral gives

$$
\boxed{\langle v(t)\rangle=\langle v_0\rangle e^{-t/\tau},\qquad \langle v(t)^2\rangle=\langle v_0^2\rangle e^{-2t/\tau}+\frac{A}{2m\zeta}(1-e^{-2t/\tau}).}
$$

Here the noise contribution is $A m^{-2}\int_0^t e^{-2(t-s)/\tau}ds$. The [equipartition theorem](../../../../../../equipartition-theorem.md) requires the long-time value $\langle mv^2/2\rangle=k_BT/2$. Consequently the [fluctuation-dissipation relation for a Langevin particle](../../../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md) is

$$
\boxed{A=2\zeta k_BT,\qquad \langle F(t)F(s)\rangle=2\zeta k_BT\delta(t-s).}
$$

With an initially thermal [velocity](../../../../../../velocity.md), $\langle v_0\rangle=0$ and $\langle v_0^2\rangle=k_BT/m$, so the [velocity](../../../../../../velocity.md) variance is stationary. If one insists on the printed coefficient $A=1$ in dimensional units, the model has [temperature](../../../../../../temperature.md) fixed by $k_BT=1/(2\zeta)$ in those units; it cannot describe arbitrary [temperature](../../../../../../temperature.md) while retaining that coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
