<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [Hodgkin-Huxley model](../../../../hodgkin-huxley-model.md), $V$ is the [membrane potential](../../../../membrane-potential-split.md), the [voltage](../../../../voltage.md) inside the axon relative to outside. The [space clamp](../../../../space-clamp.md) assumption makes it spatially uniform. The gating variables lie between zero and one: $m$ describes [sodium](../../../../sodium.md) activation, $h$ describes availability against [sodium](../../../../sodium.md) inactivation, and $n$ describes [potassium](../../../../potassium.md) activation. Thus large $h$ means channels remain available, not that inactivation is strong.

The left side $C_m\dot V$ is capacitive [electric current](../../../../electric-current.md) per unit membrane area. The imposed $I$ is inward-positive applied [electric current](../../../../electric-current.md). The other terms are outward-positive ionic [electric currents](../../../../electric-current.md): [sodium](../../../../sodium.md) with [electrical conductance](../../../../electrical-conductance.md) $g_{Na}m^3h$, [potassium](../../../../potassium.md) with conductance $g_Kn^4$, and a passive leak with conductance $g_L$. Each current is its conductance times the difference between $V$ and the corresponding [reversal potential](../../../../reversal-potential.md) $V_{Na}$, $V_K$ or $V_L$. The coefficients $g_{Na},g_K$ are maximal conductances; the gate factors represent [independent permissive gates in an ion channel](../../../../independent-permissive-gates-in-an-ion-channel.md).

For each gate, $k_\infty(V)$ is the equilibrium opening/availability fraction at fixed [voltage](../../../../voltage.md) and $\tau_k(V)>0$ its [exponential relaxation time](../../../../exponential-relaxation-time.md). The equation follows from [two-state ion-channel gating](../../../../two-state-ion-channel-gating.md): if $\dot k=\alpha_k(V)(1-k)-\beta_k(V)k$, then

$$
\boxed{k_\infty=\frac{\alpha_k}{\alpha_k+\beta_k},\qquad\tau_k=\frac1{\alpha_k+\beta_k}.}
$$

[Voltage](../../../../voltage.md) feedback couples these otherwise elementary gating equations to the [membrane potential](../../../../membrane-potential-split.md) and produces [action potentials](../../../../action-potential.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
