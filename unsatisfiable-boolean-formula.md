# Unsatisfiable Boolean formula

↑ **Parent:** [Boolean satisfiability problem](boolean-satisfiability-problem.md)

An [unsatisfiable Boolean formula](unsatisfiable-boolean-formula.md) has no [satisfying assignment](satisfying-assignment.md). For

$$
G=x\land\neg x,
$$

the [Boolean valuation](boolean-valuation.md) $x=0$ falsifies the first [Boolean clause](clause-of-a-boolean-formula.md), and $x=1$ falsifies the second. Both possible [truth values](truth-value.md) fail, proving `UNSAT`. Each [Boolean clause](clause-of-a-boolean-formula.md) alone has a [satisfying assignment](satisfying-assignment.md), but their [logical conjunction](logical-conjunction.md) does not: compatibility is the central issue. By contrast, finding just one failed [Boolean valuation](boolean-valuation.md) for a general [Boolean formula](boolean-formula.md) only rejects that candidate. Finding one successful [Boolean valuation](boolean-valuation.md) proves `SAT`; proving `UNSAT` requires excluding every candidate, possibly with a compact argument rather than a full [truth table](truth-table.md).

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

## ← Incoming links (10)

- [Boolean satisfiability problem](boolean-satisfiability-problem.md)
- [Candidate equilibrium checking in a Boolean game](candidate-equilibrium-checking-in-a-boolean-game.md)
- [Conjunctive normal form](conjunctive-normal-form.md)
- [Equivalence of weighted formula utility representations](equivalence-of-weighted-formula-utility-representations.md)
- [Partial Boolean assignment](partial-boolean-assignment.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/2/d/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/2/c/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2023/computational-game-theory/1/c/solution.md)
- [Semantic entailment](semantic-entailment.md)
- [Unsatisfiable Boolean formula](unsatisfiable-boolean-formula.md)
