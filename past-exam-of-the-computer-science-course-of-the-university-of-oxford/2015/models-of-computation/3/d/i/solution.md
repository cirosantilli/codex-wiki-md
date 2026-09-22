<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The problem is decidable.** We need exactly one accepted [word](../../../../../../string.md), even if that [word](../../../../../../string.md) has several accepting runs in the [nondeterministic finite automaton](../../../../../../nondeterministic-finite-automaton.md).

First convert the input [nondeterministic finite automaton](../../../../../../nondeterministic-finite-automaton.md) to an equivalent [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) $D$ using the [subset construction](../../../../../../subset-construction-with-epsilon-transitions.md), taking [epsilon closure](../../../../../../epsilon-closure.md) where necessary. In the finite transition [directed graph](../../../../../../directed-graph.md) of $D$, test whether an accepting [automaton state](../../../../../../automaton-state.md) is reachable from the initial [automaton state](../../../../../../automaton-state.md). This is the standard [finite automaton emptiness test](../../../../../../finite-automaton-emptiness-test.md). If none is reachable, the recognized [formal language](../../../../../../formal-language.md) is empty, so answer no.

Otherwise retain a [graph path](../../../../../../path-in-a-graph.md) to an accepting [automaton state](../../../../../../automaton-state.md) and read its labels to obtain one accepted [word](../../../../../../string.md) $w$. If the initial [automaton state](../../../../../../automaton-state.md) is accepting, $w$ may be the [empty word](../../../../../../empty-word.md). Build a complete [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) for the [singleton](../../../../../../singleton-mathematics.md) [formal language](../../../../../../formal-language.md) $\{w\}$: it tracks the matching prefix of $w$, accepts only after exactly its full length, and enters a rejecting sink on a mismatch or any extra input symbol.

Complement that complete [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) by exchanging accepting and rejecting [automaton states](../../../../../../automaton-state.md). Form its product with $D$, accepting exactly when the $D$ coordinate accepts and the other coordinate accepts. This product recognizes

$$
L(D)\cap(\Sigma^*\setminus\{w\})=L(D)\setminus\{w\}.
$$

Apply the [finite automaton emptiness test](../../../../../../finite-automaton-emptiness-test.md) again. **Answer yes if and only if this difference is empty.** The first test guarantees that $w$ belongs to $L(D)$; the second guarantees there is no different accepted [word](../../../../../../string.md). All constructions have finitely many [automaton states](../../../../../../automaton-state.md) and all reachability tests terminate. This gives a [singleton-language test for finite automata](../../../../../../singleton-language-test-for-finite-automata.md).

$$
\boxed{\text{Decidable: test }L(D)\ne\varnothing\text{ and }L(D)\setminus\{w\}=\varnothing.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
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
