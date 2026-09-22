<h1 id="30k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define

$$
H_n=
\begin{cases}
1,&n\leq T_a,\\
-1,&n>T_a.
\end{cases}
$$

The event $\{n\leq T_a\}$ means that level $a$ has not been reached by time $n-1$, so it belongs to $\mathcal F_{n-1}$. Hence $H$ is a bounded [predictable process](../../../../../../predictable-process.md). A direct check across the hitting time gives

$$
\widehat X_n-\widehat X_{n-1}
=H_n(X_n-X_{n-1}),
$$

and therefore

$$
\widehat X_n=\sum_{k=1}^nH_k(X_k-X_{k-1}).
$$

Part (c) shows that $\widehat X$ is a martingale. Its increments still take values in $\{-1,1\}$, so part (b) shows that they are IID symmetric signs. Consequently $\widehat X$ is a simple symmetric random walk. This is the path transformation behind the [reflection principle for simple symmetric random walk](../../../../../../reflection-principle-for-simple-symmetric-random-walk.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
