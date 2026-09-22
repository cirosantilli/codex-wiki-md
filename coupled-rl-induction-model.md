# Coupled RL induction model

↑ **Parent:** [Faraday induction-ring experiment](faraday-induction-ring-experiment.md)

Take two [electrical circuits](electrical-circuit-split.md) containing [coupled inductors](coupled-inductors.md). Let their constant [self-inductances](self-inductance.md) be $L_1,L_2>0$, [mutual inductance](mutual-inductance.md) $M$, and positive [electrical resistances](electrical-resistance.md) $R_1,R_2$. Choose current directions so that the off-diagonal entries of the [inductance matrix](inductance-matrix.md) are $+M$. Assume a linear, quasistatic model, with no capacitive effects or core [hysteresis](hysteresis.md). The [magnetic flux linkages](magnetic-flux-linkage.md) are $\lambda_1=L_1i_1+Mi_2$ and $\lambda_2=Mi_1+L_2i_2$. Combining their time derivatives with resistive [electric potential differences](electric-potential-difference.md) gives

$$
L_1\dot i_1+M\dot i_2+R_1i_1=V(t),\qquad
M\dot i_1+L_2\dot i_2+R_2i_2=0.
$$

The secondary is a closed, undriven [electrical circuit](electrical-circuit-split.md). Require $M^2<L_1L_2$, making $\mathbf L$ a [positive-definite matrix](positive-definite-matrix.md). The chosen current convention fixes the signs; reversing the secondary's reference direction changes the sign assigned to $M$ and $i_2$ without changing the physical circuit.

There is an essential switching assumption: **the primary loop remains closed when $V$ becomes zero**. An ideal [voltage source](voltage-source.md) then imposes zero [electric potential difference](electric-potential-difference.md), allowing the current to decay. Literally opening an inductive circuit requires additional physics to determine the interruption, including possible [capacitance](capacitance.md) and an [electric arc](electric-arc.md). This closed-return model explains transient induction while keeping that distinction from Faraday's historical making and breaking of contact explicit.

**Table of contents**

- [Equal-loop RL induction step](equal-loop-rl-induction-step.md)
- [Closed-return induction under a voltage pulse](closed-return-induction-under-a-voltage-pulse.md)
- [Energy balance of coupled RL circuits](energy-balance-of-coupled-rl-circuits.md)

## ↑ Ancestors (7)

1. [Faraday induction-ring experiment](faraday-induction-ring-experiment.md)
2. [Faraday's law of induction](faraday-s-law-of-induction.md)
3. [Maxwell equations](maxwell-equations-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Faraday induction-ring experiment](faraday-induction-ring-experiment.md)
