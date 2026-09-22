<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [clique decision problem](../../../../../clique-decision-problem.md) belongs to [NP](../../../../../np-complexity.md). First reject $k>|V(G)|$. Otherwise a [complexity certificate](../../../../../certificate-complexity.md) lists $k$ distinct [vertices](../../../../../vertex-graph-theory.md). Check distinctness and test that each of the $\binom k2$ pairs is an [edge](../../../../../edge-of-a-graph.md). Under a conventional explicit [graph](../../../../../graph-split.md) encoding, the [complexity certificate](../../../../../certificate-complexity.md) length and verification [time complexity](../../../../../time-complexity.md) are [polynomial](../../../../../polynomial-split.md) in the [input](../../../../../input-computer-science.md) length. The early rejection is relevant when $k$ is given in the [binary numeral system](../../../../../binary-numeral-system.md).

For [NP-hardness](../../../../../np-hardness.md), first transform a [SAT](../../../../../boolean-satisfiability-problem.md) instance into an equisatisfiable [conjunctive normal form](../../../../../conjunctive-normal-form.md) $F=C_1\land\cdots\land C_m$ of [polynomial](../../../../../polynomial-split.md) size using a [Tseitin transformation](../../../../../tseytin-transformation.md). This step avoids the possibly exponential increase caused by distributing arbitrary [Boolean formulas](../../../../../boolean-formula.md) into [conjunctive normal form](../../../../../conjunctive-normal-form.md). Introduce a fresh [Boolean variable](../../../../../boolean-variable.md) for each subformula, constrain it to have the connective's [truth value](../../../../../truth-value.md) using a constant number of [Boolean clauses](../../../../../clause-of-a-boolean-formula.md), and require the top variable to be true. A [Boolean valuation](../../../../../boolean-valuation.md) of the original [Boolean variables](../../../../../boolean-variable.md) satisfies the original [Boolean formula](../../../../../boolean-formula.md) exactly when it extends to a [satisfying assignment](../../../../../satisfying-assignment.md) of these constraints.

Create one [vertex](../../../../../vertex-graph-theory.md) for each occurrence of a [Boolean literal](../../../../../boolean-literal.md) in each [Boolean clause](../../../../../clause-of-a-boolean-formula.md). Join two such [vertices](../../../../../vertex-graph-theory.md) by an [edge](../../../../../edge-of-a-graph.md) exactly when they belong to different [Boolean clauses](../../../../../clause-of-a-boolean-formula.md) and their [Boolean literals](../../../../../boolean-literal.md) are not a variable and its [logical negation](../../../../../negation.md). Set $k=m$. There are at most as many [vertices](../../../../../vertex-graph-theory.md) as [Boolean literal](../../../../../boolean-literal.md) occurrences and at most quadratically many [edges](../../../../../edge-of-a-graph.md), so this construction takes [polynomial time](../../../../../polynomial-time.md).

If $F$ has a [satisfying assignment](../../../../../satisfying-assignment.md), choose one true [Boolean literal](../../../../../boolean-literal.md) occurrence from each [Boolean clause](../../../../../clause-of-a-boolean-formula.md). No two selected [Boolean literals](../../../../../boolean-literal.md) are contradictory, so their $m$ [vertices](../../../../../vertex-graph-theory.md) form a [clique](../../../../../clique-graph-theory.md). Conversely, an $m$-[clique](../../../../../clique-graph-theory.md) contains at most one [vertex](../../../../../vertex-graph-theory.md) from each [Boolean clause](../../../../../clause-of-a-boolean-formula.md), because there are no [edges](../../../../../edge-of-a-graph.md) within a [Boolean clause](../../../../../clause-of-a-boolean-formula.md). It therefore selects exactly one occurrence from each of the $m$ [Boolean clauses](../../../../../clause-of-a-boolean-formula.md). The selected [Boolean literals](../../../../../boolean-literal.md) are pairwise noncontradictory, so assign their [Boolean variables](../../../../../boolean-variable.md) the indicated [truth values](../../../../../truth-value.md) and assign any other [Boolean variables](../../../../../boolean-variable.md) arbitrarily. This [Boolean valuation](../../../../../boolean-valuation.md) satisfies every [Boolean clause](../../../../../clause-of-a-boolean-formula.md).

An empty [Boolean clause](../../../../../clause-of-a-boolean-formula.md) gives no [vertex](../../../../../vertex-graph-theory.md) in its group, correctly preventing an $m$-[clique](../../../../../clique-graph-theory.md). An empty [logical conjunction](../../../../../logical-conjunction.md) can instead be mapped to a fixed yes-instance, avoiding any convention about $k=0$. Malformed [SAT](../../../../../boolean-satisfiability-problem.md) descriptions can be mapped to a fixed no-instance. We have proved

$$
F\text{ satisfiable}\quad\Longleftrightarrow\quad
\langle G_F,m\rangle\in\mathrm{Clique},
\qquad
\boxed{\mathrm{Clique}\text{ is NP-complete}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
