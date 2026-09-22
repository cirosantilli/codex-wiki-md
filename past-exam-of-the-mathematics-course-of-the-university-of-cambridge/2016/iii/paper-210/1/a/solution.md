<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each ball, the event of landing in $S_j$ is a [Bernoulli distribution](../../../../../../bernoulli-distribution.md) trial. Under the [null hypothesis](../../../../../../null-hypothesis.md) its [probability](../../../../../../probability.md) is $\varepsilon$. Under the selected alternative $Q_j$, its [probability](../../../../../../probability.md) is $p_1=\pi+(1-\pi)\varepsilon=\varepsilon+\pi(1-\varepsilon)$. The placements are [independent random variables](../../../../../../independent-random-variables.md) conditional on that selected index, so the count has the [binomial distribution](../../../../../../binomial-distribution.md):

$$
\boxed{c_j\sim\operatorname{Bin}(n,\varepsilon)\text{ under }P_0,\qquad c_j\sim\operatorname{Bin}(n,\varepsilon+\pi(1-\varepsilon))\text{ under }Q_j.}
$$

The second assertion concerns $Q_j$, rather than the unconditional [mixture model](../../../../../../mixture-model.md) $P_1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
