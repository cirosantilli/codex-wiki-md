<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**The difficulty is representing dictionary membership and the one-letter relationship in positive conjunctive [STRIPS](../../../../../strips.md) [preconditions](../../../../../precondition.md); a finite dictionary nevertheless admits an exact encoding.** Pure [STRIPS](../../../../../strips.md) does not provide string indexing, a “differs in one position” operator, arbitrary disjunctive tests or a procedure that calls a dictionary lookup. Those relationships must be represented by ground facts or compiled into [ground actions](../../../../../ground-action.md).

One exact whole-word encoding uses a [planning fluent](../../../../../planning-fluent.md) $\operatorname{At}(w)$ and a [static predicate](../../../../../static-predicate.md) $\operatorname{Next}(w,w')$ containing exactly the permitted dictionary mutations. For the [action schema](../../../../../action-schema.md) $\operatorname{Change}(w,w')$, use

$$
\begin{aligned}
\operatorname{Pre}&=\{\operatorname{At}(w),\operatorname{Next}(w,w')\},\\
\operatorname{Add}&=\{\operatorname{At}(w')\},\\
\operatorname{Del}&=\{\operatorname{At}(w)\}.
\end{aligned}
$$

Initialize $\operatorname{At}(s)$ and the static transition facts, and use goal $\operatorname{At}(t)$. Only one $\operatorname{At}$ fact is true initially. Each applicable [ground action](../../../../../ground-action.md) deletes it and adds exactly its permitted successor, so [mathematical induction](../../../../../mathematical-induction.md) proves that exactly one current-word fact remains true and that every [plan](../../../../../plan.md) is a legal [word ladder](../../../../../word-ladder.md). Conversely, every legal [word ladder](../../../../../word-ladder.md) directly supplies a [plan](../../../../../plan.md). An isolated non-dictionary start is handled as in (c). A shortest [plan](../../../../../plan.md) has the fewest mutations.

This encoding moves the hard lexical relationship into preprocessing. For $N$ dictionary words, checking all ordered pairs takes $O(N^2L)$ character comparisons, although indexing can do better; the number of stored transitions is at most $N L(|\Sigma|-1)$ when all states are dictionary words. The [STRIPS](../../../../../strips.md) representation is finite, but its size and preprocessing cost matter.

A position-based representation instead uses [planning fluents](../../../../../planning-fluent.md) $\operatorname{Letter}(i,\ell)$. Changing position $i$ must delete its old letter and add its new one; all other positions persist through the [STRIPS](../../../../../strips.md) update rule. Merely requiring each position to contain a letter admits non-dictionary strings. A disjunction over all dictionary words is not a positive conjunctive [STRIPS](../../../../../strips.md) [precondition](../../../../../precondition.md). It can be compiled into separate [ground actions](../../../../../ground-action.md), each requiring every letter of a valid source word and changing one position to reach a valid destination. This again enumerates lexical cases and can be large. Arbitrary letter changes followed by an unconstrained “validate” action are unsound: several illegal intermediate strings could otherwise lead to a legal goal. Legality must hold after every mutation, not only at the endpoint.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
