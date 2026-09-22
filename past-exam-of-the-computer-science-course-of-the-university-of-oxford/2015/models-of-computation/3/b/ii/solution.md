<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The [formal language](../../../../../../formal-language.md) is not a [regular language](../../../../../../regular-language.md).** Let $K$ denote it and consider the infinitely many prefixes

$$
u_i=(ab)^i,\qquad i\geq0.
$$

For any $i\ne j$, append the [word](../../../../../../string.md) $z_i=(bc)^i$. Then $u_iz_i\in K$, whereas $u_jz_i\notin K$: the latter [word](../../../../../../string.md) has $j$ occurrences of $a$ and $i$ occurrences of $c$, and every [word](../../../../../../string.md) of $K$ has equal numbers of those two symbols.

Thus $u_i$ and $u_j$ are not [Myhill-Nerode equivalent](../../../../../../myhill-nerode-equivalence.md). There are infinitely many [Myhill-Nerode equivalence](../../../../../../myhill-nerode-equivalence.md) classes, so the [Myhill-Nerode theorem](../../../../../../myhill-nerode-theorem.md) rules out a [finite-state automaton](../../../../../../finite-state-machine.md) recognizing $K$. Equivalently, if two such prefixes left a [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) in the same [automaton state](../../../../../../automaton-state.md), appending $z_i$ could not distinguish their acceptance, giving the same contradiction.

$$
\boxed{K\text{ is not regular}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
