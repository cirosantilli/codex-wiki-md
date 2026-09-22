<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**A loop-free [induced subgraph game](../../../../../induced-subgraph-game.md) is a [convex cooperative game](../../../../../convex-cooperative-game.md) if and only if every [edge weight](../../../../../edge-weight.md) is nonnegative.** Necessity follows by applying the [supermodular](../../../../../supermodular-set-function.md) inequality to $S=\{i\}$ and $T=\{j\}$. Since both singleton values and the empty value are zero,

$$
v(\{i,j\})+v(\varnothing)\ge v(\{i\})+v(\{j\})
\quad\Longrightarrow\quad w_{ij}\ge0.
$$

Conversely, direct cancellation of common [edge](../../../../../edge-of-a-graph.md) contributions gives, for any [coalitions](../../../../../coalition-game-theory.md) $S,T$,

$$
v(S\cup T)+v(S\cap T)-v(S)-v(T)
=\sum_{\substack{i\in S\setminus T\\j\in T\setminus S}}w_{ij}.
$$

Every summand is nonnegative, proving that $v$ is a [supermodular set function](../../../../../supermodular-set-function.md) and hence convexity. Equivalently, a player's [marginal contribution](../../../../../marginal-contribution.md) to $S$ is $\Delta_i(S)=\sum_{j\in S}w_{ij}$, which cannot decrease as $S$ grows. This establishes the [convexity criterion for an induced subgraph game](../../../../../convexity-criterion-for-an-induced-subgraph-game.md) directly.[§1, printed p. 258, nonnegative-weight convexity; §2.2, printed p. 260, discussion preceding Lemma 4](../../../../../on-the-complexity-of-cooperative-solution-concepts-by-xiaotie-deng-and-christos-papadimitriou.md)

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
