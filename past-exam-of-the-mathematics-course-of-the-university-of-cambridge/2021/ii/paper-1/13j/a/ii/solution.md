<h1 id="13j/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let

$$
N_g=Y_{gB}+Y_{gW}
$$

and condition on $N_g=n_g$. The corresponding model for each treatment group is

$$
(Y_{gB},Y_{gW})\mid N_g=n_g
\sim\operatorname{Mult}(n_g;\pi_{gB},\pi_{gW}).
$$

For `fit1`, the additive Poisson means imply

$$
\pi_{go}
=\frac{e^{\beta_o}}{e^{\beta_B}+e^{\beta_W}},
$$

so the outcome probabilities are common to all three treatments. For `fit2`,

$$
\pi_{go}
=\frac{e^{\beta_o+\gamma_{go}}}
{\sum_{r\in\{B,W\}}e^{\beta_r+\gamma_{gr}}},
$$

so each treatment may have its own outcome probabilities.

The [Poisson trick](../../../../../../../poisson-trick.md) is [Poisson-multinomial conditioning](../../../../../../../poisson-multinomial-conditioning.md): independent Poisson cell counts, conditional on their total, are multinomial with probabilities proportional to their means. With free treatment main effects, profiling the Poisson likelihood over the group totals gives the multinomial likelihood up to a parameter-independent factor. The Poisson regressions therefore fit these multinomial models and give the same likelihood-ratio comparisons for the outcome parameters.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [13J](../../../13j.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
