<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Causal mediation analysis](../../../../../../causal-mediation-analysis.md) decomposes the [total causal effect](../../../../../../total-causal-effect.md) of an exposure into a pathway operating through a mediator and a pathway not operating through that mediator. Let $M(x)$ be the potential mediator under exposure $x$, and let $Y(x,m)$ be the potential outcome under exposure $x$ with mediator set to $m$. One conventional decomposition uses

$$
\operatorname{NDE}
=\mathbb E[Y(1,M(0))-Y(0,M(0))]
$$

for the [natural direct effect](../../../../../../natural-direct-effect.md), and

$$
\operatorname{NIE}
=\mathbb E[Y(1,M(1))-Y(1,M(0))]
$$

for the [natural indirect effect](../../../../../../natural-indirect-effect.md). In words, the direct effect changes exposure while holding the mediator at the value it would naturally have under no exposure; the indirect effect changes only that natural mediator value while holding exposure fixed at one.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
