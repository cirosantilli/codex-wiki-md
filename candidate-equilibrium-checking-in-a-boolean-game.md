# Candidate equilibrium checking in a Boolean game

↑ **Parent:** [Boolean game](boolean-game.md)

Given a succinct [Boolean game](boolean-game.md) and a complete [pure strategy](pure-strategy.md) [strategy profile](strategy-profile.md), determine whether it is a [Nash equilibrium](nash-equilibrium.md). The problem is [co-NP](co-np.md)-complete for goal [propositional formulas](propositional-formula.md), even with one player. This differs from [existential equilibrium checking in a Boolean game](existential-equilibrium-checking-in-a-boolean-game.md), which searches for some qualifying [Nash equilibrium](nash-equilibrium.md).

A negative instance has a short [complexity certificate](certificate-complexity.md): a currently unsatisfied player and new truth values for that player's controlled [Boolean variables](boolean-variable.md) that make the goal true. Evaluating the current and changed [propositional formulas](propositional-formula.md) takes [polynomial time](polynomial-time.md), proving membership in [co-NP](co-np.md).

For hardness, given a [propositional formula](propositional-formula.md) $F(X)$, let one player control $X$ and a fresh variable $z$, with goal $z\land F(X)$. The all-false candidate has [payoff](payoff.md) zero. It is a [Nash equilibrium](nash-equilibrium.md) exactly when $F$ is an [unsatisfiable Boolean formula](unsatisfiable-boolean-formula.md), since any [satisfying assignment](satisfying-assignment.md) permits an improvement by also setting $z$ true. This is a [polynomial-time many-one reduction](polynomial-time-many-one-reduction.md) from unsatisfiability. The fresh guard ensures that the candidate loses independently of the input formula's value there.

## ↑ Ancestors (6)

1. [Boolean game](boolean-game.md)
2. [Game theory](game-theory-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/2/c/solution.md)
