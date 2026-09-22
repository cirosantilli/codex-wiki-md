<h1 id="27j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the natural [filtration](../../../../../../filtration-probability-theory.md) $\mathcal F_t=\sigma(X_s:0\leq s\leq t)$, a nonnegative random time $\tau$ is a [stopping time](../../../../../../stopping-time.md) when $\{\tau\leq t\}\in\mathcal F_t$ for every $t\geq0$: whether it has occurred can be decided from the observations already made.

For a time-homogeneous finite-state continuous-time [Markov chain](../../../../../../markov-chain.md), the [Strong Markov property](../../../../../../strong-markov-property.md) says that, on $\{\tau<\infty\}$, conditional on $\mathcal F_\tau$, the process $(X_{\tau+s})_{s\geq0}$ has the law of a fresh chain started at $X_\tau$ and is independent of the earlier history given that state. In particular, with transition matrix $P_s=e^{sQ}$,

$$
\boxed{\mathbb E[f(X_{\tau+s})\mid\mathcal F_\tau]=(P_sf)(X_\tau)\quad\text{on }\{\tau<\infty\}.}
$$

The property applies also to bounded functions of several future times or of the entire future path.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [27J](../../27j.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
