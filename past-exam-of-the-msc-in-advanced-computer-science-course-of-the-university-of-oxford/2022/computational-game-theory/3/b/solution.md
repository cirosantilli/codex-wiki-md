<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Against [Tit for tat](../../../../../tit-for-tat.md), let $a_t$ be an arbitrary deviator's action at round $t$, and set $a_{-1}=C$ to encode the opponent's initial cooperation. The opponent then plays $a_{t-1}$. Define $h(C)=0$ and $h(D)=3$. The four possible transitions give

$$
\begin{array}{c|c|c|c}
a_{t-1}&a_t&u(a_t,a_{t-1})&3+h(a_t)-h(a_{t-1})\\\hline
C&C&3&3\\
C&D&6&6\\
D&C&0&0\\
D&D&1&3
\end{array}
$$

Thus every stage [payoff](../../../../../payoff.md) is at most $3+h(a_t)-h(a_{t-1})$. The [telescoping sum](../../../../../telescoping-sum.md) yields the [uniform payoff bound against Tit for tat](../../../../../uniform-payoff-bound-against-tit-for-tat.md):

$$
\sum_{t=0}^{T-1}u(a_t,a_{t-1})\le3T+h(a_{T-1})-h(C)\le3T+3.
$$

After division by $T$, no [long-run average payoff](../../../../../long-run-average-payoff.md) can exceed three. The bound applies to every action [sequence](../../../../../sequence.md), so in particular it covers every [finite-state machine](../../../../../finite-state-machine.md) representing a [unilateral deviation](../../../../../unilateral-deviation.md). Mutual [Tit for tat](../../../../../tit-for-tat.md) produces $C,C$ in every round and gives each player three. Neither player can improve, proving **$(\mathrm{TFT},\mathrm{TFT})$ is a [Nash equilibrium](../../../../../nash-equilibrium.md)**.

Another pair is **$(\mathrm{TFT},\text{grim trigger})$**. Here [grim trigger](../../../../../grim-trigger.md) initially cooperates and continues cooperating until the opponent first defects, after which it defects forever. Both strategies are two-state [finite-state machines](../../../../../finite-state-machine.md): [Tit for tat](../../../../../tit-for-tat.md) records the opponent's previous action, while [grim trigger](../../../../../grim-trigger.md) records whether defection has ever occurred. Their prescribed play again consists entirely of cooperation and gives $(3,3)$.

The player using [grim trigger](../../../../../grim-trigger.md) faces [Tit for tat](../../../../../tit-for-tat.md), so every [unilateral deviation](../../../../../unilateral-deviation.md) is bounded by the same [telescoping sum](../../../../../telescoping-sum.md) and cannot improve on three. The player using [Tit for tat](../../../../../tit-for-tat.md) faces [grim trigger](../../../../../grim-trigger.md). If that player never defects, the [payoff](../../../../../payoff.md) remains three. If the first defection occurs at a finite round $\tau$, it gives a one-time [payoff](../../../../../payoff.md) six; thereafter the opponent always defects, against which each subsequent [payoff](../../../../../payoff.md) is at most one. Any finite initial prefix has zero contribution to the [long-run average payoff](../../../../../long-run-average-payoff.md), so such a [unilateral deviation](../../../../../unilateral-deviation.md) has limiting upper average at most one. It cannot improve on three either. Both players are therefore [best responses](../../../../../best-response.md), proving the second claimed [Nash equilibrium](../../../../../nash-equilibrium.md).

For deterministic [finite-state machines](../../../../../finite-state-machine.md), the joint state path is eventually periodic, so the displayed averages have a [limit](../../../../../limit-of-a-function.md). The first bound also controls the limiting upper average for arbitrary action [sequences](../../../../../sequence.md), making the no-improvement argument stronger than an enumeration of finite-state deviations. Notice that equality in the bound permits alternating exploitation to average three: equilibrium requires absence of a strict improvement, not uniqueness of a [best response](../../../../../best-response.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2022](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
