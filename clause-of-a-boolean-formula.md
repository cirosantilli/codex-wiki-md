# Clause of a Boolean formula

↑ **Parent:** [Boolean formula](boolean-formula.md)

A [Boolean clause](clause-of-a-boolean-formula.md) is an expression $\ell_1\lor\cdots\lor\ell_k$ formed from [Boolean literals](boolean-literal.md), true when at least one [Boolean literal](boolean-literal.md) is true. The empty [Boolean clause](clause-of-a-boolean-formula.md) is false. Repeating a [Boolean literal](boolean-literal.md) does not change the [truth value](truth-value.md). A [CNF](conjunctive-normal-form.md) [Boolean formula](boolean-formula.md) is a [logical conjunction](logical-conjunction.md) of these [Boolean clauses](clause-of-a-boolean-formula.md).

For $(\neg x\lor z)$, the only failing pair is $(x,z)=(1,0)$: its two [Boolean literals](boolean-literal.md) then both have [truth value](truth-value.md) zero. The one-[Boolean literal](boolean-literal.md) [Boolean clause](clause-of-a-boolean-formula.md) $(x)$ requires $x=1$. A [Boolean clause](clause-of-a-boolean-formula.md) containing both $x$ and $\neg x$ is a [tautology](tautology.md), since one of those [Boolean literals](boolean-literal.md) is true under every [Boolean valuation](boolean-valuation.md). These observations separate [Boolean clause](clause-of-a-boolean-formula.md) satisfaction from the simultaneous satisfaction required by [SAT](boolean-satisfiability-problem.md).

## ↑ Ancestors (10)

1. [Boolean formula](boolean-formula.md)
2. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
3. [NP-completeness](np-completeness.md)
4. [NP-hardness](np-hardness.md)
5. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
6. [Polynomial-time reduction](polynomial-time-reduction.md)
7. [Computational complexity theory](computational-complexity-theory.md)
8. [Theoretical computer science](theoretical-computer-science-split.md)
9. [Computer science](computer-science-split.md)
10. [Codex Wiki](split.md)
