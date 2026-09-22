# Equivalence of weighted formula utility representations

↑ **Parent:** [Computational complexity theory](computational-complexity-theory.md)

Given two [weighted formula utility representations](weighted-formula-utility-representation.md) with binary [rational numbers](rational-number.md) as weights, decide whether their values agree on every [Boolean valuation](boolean-valuation.md). This problem is [co-NP](co-np.md)-complete.

For membership, a valuation witnessing unequal values certifies non-equivalence. Evaluate all [propositional formulas](propositional-formula.md) and add their weights exactly in [polynomial time](polynomial-time.md). For hardness, compare the one-rule base $\{(\theta,1)\}$ with the empty base. They are equivalent exactly when $\theta$ is an [unsatisfiable Boolean formula](unsatisfiable-boolean-formula.md). Thus even very small weighted rule bases express a universal equivalence question.

## ↑ Ancestors (4)

1. [Computational complexity theory](computational-complexity-theory.md)
2. [Theoretical computer science](theoretical-computer-science-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
