<h1 id="28k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\nu$ be an [invariant distribution](../../../../../../stationary-distribution.md) for the [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md). Using $Q=D_g(P-I)$, its [stationarity equation](../../../../../../invariant-distribution-of-a-continuous-time-markov-chain.md) $\nu Q=0$ becomes

$$
(\nu D_g)P=\nu D_g.
$$

Thus the measure with weights $\nu_i g(i)$ is invariant for the irreducible positive-recurrent [jump chain](../../../../../../jump-chain.md). Its [invariant distribution](../../../../../../stationary-distribution.md) $\pi$ is unique, so $\nu_i g(i)=c\pi_i$. Normalization gives the [invariant-measure transfer between a jump chain and a CTMC](../../../../../../invariant-measure-transfer-between-a-jump-chain-and-a-ctmc.md) formula

$$
\boxed{\nu_i=\frac{\pi_i/g(i)}{\displaystyle\sum_{j\in S}\pi_j/g(j)}}.
$$

The denominator is finite and nonzero because $\varepsilon<g(j)<1/\varepsilon$. Thus $\nu$ is a [probability distribution](../../../../../../probability-distribution.md) and $(X_t)$ is positive recurrent.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
