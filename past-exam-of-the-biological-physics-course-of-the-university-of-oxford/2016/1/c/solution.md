<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the instantaneous [electrical conductance](../../../../electrical-conductance.md) as $g_K(t)=\bar g_K n(t)^4$. Here $\bar g_K$ is the maximal [electrical conductance](../../../../electrical-conductance.md) of the recorded membrane, $n$ is the activation variable, $V_m$ is inside-minus-outside [membrane potential](../../../../membrane-potential-split.md), and $V_K$ is the [potassium](../../../../potassium.md) [Nernst equilibrium potential](../../../../nernst-equilibrium-potential.md). The factor $V_m-V_K$ is the electrochemical driving [voltage](../../../../voltage.md); positive $I_K$ conventionally denotes outward positive charge. For an [electric current](../../../../electric-current.md) density, $\bar g_K$ must instead be an [electrical conductance](../../../../electrical-conductance.md) per area.

In the [Hodgkin-Huxley model](../../../../hodgkin-huxley-model.md), four equivalent independent activation gates must all be permissive, each with [probability](../../../../probability.md) $n$, so their joint opening [probability](../../../../probability.md) is $n^4$. At fixed [voltage](../../../../voltage.md) each gate obeys

$$
\dot n=\alpha_n(V_m)(1-n)-\beta_n(V_m)n,\qquad
n_\infty=\frac{\alpha_n}{\alpha_n+\beta_n},\quad
\tau_n=\frac1{\alpha_n+\beta_n}.
$$

The model assumes approximately Ohmic open-channel conduction, a well-defined population-average [electrical conductance](../../../../electrical-conductance.md), and an almost constant [potassium](../../../../potassium.md) [reversal potential](../../../../reversal-potential.md) during a brief recording. Four phenomenological gates should not be mistaken for a proof of four physically independent molecular transitions. The simple delayed-rectifier description also omits [ion-channel inactivation](../../../../ion-channel-inactivation.md).

Reducing the available [electrical conductance](../../../../electrical-conductance.md) can weaken [repolarization](../../../../repolarization.md), broaden an [action potential](../../../../action-potential.md) and alter repetitive firing. Depending on channel class and tissue, excess excitability or impaired recovery can follow; persistent depolarization can also reduce [voltage-gated sodium channel](../../../../voltage-gated-sodium-channel.md) availability. Cardiac potassium-current reductions can prolong the [action potential](../../../../action-potential.md) and contribute to [Long QT syndrome](../../../../long-qt-syndrome.md). These are conditional physiological consequences, not a claim that every potassium-current reduction has the same clinical effect.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
