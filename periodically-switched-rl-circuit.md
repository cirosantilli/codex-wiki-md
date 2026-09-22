# Periodically switched RL circuit

↑ **Parent:** [RL circuit](rl-circuit.md)

An [RL circuit](rl-circuit.md) alternating for equal intervals $\Delta t$ between zero drive and constant drive $V$ has a unique attracting periodic [electric current](electric-current.md) when $R,L,\Delta t>0$. Write $s=e^{-R\Delta t/L}$ and $J=V/R$. Sampling just before each zero-drive interval gives the [recurrence relation](recurrence-relation.md) $I_{n+1}=s^2I_n+J(1-s)$. Subtracting its [fixed point](fixed-point.md) yields $I_n-J/(1+s)=s^{2n}[I_0-J/(1+s)]$. Thus the limiting upper and lower [electric currents](electric-current.md) are $J/(1+s)$ and $sJ/(1+s)$; convergence is geometric. This gives a simple exact ripple estimate for a periodically driven [inductor](inductor.md).

## ↑ Ancestors (6)

1. [RL circuit](rl-circuit.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-2-paper-of-the-university-of-oxford/2022/1/ii/solution.md)
