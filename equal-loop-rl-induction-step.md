# Equal-loop RL induction step

↑ **Parent:** [Coupled RL induction model](coupled-rl-induction-model.md)

For an exactly soluble example, set $L_1=L_2=L$, $R_1=R_2=R$, and $0<M<L$. Start with zero [electric currents](electric-current.md), and apply a constant [electric potential difference](electric-potential-difference.md) $V_0>0$ at $t=0$. The sums $s=i_1+i_2$ and $d=i_1-i_2$ obey separate [first-order linear differential equations](first-order-linear-differential-equation.md):

$$
(L+M)\dot s+Rs=V_0,\qquad
(L-M)\dot d+Rd=V_0.
$$

Their [time constants](time-constant.md) are $\tau_+=(L+M)/R$ and $\tau_-=(L-M)/R$. Thus, for $t\geq0$,

$$
i_1(t)=\frac{V_0}{2R}\left(2-e^{-t/\tau_+}-e^{-t/\tau_-}\right),\qquad
i_2(t)=\frac{V_0}{2R}\left(e^{-t/\tau_-}-e^{-t/\tau_+}\right).
$$

Since $\tau_-<\tau_+$, **$i_2(t)<0$ for $t>0$, but $i_2(t)\to0$ as $t\to\infty$**. The primary approaches $V_0/R$. The secondary response opposes the rise of linked [magnetic flux](magnetic-flux.md), in accordance with [Lenz's law](lenz-s-law.md). Removing [mutual inductance](mutual-inductance.md) by setting $M=0$ makes the two exponentials equal and gives zero secondary [electric current](electric-current.md).

For stipulated $L=0.1\,\mathrm H$, $M=0.06\,\mathrm H$, $R=10\,\Omega$ and $V_0=1\,\mathrm V$, the two [time constants](time-constant.md) are $16\,\mathrm{ms}$ and $4\,\mathrm{ms}$. Setting $\dot i_2=0$ gives its largest negative magnitude at

$$
t_* =\frac{\tau_+\tau_-}{\tau_+-\tau_-}\log\frac{\tau_+}{\tau_-}
\simeq7.394\,\mathrm{ms},\qquad
i_2(t_*)\simeq-23.62\,\mathrm{mA}.
$$

The continuing primary [electric current](electric-current.md) eventually reaches $100\,\mathrm{mA}$ while the secondary returns to zero. These numbers belong to the stated model, not the 1831 apparatus.

## ↑ Ancestors (8)

1. [Coupled RL induction model](coupled-rl-induction-model.md)
2. [Faraday induction-ring experiment](faraday-induction-ring-experiment.md)
3. [Faraday's law of induction](faraday-s-law-of-induction.md)
4. [Maxwell equations](maxwell-equations-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Closed-return induction under a voltage pulse](closed-return-induction-under-a-voltage-pulse.md)
