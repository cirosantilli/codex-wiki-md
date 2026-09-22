<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The translation gives a sound and complete route through an optimized [SAT solver](../../../../../sat-solver.md); it trades access to general-purpose [SAT](../../../../../boolean-satisfiability-problem.md) machinery against encoding cost and the possible loss of constraint-specific structure.** Modern [SAT solvers](../../../../../sat-solver.md) use efficient [unit propagation](../../../../../unit-propagation.md), adaptive branching and [clause learning](../../../../../clause-learning.md). Learned [Boolean clauses](../../../../../clause-of-a-boolean-formula.md) can summarize conflicts involving many original [variables](../../../../../variable-mathematics.md), allowing later branches to avoid repeating the same failed combination. The reduction also offers a standard, reusable interface: improvements to a [SAT solver](../../../../../sat-solver.md) can benefit many finite-domain [constraint satisfaction problems](../../../../../constraint-satisfaction-problem.md).

The [Boolean formula](../../../../../boolean-formula.md) may be much larger than the original [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md), especially for a succinct high-arity relation. One original [variable](../../../../../variable-mathematics.md) becomes many indicators, and general branching may lose the interpretation that the [minimum remaining values](../../../../../minimum-remaining-values.md) and [degree heuristic](../../../../../degree-heuristic.md) exploit directly. Native [constraint propagation](../../../../../constraint-propagation.md) can exploit a relation without enumerating all its forbidden tuples. Even in the binary case, stronger propagation does not follow just from switching to [SAT](../../../../../boolean-satisfiability-problem.md).

For example, take $D_X=\{1,2\}$, $D_Y=\{a,b,c\}$, and let the only allowed pairs be $(1,c),(2,a),(2,b)$. The forbidden-pair encoding contains $\neg p_{X,1}\lor\neg p_{Y,a}$ and $\neg p_{X,1}\lor\neg p_{Y,b}$. If $p_{Y,c}$ becomes false, [arc consistency](../../../../../arc-consistency.md) deletes $X=1$ because it has no support. Yet the direct encoding has no unit [Boolean clause](../../../../../clause-of-a-boolean-formula.md) forcing $\neg p_{X,1}$: both $a,b$ remain possible individually, so plain [unit propagation](../../../../../unit-propagation.md) does not make that deletion. A [SAT solver](../../../../../sat-solver.md) can eventually derive it through additional reasoning or search. Conversely, [clause learning](../../../../../clause-learning.md) can combine information beyond the local consistency enforced by [AC-3](../../../../../ac-3.md). **Neither approach uniformly dominates:** performance depends on representation, propagation strength and the instance's structure; both still face exponential worst-case search on general inputs.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
