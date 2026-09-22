<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [regular language](../../../../../regular-language.md) over a finite [alphabet](../../../../../alphabet.md) is a [formal language](../../../../../formal-language.md) recognized by a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md); equivalently it is described by a [regular expression](../../../../../regular-expression.md). A [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md) accepts an input [string](../../../../../string.md) if at least one permitted computation consumes that [string](../../../../../string.md) and reaches an accepting state. The connection is the equivalence

$$
\boxed{L\text{ is regular}\iff L\text{ is recognized by some nondeterministic finite automaton}.}
$$

Every [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) is a special case of a [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md). Conversely, the [subset construction](../../../../../subset-construction-with-epsilon-transitions.md) makes a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) whose states record the [set](../../../../../set-split.md) of all possible current states of a [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md). After each input symbol, update that [set](../../../../../set-split.md) by taking all permitted transitions, also including any [epsilon closure](../../../../../epsilon-closure.md). A new state is accepting exactly when it contains an old accepting state. A finite state [set](../../../../../set-split.md) has finitely many [subsets](../../../../../subset.md), so this really is a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) recognizing the same [formal language](../../../../../formal-language.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
