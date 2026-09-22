# RL circuit

↑ **Parent:** [Electrical circuit](electrical-circuit-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/RL_circuit)

An [RL circuit](rl-circuit.md) combines [electrical resistance](electrical-resistance.md) $R$ and [self-inductance](self-inductance.md) $L$. In the series model, the same [electric current](electric-current.md) $I$ flows through both components. An ideal [battery](electric-battery.md) maintains terminal [electric potential difference](electric-potential-difference.md) $V$; the drops in the direction of positive [electric current](electric-current.md) obey [Ohm's law](ohm-s-law.md) and the [inductor](inductor.md) relation:

$$
v_R=RI,\qquad v_L=L\frac{dI}{dt},\qquad
V=v_R+v_L.
$$

This is [Kirchhoff's voltage law](kirchhoff-cycle-law.md) with the [inductor](inductor.md)'s terminal drop, rather than its oppositely signed induced [electromotive force](electromotive-force.md). For constant $R>0$, $L>0$, and $V$, the [first-order linear differential equation](first-order-linear-differential-equation.md) has solution

$$
I(t)=I_\infty+(I(0)-I_\infty)e^{-t/\tau},\qquad
I_\infty=\frac VR,\qquad \tau=\frac LR.
$$

The [time constant](time-constant.md) $\tau$ measures [exponential decay](exponential-decay.md) of the difference from the final [electric current](electric-current.md). [OpenStax University Physics 2, §14.4: RL circuits](https://openstax.org/books/university-physics-volume-2/pages/14-4-rl-circuits).

For a stipulated example, take [electrical resistance](electrical-resistance.md) $R=2\,\Omega$, [self-inductance](self-inductance.md) $L=0.5\,\mathrm H$, terminal [electric potential difference](electric-potential-difference.md) $V=6\,\mathrm V$, and initial [electric current](electric-current.md) $I(0)=0$. Then

$$
\tau=0.25\,\mathrm s,\qquad I_\infty=3\,\mathrm A,
\qquad I(t)=(3\,\mathrm A)(1-e^{-t/(0.25\,\mathrm s)}).
$$

With $t$ measured numerically in seconds, this is $I(t)=3(1-e^{-4t})$ in amperes. At one [time constant](time-constant.md),

$$
I(\tau)=3(1-e^{-1})\,\mathrm A\approx1.89636\,\mathrm A,
$$

and the terminal [electric potential difference](electric-potential-difference.md) drops are

$$
v_R(\tau)=6(1-e^{-1})\,\mathrm V\approx3.79272\,\mathrm V,
\qquad v_L(\tau)=6e^{-1}\,\mathrm V\approx2.20728\,\mathrm V.
$$

Their sum is exactly $6\,\mathrm V$. At $t=0^+$, the [inductor](inductor.md) takes the entire terminal [electric potential difference](electric-potential-difference.md) while the [electric current](electric-current.md) is still zero. At steady [electric current](electric-current.md), the [inductor](inductor.md)'s terminal drop is zero and the entire drop is across the [electrical resistance](electrical-resistance.md).

<a id="image-electric-current-and-terminal-electric-potential-difference-drops-during-an-rl-circuit-response"></a>
![](rl-current-and-voltage.png)

**[Figure 13](#image-electric-current-and-terminal-electric-potential-difference-drops-during-an-rl-circuit-response). Electric current and terminal electric potential difference drops during an RL circuit response**. The [battery](electric-battery.md) maintains $6\,\mathrm V$ across [electrical resistance](electrical-resistance.md) $2\,\Omega$ and [self-inductance](self-inductance.md) $0.5\,\mathrm H$ in series. The dashed vertical line marks [time constant](time-constant.md) $0.25\,\mathrm s$; $v_L$ uses the positive terminal-drop convention.

The final [magnetic energy](magnetic-energy.md) stored by the [inductor](inductor.md) is $U_\infty=LI_\infty^2/2=2.25\,\mathrm J$. At one [time constant](time-constant.md), the [electric current](electric-current.md) has reached about $63.21\%$ of its final value, but its [magnetic energy](magnetic-energy.md) has reached only about $39.96\%$:

$$
U(\tau)=\frac12L I(\tau)^2
=2.25(1-e^{-1})^2\,\mathrm J\approx0.899047\,\mathrm J.
$$

This difference follows from the square of [electric current](electric-current.md) in the [inductor](inductor.md)'s [magnetic energy](magnetic-energy.md).

For release, take $t=0$ at the start of a separate experiment with initial [electric current](electric-current.md) $3\,\mathrm A$. Remove the [battery](electric-battery.md) from the model while maintaining a closed path through the same [electrical resistance](electrical-resistance.md) and [inductor](inductor.md). Then

$$
L\frac{dI}{dt}+RI=0,\qquad
I(t)=(3\,\mathrm A)e^{-t/(0.25\,\mathrm s)}.
$$

Now $v_L=-v_R$: the induced [electromotive force](electromotive-force.md) supports the continuing positive [electric current](electric-current.md) as its magnitude decreases. This closed-loop model describes [exponential decay](exponential-decay.md), not opening the sole path and imposing an instantaneous jump to zero [electric current](electric-current.md). The [inductor](inductor.md)'s [magnetic energy](magnetic-energy.md) and the [power](power.md) of [Joule heating](joule-heating.md) are

$$
U(t)=(2.25\,\mathrm J)e^{-2t/\tau},\qquad
P_R(t)=RI(t)^2=(18\,\mathrm W)e^{-2t/\tau},\qquad
\frac{dU}{dt}=-P_R.
$$

Their [time constant](time-constant.md) is $\tau/2=0.125\,\mathrm s$. The total [energy](energy-split.md) dissipated by [Joule heating](joule-heating.md) is exactly the initial [magnetic energy](magnetic-energy.md):

$$
\int_0^\infty P_R(t)\,dt
=(18\,\mathrm W)\frac{\tau}{2}=2.25\,\mathrm J.
$$

The second diagram in [inductor](inductor.md) shows this [energy](energy-split.md) transfer. A finite closed path lets us predict both how long the [electric current](electric-current.md) persists and how much [energy](energy-split.md) becomes heat. [OpenStax University Physics 2, §14.4: decay in a closed RL loop](https://openstax.org/books/university-physics-volume-2/pages/14-4-rl-circuits).

## ↑ Ancestors (5)

1. [Electrical circuit](electrical-circuit-split.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Inductor](inductor.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-a/6/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-e/15/c/solution.md)
- [Persistent current (superconductivity)](persistent-current-superconductivity.md)
- [Resistance upper bound from persistent-current decay](resistance-upper-bound-from-persistent-current-decay.md)
- [RL circuit](rl-circuit.md)
- [RL low-pass filter](rl-low-pass-filter.md)
- [Self-inductance](self-inductance.md)
- [Stored energy of a solenoid](stored-energy-of-a-solenoid.md)
