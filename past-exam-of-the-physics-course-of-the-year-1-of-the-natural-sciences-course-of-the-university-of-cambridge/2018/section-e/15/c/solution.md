<h1 id="section-e/15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Faraday's law of induction](../../../../../faraday-s-law-of-induction.md) relates an induced [electromotive force](../../../../../electromotive-force.md) to the rate of change of [magnetic flux](../../../../../magnetic-flux.md). Choose a positive orientation around a loop and its associated surface normal by the [right-hand rule](../../../../../right-hand-rule.md). For a stationary conducting loop,

$$
\Phi_B=\int_S\mathbf B\cdot d\mathbf S,\qquad
\boxed{\mathcal E=\oint\mathbf E\cdot d\mathbf l=-\frac{d\Phi_B}{dt}.}
$$

Unlike an electrostatic field, the induced [electric field](../../../../../electric-field-split.md) generally has nonzero [curl](../../../../../curl.md); the differential form is $\nabla\times\mathbf E=-\partial\mathbf B/\partial t$. For a moving circuit, [magnetic flux transport for a moving circuit](../../../../../magnetic-flux-transport-for-a-moving-circuit.md) includes the magnetic [Lorentz force](../../../../../lorentz-force.md) on the charges:

$$
\mathcal E=\oint(\mathbf E+\mathbf u\times\mathbf B)\cdot d\mathbf l
=-\frac{d\Phi_B}{dt},
$$

where $\mathbf u$ is the local wire [velocity](../../../../../velocity.md). Thus changing the field or moving a conductor can produce induction.

The minus sign is [Lenz's law](../../../../../lenz-s-law.md): an induced [electric current](../../../../../electric-current.md), when a closed conducting path permits it, produces a [magnetic field](../../../../../magnetic-field-split.md) opposing the change of linked flux. It need not oppose the original field itself. For example, increasing flux through a loop produces a current tending to reduce that increase; decreasing the same flux reverses the current. The opposition is consistent with [conservation of energy](../../../../../conservation-of-energy.md): external mechanical or electrical [work](../../../../../work.md) is needed to maintain a change against its inductive reaction.

For a coil of $N$ turns, define the [magnetic flux linkage](../../../../../magnetic-flux-linkage.md) $\Lambda=\sum_{j=1}^N\Phi_j$, reducing to $N\Phi_B$ when every turn links the same flux. For fixed geometry and a linear magnetic response, [self-inductance](../../../../../self-inductance.md) $L$ is defined by $\Lambda=LI$, and the coil's induced [electromotive force](../../../../../electromotive-force.md) is

$$
\boxed{\mathcal E_{\rm self}=-L\frac{dI}{dt},\qquad [L]=\mathrm H=\mathrm{Wb\,A^{-1}}.}
$$

The corresponding terminal voltage drop, with the [passive sign convention](../../../../../passive-sign-convention.md), is $V_L=L\,dI/dt$. It opposes changes in [electric current](../../../../../electric-current.md); it does not require the current itself to vanish.

Building the current from zero requires power $P=IV_L=LI\,dI/dt$. Integrating gives the energy stored by an ideal [inductor](../../../../../inductor.md):

$$
\boxed{U_B=\int_0^I LI'\,dI'=\frac12LI^2.}
$$

This energy is stored in the [magnetic field](../../../../../magnetic-field-split.md) and can be returned when the current falls. In a series [RL circuit](../../../../../rl-circuit.md) driven by a constant voltage $V_0$, [Kirchhoff's voltage law](../../../../../kirchhoff-cycle-law.md) gives $L\dot I+RI=V_0$. Starting with zero current, $I=(V_0/R)(1-e^{-tR/L})$, with [time constant](../../../../../time-constant.md) $L/R$. This makes the resistance to rapid current changes directly observable. Two coils also have [mutual inductance](../../../../../mutual-inductance.md): changing primary current induces secondary [electromotive force](../../../../../electromotive-force.md) $-M\,dI_1/dt$ with a polarity determined by the chosen winding orientations, the principle behind a transformer.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
3. [Section E](../../../section-e.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
