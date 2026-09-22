# Expectimax

↑ **Parent:** [Adversarial search](adversarial-search.md)

A [game tree](game-tree.md) evaluation rule using maxima at the controlled player’s decision nodes and [expected values](expected-value-split.md) at chance nodes:

$$
V(s)=\max_a V(T(s,a)),\qquad V(s)=\sum_{s'}P(s'\mid s)V(s'),
$$

respectively. Terminal [utilities](utility.md) fix the boundary values. These rules exactly optimize a finite-horizon [expected utility](expected-utility.md) objective by [backward induction](backward-induction.md). For cyclic infinite-horizon reachability problems, a finite [Markov decision process](markov-decision-process.md) formulation and [value iteration](value-iteration.md) replace naive expansion of an infinite [game tree](game-tree.md). Start with one at successful terminal states and zero elsewhere, keep terminal values fixed, and apply the maximizing/expectation backups repeatedly. The $t$th iterate is the greatest success [probability](probability.md) achievable within $t$ transitions, by [backward induction](backward-induction.md). These values are nondecreasing and bounded by one. For every policy, eventual success is the increasing [set union](set-union.md) of success within finite horizons, so its [probability](probability.md) is the [limit](limit-of-a-function.md) of those finite-horizon [probabilities](probability.md). Taking the supremum over policies and horizons in either order proves that the iterates converge to the optimal eventual-success [probability](probability.md). The limiting fixed-point equations can also admit larger solutions, so the initialization from terminal-success indicators matters.

## ↑ Ancestors (7)

1. [Adversarial search](adversarial-search.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Adversarial search](adversarial-search.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/i/solution.md)
