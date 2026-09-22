<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The definition in this part uses a single [Boolean valuation](../../../../../boolean-valuation.md), so the relevant [Nash equilibria](../../../../../nash-equilibrium.md) are [pure strategy](../../../../../pure-strategy.md) equilibria of a [Boolean game](../../../../../boolean-game.md). Use its standard convention that the players' control sets form a [set partition](../../../../../set-partition.md) of the variables.

Membership follows from an existential choice of a [strategy profile](../../../../../strategy-profile.md) and a universal check of all [unilateral deviations](../../../../../unilateral-deviation.md). Assign [payoff](../../../../../payoff.md) one to satisfying a player's goal and zero otherwise. A [strategy profile](../../../../../strategy-profile.md) $\sigma$ is a [Nash equilibrium](../../../../../nash-equilibrium.md) precisely when, for every player $i$ and every alternative [Boolean valuation](../../../../../boolean-valuation.md) $\tau_i$ of that player's variables,

$$
\gamma_i(\sigma)\ \lor\ \neg\gamma_i(\tau_i,\sigma_{-i})
$$

is true: either the goal is already satisfied or no deviation can satisfy it. Thus the requested property is

$$
\exists\sigma\ \forall(i,\tau_i)\quad
\left[
\phi(\sigma)\land
\bigl(\gamma_i(\sigma)\lor
\neg\gamma_i(\tau_i,\sigma_{-i})\bigr)
\right].
$$

The strings encoding $\sigma$, $i$ and $\tau_i$ have polynomial length, and evaluating the bracketed [propositional formulas](../../../../../propositional-formula.md) takes [polynomial time](../../../../../polynomial-time.md). Invalid encodings of a player index can simply be ignored by the test. This is the existential [second level of the polynomial hierarchy](../../../../../second-level-of-the-polynomial-hierarchy.md), $\Sigma_2^{\mathrm P}$.

For hardness, reduce the canonical complete problem of deciding a [two-block quantified Boolean formula](../../../../../two-block-quantified-boolean-formula.md)

$$
\exists X\ \forall Y\ \psi(X,Y).
$$

Make a two-player [Boolean game](../../../../../boolean-game.md): player 1 controls $X$ and has goal $\gamma_1=\top$; player 2 controls $Y$ and has goal $\gamma_2=\neg\psi$. Set the query formula to $\phi=\psi$. The construction has size linear in the input formula.

If an assignment $x$ satisfies $\forall Y\,\psi(x,Y)$, combine it with any assignment $y$. Player 1 already satisfies its goal, and player 2 cannot satisfy $\neg\psi$ by any [unilateral deviation](../../../../../unilateral-deviation.md). Thus $(x,y)$ is a [Nash equilibrium](../../../../../nash-equilibrium.md) satisfying the query.

Conversely, let $(x,y)$ be a [Nash equilibrium](../../../../../nash-equilibrium.md) satisfying $\psi$. Player 2 currently has [payoff](../../../../../payoff.md) zero. If some alternative $y'$ made $\psi(x,y')$ false, that deviation would satisfy player 2's goal and increase its [payoff](../../../../../payoff.md) to one. The [Nash equilibrium](../../../../../nash-equilibrium.md) condition therefore implies $\forall Y\,\psi(x,Y)$. This proves the required equivalence and the [polynomial-time reduction](../../../../../polynomial-time-reduction.md).

Together, membership and hardness prove **$\Sigma_2^{\mathrm P}$-completeness** of [existential equilibrium checking in a Boolean game](../../../../../existential-equilibrium-checking-in-a-boolean-game.md). The reduction works with only two players and one constant goal.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2023](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
