<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Use the ideal long-[solenoid](../../../../../solenoid.md) approximation: negligible pitch and end effects, vacuum permeability $\mu_0$, and negligible [displacement current](../../../../../displacement-current.md). By cylindrical symmetry the [magnetic field](../../../../../magnetic-field.md) is axial. An [Ampère's law](../../../../../ampere-s-circuital-law.md) rectangular loop with one axial side inside and the other outside gives $B_{\rm in}-B_{\rm out}=\mu_0NI$. A loop wholly outside shows the outside axial field is constant with radius; requiring it to vanish far away gives

$$
 \boxed{\mathbf B_{\rm in}=\mu_0NI\,\widehat{\mathbf z},\qquad
 \mathbf B_{\rm out}=0.}
$$

The axial sign is determined by the winding direction and the [right-hand rule](../../../../../right-hand-rule.md). The small axial component of current from the spiral pitch is neglected in this idealization.

There are $Nl$ turns, and the [magnetic flux](../../../../../magnetic-flux.md) through each is $\pi a^2\mu_0NI$. The flux linkage is $LI$, so the [self-inductance](../../../../../self-inductance.md) is

$$
 \boxed{L=\mu_0N^2\pi a^2l.}
$$

The induced [electromotive force](../../../../../electromotive-force.md) opposes increasing current by [Faraday's law](../../../../../faraday-s-law-of-induction.md). Together with [Ohm's law](../../../../../ohm-s-law.md), the circuit equation is $L\dot I+RI=\mathcal E_0$. Solving this first-order [ordinary differential equation](../../../../../ordinary-differential-equation.md) with $I(0)=0$ gives

$$
 \boxed{I(t)=\frac{\mathcal E_0}{R}\left(1-e^{-Rt/L}\right),\qquad t\geq0.}
$$

The [time constant](../../../../../time-constant.md) is $L/R$, and the limiting current is $\mathcal E_0/R$.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
