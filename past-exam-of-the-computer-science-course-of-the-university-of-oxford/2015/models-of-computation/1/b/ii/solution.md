<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [state elimination for finite automata](../../../../../../state-elimination-for-finite-automata.md), with [regular expression](../../../../../../regular-expression.md) labels on a [generalized finite automaton](../../../../../../generalized-finite-automaton.md). Add a fresh initial [automaton state](../../../../../../automaton-state.md) $s$ with $s\xrightarrow{\varepsilon}q_0$, and a fresh final [automaton state](../../../../../../automaton-state.md) $f$ with $q_2\xrightarrow{\varepsilon}f$. Only $f$ is now accepting. Missing labels represent the [empty language](../../../../../../empty-language.md), and parallel alternatives are combined by [union](../../../../../../set-union.md).

When eliminating an internal [automaton state](../../../../../../automaton-state.md) $k$, update every surviving label by

$$
R_{ij}\longleftarrow R_{ij}\cup R_{ik}(R_{kk})^*R_{kj}.
$$

The added [regular expression](../../../../../../regular-expression.md) describes entering $k$, traversing its loop zero or more times by [Kleene star](../../../../../../kleene-star.md), and leaving it. This accounts for exactly the [graph paths](../../../../../../path-in-a-graph.md) newly bypassing $k$.

First eliminate $q_1$. Its only incoming and outgoing labels are both $1$, and it has no loop. The [graph path](../../../../../../path-in-a-graph.md) through it contributes $11$, so the label from $q_0$ to $q_2$ becomes

$$
R_{02}=\varepsilon\cup11.
$$

The other relevant labels are still $R_{00}=0$, $R_{20}=0$, and $R_{2f}=\varepsilon$.

Next eliminate $q_2$. It has no loop, so the new loop at $q_0$ and the new label to $f$ are

$$
\begin{aligned}
R_{00}&=0\cup(\varepsilon\cup11)0=0\cup110,\\
R_{0f}&=(\varepsilon\cup11)\varepsilon=\varepsilon\cup11.
\end{aligned}
$$

Finally eliminate $q_0$. The label from $s$ to $f$ is

$$
\varepsilon(0\cup110)^*(\varepsilon\cup11).
$$

Thus an equivalent [regular expression](../../../../../../regular-expression.md) is

$$
\boxed{(0\cup110)^*(\varepsilon\cup11).}
$$

For an independent interpretation, every completed return to $q_0$ consumes either $0$ or $110$: the latter traverses $q_1,q_2$ before returning. The last visit to $q_2$ consumes either nothing or $11$. Consequently every run of ones has length exactly two, and successive such runs require at least one zero between them. In particular, consecutive copies of $11$ without a separating zero are not accepted.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
