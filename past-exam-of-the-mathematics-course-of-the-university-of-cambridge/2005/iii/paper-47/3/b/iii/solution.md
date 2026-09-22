<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $0\leq p\leq1$. Draw an [independent](../../../../../../../independent-random-variables.md) component indicator with a [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) of success [probability](../../../../../../../probability.md) $p$. On success, generate the [normal distribution](../../../../../../../normal-distribution.md) from part (i) and return its absolute value; this has the [half-normal distribution](../../../../../../../half-normal-distribution.md) [probability density function](../../../../../../../probability-density-function.md) $2f(x)$ on $x\geq0$. On failure, generate the [Weibull distribution](../../../../../../../weibull-distribution.md) from part (ii). Use fresh [independent](../../../../../../../independent-random-variables.md) uniforms for the chosen component.

The law of total [probability](../../../../../../../probability.md) gives the output [probability density function](../../../../../../../probability-density-function.md)

$$
\boxed{p\,2f(x)+(1-p)g(x)\quad(x\geq0),}
$$

as required. The factor two belongs inside the half-normal component; the [probability](../../../../../../../probability.md) of choosing that component is $p$, not $2p$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
