<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A proposed assignment for [2UN-SAT](../../../../../../2un-sat.md) can be checked in [polynomial time](../../../../../../polynomial-time.md), including checking the syntactic restriction, so the language belongs to [NP](../../../../../../np-complexity.md).

For an explicit reduction, parse any [Boolean formula](../../../../../../boolean-formula.md) into a [Boolean circuit](../../../../../../boolean-circuit.md) over binary AND ([logical conjunction](../../../../../../logical-conjunction.md)), binary OR ([logical disjunction](../../../../../../logical-disjunction.md)) and unary NOT ([negation](../../../../../../negation.md)), and apply the gate equivalences in part (a), asserting its output. Every gate [clause](../../../../../../clause-of-a-boolean-formula.md) has at most two positive [literals](../../../../../../boolean-literal.md): the AND [clauses](../../../../../../clause-of-a-boolean-formula.md) have respectively one, one and one; the OR [clauses](../../../../../../clause-of-a-boolean-formula.md) have one, one and two; and the NOT [clauses](../../../../../../clause-of-a-boolean-formula.md) have two and zero. The unit output/constant [clauses](../../../../../../clause-of-a-boolean-formula.md) also obey the restriction. Hence the resulting formula is an instance of [2UN-SAT](../../../../../../2un-sat.md).

The [Tseitin transformation](../../../../../../tseytin-transformation.md) is linear in the gate description, and its auxiliary variables enforce the gate values rather than relaxing their relation to the inputs. Therefore the original formula is satisfiable if and only if the transformed restricted formula is satisfiable. This is a [polynomial-time many-one reduction](../../../../../../polynomial-time-many-one-reduction.md) from [SAT](../../../../../../boolean-satisfiability-problem.md), whose hardness follows from the [Cook-Levin theorem](../../../../../../cook-levin-theorem.md). Consequently

$$
\boxed{\mathrm{2UN\text{-}SAT}\text{ is NP-complete}}.
$$

The condition limits positive [literals](../../../../../../boolean-literal.md), without limiting total [clause](../../../../../../clause-of-a-boolean-formula.md) length.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
