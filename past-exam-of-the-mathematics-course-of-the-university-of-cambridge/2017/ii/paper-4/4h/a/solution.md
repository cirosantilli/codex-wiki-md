<h1 id="4h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [state elimination for finite automata](../../../../../../state-elimination-for-finite-automata.md) on a [generalized finite automaton](../../../../../../generalized-finite-automaton.md), whose directed [edges](../../../../../../edge-of-a-graph.md) are labelled by [regular expressions](../../../../../../regular-expression.md). Add a fresh initial state $s$ with an $\varepsilon$-edge to the old initial state and a fresh final state $f$ with $\varepsilon$-edges from all old accepting states. Every missing [edge](../../../../../../edge-of-a-graph.md) has label $\varnothing$, the [empty language](../../../../../../empty-language.md); parallel [edges](../../../../../../edge-of-a-graph.md) are merged by [union](../../../../../../set-union.md). The label $\varepsilon$ denotes the language containing just the [empty word](../../../../../../empty-word.md).

When eliminating a state $k$, replace the label on each surviving [edge](../../../../../../edge-of-a-graph.md) $i\to j$ by

$$
\boxed{R_{ij}\ \cup\ R_{ik}(R_{kk})^*R_{kj}.}
$$

Here juxtaposition means [concatenation of formal languages](../../../../../../concatenation-of-formal-languages.md), and the [Kleene star](../../../../../../kleene-star.md) allows zero or more traversals of the loop at $k$. Then delete $k$ and its incident [edges](../../../../../../edge-of-a-graph.md). Eliminate every original state; the remaining $s\to f$ label is a [regular expression](../../../../../../regular-expression.md) for exactly the accepted [formal language](../../../../../../formal-language.md). The update accounts for paths avoiding $k$ and paths entering $k$, looping there any number of times, and leaving it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4H](../../4h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
