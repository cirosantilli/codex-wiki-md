# Existential equilibrium checking in a Boolean game

↑ **Parent:** [Nash equilibrium](nash-equilibrium.md)

Given a [Boolean game](boolean-game.md) and a query [propositional formula](propositional-formula.md) $\phi$, decide whether some [pure strategy](pure-strategy.md) [Nash equilibrium](nash-equilibrium.md) satisfies $\phi$. The problem is complete for the existential [second level of the polynomial hierarchy](second-level-of-the-polynomial-hierarchy.md).

For membership, existentially choose a [Boolean valuation](boolean-valuation.md) and universally check every player's every [unilateral deviation](unilateral-deviation.md). The goal must remain false under all such deviations for each player whose goal is currently false. Each individual check takes [polynomial time](polynomial-time.md).

For hardness, start with a [two-block quantified Boolean formula](two-block-quantified-boolean-formula.md) $\exists X\forall Y\,\psi(X,Y)$. Give player 1 control of $X$ and the constant true goal. Give player 2 control of $Y$ and goal $\neg\psi$, and use $\psi$ as the query. A queried [Nash equilibrium](nash-equilibrium.md) exists exactly when some choice of $X$ leaves player 2 unable to falsify $\psi$ by changing $Y$. This is precisely the input quantified statement, and the construction is a [polynomial-time reduction](polynomial-time-reduction.md).

## ↑ Ancestors (7)

1. [Nash equilibrium](nash-equilibrium.md)
2. [Bimatrix game](bimatrix-game.md)
3. [Game theory](game-theory-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Candidate equilibrium checking in a Boolean game](candidate-equilibrium-checking-in-a-boolean-game.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2023/computational-game-theory/2/b/solution.md)
