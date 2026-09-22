# 2-satisfiability

↑ **Parent:** [Boolean satisfiability problem](boolean-satisfiability-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/2-satisfiability)

[2-satisfiability](2-satisfiability.md) restricts [SAT](boolean-satisfiability-problem.md) to [CNF](conjunctive-normal-form.md) in which each [Boolean clause](clause-of-a-boolean-formula.md) has at most two [Boolean literals](boolean-literal.md). The example in [Boolean satisfiability problem](boolean-satisfiability-problem.md) is therefore a [2-SAT](2-satisfiability.md) instance. Unlike general [SAT](boolean-satisfiability-problem.md) and [3-SAT](3-sat.md), [2-SAT](2-satisfiability.md) has a [polynomial-time algorithm](polynomial-time-algorithm.md); its tractability concerns finding a [satisfying assignment](satisfying-assignment.md) or deciding that none exists, not merely checking a candidate. [3-SAT](3-sat.md) allows up to three [Boolean literals](boolean-literal.md) per [Boolean clause](clause-of-a-boolean-formula.md) and is [NP-complete](np-completeness.md), even though it includes many individually easy instances such as this one.[CS 252, Lecture 8: Constraint Satisfaction Problems, pp. 1–2, §2 examples 1 and 3; p. 3, §3 classification items 1 and 3](cs-252-lecture-8-constraint-satisfaction-problems-carnegie-mellon-university.md)

The key [logical equivalence](logical-equivalence.md) is

$$
a\lor b\equiv(\neg a\to b)\land(\neg b\to a),
$$

where $a,b$ are [Boolean literals](boolean-literal.md). It expresses a two-[Boolean literal](boolean-literal.md) [Boolean clause](clause-of-a-boolean-formula.md) as two [logical implications](logical-implication.md). Representing these [logical implications](logical-implication.md) as edges in a [directed graph](directed-graph.md) gives a route to the [polynomial-time algorithm](polynomial-time-algorithm.md). In the example, $C_2$ says both $x\to z$ and $\neg z\to\neg x$: enabling the feature requires its component, and an absent component excludes the feature.

## ↑ Ancestors (9)

1. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
2. [NP-completeness](np-completeness.md)
3. [NP-hardness](np-hardness.md)
4. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
5. [Polynomial-time reduction](polynomial-time-reduction.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science-split.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [2-satisfiability](2-satisfiability.md)
