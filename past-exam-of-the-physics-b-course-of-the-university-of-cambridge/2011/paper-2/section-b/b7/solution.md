<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

[Self-inductance](../../../../../self-inductance.md) relates current to its own [magnetic flux linkage](../../../../../magnetic-flux-linkage.md): $\Lambda=LI$, so the induced [electromotive force](../../../../../electromotive-force.md) is $-L\dot I$ for fixed geometry. A long [solenoid](../../../../../solenoid.md) has $B=\mu_0NI/l$ and area $\pi a^2$. Its $N$ turns give

$$
\boxed{L=\frac{\mu_0N^2\pi a^2}{l}.}
$$

The [homopolar generator](../../../../../homopolar-generator.md) uses a disc rotating through this axial field; integrate the motional [Lorentz force](../../../../../lorentz-force.md) from shaft to rim:

$$
\mathcal E=\int_0^a\omega rB\,dr=\frac12\omega B a^2=C\omega I,\qquad C=\frac{\mu_0Na^2}{2l}.
$$

For a [homopolar disc dynamo](../../../../../homopolar-disc-dynamo.md), choose the wiring and rotation sense giving positive magnetic feedback. [Kirchhoff's voltage law](../../../../../kirchhoff-cycle-law.md) is

$$
L\dot I+RI=C\omega I,\qquad I(t)=I(0)\exp\!\left[\frac{C\omega-R}{L}t\right]
$$

for prescribed constant $\omega$. Thus

$$
\boxed{\omega_c=\frac{R}{C}=\frac{2Rl}{\mu_0Na^2}.}
$$

A nonzero seed grows when $\omega>\omega_c$, decays when $\omega<\omega_c$, and is marginal at equality. This explains the printed $\omega\geq\omega_c$ as the threshold including its boundary; equality does not itself give exponential growth. An exactly zero initial current remains zero in the ideal homogeneous equation, and reversing the feedback sense prevents the instability.

In the [torque-controlled homopolar dynamo equilibrium](../../../../../torque-controlled-homopolar-dynamo-equilibrium.md), a radial current element exerts a braking [torque](../../../../../torque.md) $dG_B=I B r\,dr$, so $G_B=IBa^2/2=C I^2$. For steady rotation and nonzero steady current, $G=CI^2$ and $\omega=\omega_c$. Hence the field intensity magnitude is

$$
\boxed{|H|=\frac Nl\sqrt{\frac GC}=\sqrt{\frac{2NG}{\mu_0a^2l}}.}
$$

The two current signs give opposite magnetic polarities. Finally,

$$
\boxed{P_{\rm mechanical}=G\omega_c=CI^2\frac RC=RI^2=P_{\rm Joule}.}
$$

The steady magnetic and rotational [energies](../../../../../energy-split.md) do not change. This is a steady-state balance, not an assertion that every dynamical trajectory must approach that state.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
