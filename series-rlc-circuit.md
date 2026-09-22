# Series RLC circuit

↑ **Parent:** [RLC circuit](rlc-circuit.md)

In a [series RLC circuit](series-rlc-circuit.md), the same [electric current](electric-current.md) $i=q'$ flows through the [resistor](resistor.md) with [electrical resistance](electrical-resistance.md) $R$, the [inductor](inductor.md), and the [capacitor](capacitor.md). Choose $q$ as the signed [electric charge](electric-charge.md) on the [capacitor](capacitor.md) plate into which positive $i$ flows. With terminal drops measured in that direction, [Kirchhoff's voltage law](kirchhoff-cycle-law.md) gives

$$
v_R=Ri,\qquad v_L=Li',\qquad v_C=q/C,\qquad
Lq''+Rq'+q/C=V(t).
$$

Here $V(t)$ is the applied [electric potential difference](electric-potential-difference.md); assume constant $L>0$, $C>0$, and $R>0$. With the applied source set to zero and the loop kept closed, the free response satisfies

$$
q''+2\alpha q'+\omega_0^2q=0,\qquad
\alpha=\frac{R}{2L},\qquad \omega_0=\frac{1}{\sqrt{LC}}.
$$

The [angular frequency](angular-frequency.md) $\omega_0$ is the value for lossless free [oscillation](oscillation.md); $\alpha$ is the decay parameter. The three possibilities are [underdamped RLC response](underdamped-rlc-response.md) for $\alpha<\omega_0$, [critically damped RLC response](critically-damped-rlc-response.md) for $\alpha=\omega_0$, and [overdamped RLC response](overdamped-rlc-response.md) for $\alpha>\omega_0$. [OpenStax University Physics 2, §14.6: free RLC response](https://openstax.org/books/university-physics-volume-2/pages/14-6-rlc-series-circuits).

For a fair comparison, start each circuit with the same [electric charge](electric-charge.md) $q(0)=q_0$ and zero [electric current](electric-current.md) $q'(0)=0$. Set $\tau=\omega_0t$ and $a=\alpha/\omega_0$; then $x=q/q_0$ obeys $d^2x/d\tau^2+2a\,dx/d\tau+x=0$. The plot compares $a=0.5,1,2$. These dimensionless curves apply to any $L,C$ after rescaling time and [electric charge](electric-charge.md).

<a id="image-free-series-rlc-circuit-responses-with-identical-initial-conditions"></a>
![](rlc-free-damping.png)

**[Figure 6](#image-free-series-rlc-circuit-responses-with-identical-initial-conditions). Free series RLC circuit responses with identical initial conditions**. Left: [electric charge](electric-charge.md) for [underdamped RLC response](underdamped-rlc-response.md), [critically damped RLC response](critically-damped-rlc-response.md), and [overdamped RLC response](overdamped-rlc-response.md). Right: total stored [energy](energy.md), which decreases in all three cases even when [electric charge](electric-charge.md) oscillates. The normalization is $\omega_0=1$, $q_0=1$, $q'(0)=0$.

The stored [energy](energy.md) is the sum of [magnetic energy](magnetic-energy.md) and [capacitor energy](capacitor-energy.md):

$$
E=\frac12Li^2+\frac{q^2}{2C}.
$$

Differentiating and using the circuit equation gives the complete [power](power.md) balance,

$$
E'=i\left(Li'+\frac qC\right)=V(t)i-Ri^2.
$$

In the free response, $E'=-Ri^2\leq0$: [Joule heating](joule-heating.md) accounts exactly for the lost [energy](energy.md). For the plotted [initial conditions](initial-condition.md), $E(0)=q_0^2/(2C)$ and $E/E(0)=x^2+(dx/d\tau)^2$. Since every free solution tends to zero for $R>0$,

$$
\int_0^\infty Ri(t)^2\,dt=E(0).
$$

In the lossless limit $R=0$, [energy](energy.md) stays constant and shuttles between the [capacitor](capacitor.md) and [inductor](inductor.md). Thus an [oscillation](oscillation.md) of [electric charge](electric-charge.md) and a decrease of total [energy](energy.md) are compatible statements.

The analogy with a [damped harmonic oscillator](damped-harmonic-oscillator.md) is exact within these ideal models: [electric charge](electric-charge.md) corresponds to displacement, [electric current](electric-current.md) to [velocity](velocity.md), [inductance](inductance.md) to [mass](mass.md), $1/C$ to [spring constant](spring-constant.md), and $R$ to the coefficient of a resisting force proportional to [velocity](velocity.md). The two stored [energy](energy.md) terms play the roles of [kinetic energy](kinetic-energy.md) and elastic [potential energy](potential-energy.md). [Feynman lectures, I.23.3: the oscillator analogy](https://www.feynmanlectures.caltech.edu/I_23.html#Ch23-S3).

Differentiating the driven equation also gives $Li''+Ri'+i/C=V'$. When using this equation to solve for [electric current](electric-current.md), retain the original constraint $Li'(0)+Ri(0)+q(0)/C=V(0)$: the initial [electric charge](electric-charge.md) fixes the initial rate of change of [electric current](electric-current.md).

**Table of contents**

- [Resonant series RLC response](resonant-series-rlc-response.md)
- [Overdamped RLC response](overdamped-rlc-response.md)
- [Critically damped RLC response](critically-damped-rlc-response.md)
- [Underdamped RLC response](underdamped-rlc-response.md)

## ↑ Ancestors (6)

1. [RLC circuit](rlc-circuit.md)
2. [Electrical circuit](electrical-circuit.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Band-pass filter](band-pass-filter.md)
- [Critically damped RLC response](critically-damped-rlc-response.md)
- [Electrical engineering](electrical-engineering-split.md)
- [Electrical impedance](electrical-impedance.md)
- [Electrical reactance](electrical-reactance.md)
- [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)
- [Linear filter](linear-filter.md)
- [Overdamped RLC response](overdamped-rlc-response.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/5c/b/solution.md)
- [Q factor](q-factor.md)
- [Resistor](resistor.md)
- [Resonant series RLC response](resonant-series-rlc-response.md)
- [RLC circuit](rlc-circuit.md)
- [Series RLC circuit](series-rlc-circuit.md)
- [Underdamped RLC response](underdamped-rlc-response.md)
