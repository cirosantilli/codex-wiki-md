<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $x$, there is an accepting [graph path](../../../../../../path-in-a-graph.md)

$$
q_0\xrightarrow{1}q_1\xrightarrow{1}q_2
\xrightarrow{0}q_0\xrightarrow{0}q_0
\xrightarrow{1}q_1\xrightarrow{1}q_2
\xrightarrow{0}q_0\xrightarrow{\varepsilon}q_2.
$$

Its nonempty labels spell $1100110$, and its last [automaton state](../../../../../../automaton-state.md) is accepting. **Therefore $x$ is accepted.** The last [epsilon transition](../../../../../../epsilon-transition.md) matters: finishing the consumed input at $q_0$ does not prevent a subsequent move to $q_2$.

For $y$, track all possible [automaton states](../../../../../../automaton-state.md), including their [epsilon closure](../../../../../../epsilon-closure.md), after each input prefix:

| Input prefix | Possible [automaton states](../../../../../../automaton-state.md) after [epsilon closure](../../../../../../epsilon-closure.md) |
| --- | --- |
| $\varepsilon$ | $\{q_0,q_2\}$ |
| $1$ | $\{q_1\}$ |
| $11$ | $\{q_2\}$ |
| $110$ | $\{q_0,q_2\}$ |
| $1100$ | $\{q_0,q_2\}$ |
| $11001$ | $\{q_1\}$ |

The final [set](../../../../../../set-split.md) contains no accepting [automaton state](../../../../../../automaton-state.md), and $q_1$ has no outgoing [epsilon transition](../../../../../../epsilon-transition.md). **Therefore $y$ is rejected.**

$$
\boxed{x\in L(M),\qquad y\notin L(M).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
