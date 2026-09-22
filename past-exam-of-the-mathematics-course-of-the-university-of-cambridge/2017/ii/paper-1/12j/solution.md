<h1 id="12j/solution">Solution</h1>

↑ **Parent:** [12J](../12j.md)

Under the [binomial distribution](../../../../../binomial-distribution.md) model's assumption of independent games with a common win [probability](../../../../../probability.md) $p$, the [probability](../../../../../probability.md) of winning a match is

$$
h(p)=\sum_{j=6}^{11}\binom{11}{j}p^j(1-p)^{11-j}.
$$

This is also the [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F_{6,6}(p)$ of a [Beta distribution](../../../../../beta-distribution.md) with parameters $(6,6)$: differentiation of the binomial tail gives $h'(p)=11!\,p^5(1-p)^5/(5!)^2$, and $h(0)=0$. In particular $h$ is strictly increasing on $(0,1)$ and maps $[0,1]$ bijectively onto itself.

The new match [probability](../../../../../probability.md) is $\widetilde P_{ab}=h(P_{ab})$, while the desired linear predictor remains the game-level [log odds](../../../../../log-odds.md). Therefore the [link function](../../../../../link-function.md) is

$$
\boxed{g(u)=\log\frac{F_{6,6}^{-1}(u)}{1-F_{6,6}^{-1}(u)}},\qquad0<u<1.
$$

Its endpoint values are $-\infty$ and $+\infty$. This is not the ordinary match-level [log odds](../../../../../log-odds.md) link: it first recovers the underlying game [probability](../../../../../probability.md). Symmetry of the binomial tail gives $h(1-p)=1-h(p)$, hence $g(1-u)=-g(u)$, as required by swapping the players. Dependence or varying game probabilities within a match would invalidate the stated binomial-tail conversion.

## ↑ Ancestors (10)

1. [12J](../12j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
