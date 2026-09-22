<h1 id="11h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

From the decoded [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md), retain only productive states: those reachable from the initial state and from which an accepting state is reachable. Both [sets](../../../../../../set-split.md) are computable by finite [graph search](../../../../../../graph-search.md). Its [regular language](../../../../../../regular-language.md) is infinite precisely when this productive directed graph contains a directed cycle.

Indeed, a cycle on a route from the start to acceptance can be repeated arbitrarily often, giving accepted words of different lengths. Conversely an accepted path of length at least the number of productive states repeats one such state and gives a productive cycle. Therefore absence of cycles bounds every accepted length strictly below that number. Cycle detection is a finite algorithm, proving that **finiteness of the accepted language is decidable**.

When it is finite, enumerate every word of length less than the number of states and simulate acceptance, then count the accepted words. This includes the empty word. Alternatively use dynamic programming in the productive acyclic graph:

$$
N(q)=\mathbf1_{\{q\text{ accepting}\}}+
\sum_{a:\delta(q,a)\text{ productive}}N(\delta(q,a)).
$$

Distinct alphabet symbols count distinct words even when their transitions share a destination. The result is $N(q_0)$, or zero if the start state is not productive. Validity of the encoding is checked first, so the [set](../../../../../../set-split.md) of valid finite-language codes is [recursive set](../../../../../../computable-set.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11H](../../11h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
