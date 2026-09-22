<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The succinct input is the players' variable-control sets, their goal [propositional formulas](../../../../../propositional-formula.md), and a complete candidate [Boolean valuation](../../../../../boolean-valuation.md); an exponentially expanded [payoff matrix](../../../../../payoff-matrix.md) is not part of the input. This representation is essential to [candidate equilibrium checking in a Boolean game](../../../../../candidate-equilibrium-checking-in-a-boolean-game.md).

For membership in [co-NP](../../../../../co-np.md), consider the complement: the candidate is not a [Nash equilibrium](../../../../../nash-equilibrium.md). A [complexity certificate](../../../../../certificate-complexity.md) consists of a player $i$ and an alternative [Boolean valuation](../../../../../boolean-valuation.md) of that player's controlled [Boolean variables](../../../../../boolean-variable.md). Evaluate the current goal and the goal after this [unilateral deviation](../../../../../unilateral-deviation.md), keeping every other player's variables fixed. A profitable [unilateral deviation](../../../../../unilateral-deviation.md) exists precisely when the current goal is false and the new goal is true. The certificate has at most the number of input variables plus the player index, and both [propositional formula](../../../../../propositional-formula.md) evaluations take [polynomial time](../../../../../polynomial-time.md). Thus the complement belongs to [NP](../../../../../np-complexity.md), and the original [decision problem](../../../../../decision-problem.md) belongs to [co-NP](../../../../../co-np.md).

For hardness, start with a [propositional formula](../../../../../propositional-formula.md) $F(X)$ and introduce a fresh [Boolean variable](../../../../../boolean-variable.md) $z$. Construct a one-player [Boolean game](../../../../../boolean-game.md) in which that player controls $X\cup\{z\}$ and has goal

$$
\gamma=z\land F(X).
$$

Choose the candidate [pure strategy](../../../../../pure-strategy.md) assigning every variable false. Its [payoff](../../../../../payoff.md) is zero because $z$ is false, regardless of $F$. If $F$ has a [satisfying assignment](../../../../../satisfying-assignment.md), changing $X$ to that assignment and $z$ to true is a profitable [unilateral deviation](../../../../../unilateral-deviation.md). If $F$ is an [unsatisfiable Boolean formula](../../../../../unsatisfiable-boolean-formula.md), no [unilateral deviation](../../../../../unilateral-deviation.md) can satisfy the goal. Therefore

$$
F\text{ is unsatisfiable}\quad\Longleftrightarrow\quad
\text{the constructed candidate is a Nash equilibrium}.
$$

The construction increases the formula length by only a constant and writes a candidate of linear length, so it is a [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md). Unsatisfiability is [co-NP](../../../../../co-np.md)-complete; combining hardness and membership proves that **candidate [Nash equilibrium](../../../../../nash-equilibrium.md) checking for [Boolean games](../../../../../boolean-game.md) is [co-NP](../../../../../co-np.md)-complete**. If a convention requires at least two players, add a player controlling a fresh unused variable and having the always-true goal; this changes neither direction of the proof.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2022](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
