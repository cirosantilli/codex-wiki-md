# Mixed and behavioural security levels without perfect recall

↑ **Parent:** [Behavioural strategy](behavioural-strategy.md)

Consider a [zero-sum game](zero-sum-game.md) in which a player chooses a binary action, forgets it, and chooses again, while an opponent makes one hidden binary choice. The first player's [payoff](payoff.md) is one if all three choices agree and zero otherwise. The later [information set](information-set.md) merges both initial-action histories. This violates [perfect recall](perfect-recall.md) without revisiting the same [information set](information-set.md), unlike an [absent-minded decision problem](absent-minded-decision-problem.md).

A [behavioural strategy](behavioural-strategy.md) chooses the first and second actions with [independent](independent-random-variables.md) left [probabilities](probability.md) $p,r$. Its [security level payoff](security-level-payoff.md) is $\min(pr,(1-p)(1-r))$, since the opponent selects the less favorable target action. This minimum is at most $\sqrt{p(1-p)r(1-r)}\le1/4$, attained at $p=r=1/2$.

A [mixed strategy](mixed-strategy.md) instead samples the all-left or all-right complete plan with equal [probabilities](probability.md), guaranteeing $1/2$. Against an opponent who chooses each target equally often, each complete constant plan earns $1/2$ and each nonconstant plan earns zero, so no [mixed strategy](mixed-strategy.md) can guarantee more. The separation comes from correlation between a sampled plan's actions; fresh [independent](independent-random-variables.md) randomizations cannot retain it after the initial action is forgotten.

## ↑ Ancestors (6)

1. [Behavioural strategy](behavioural-strategy.md)
2. [Game theory](game-theory-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/3/a/solution.md)
