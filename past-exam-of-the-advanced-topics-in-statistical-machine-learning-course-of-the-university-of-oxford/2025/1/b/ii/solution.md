<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With $r$, $Z$, and $W$ as above, [independence](../../../../../independent-random-variables.md) of the draws gives the [variance of a sample mean](../../../../../variance-of-a-sample-mean.md):

$$
\boxed{\operatorname{Var}(\widehat p_1)=\frac1T\left[\int\frac{r(\theta)^2}{q(\theta)}\,d\theta-Z^2\right]}.
$$

This formula allows infinite [variance](../../../../../variance-split.md). To identify the optimum, write $\pi(\theta)=p(\theta\mid\mathcal D)=r(\theta)/Z$. Then

$$
\operatorname{Var}(\widehat p_1)=\frac{Z^2}{T}\left[\int\frac{\pi^2}{q}-1\right]=\frac{Z^2}{T}\int_{\{q>0\}}\frac{(\pi-q)^2}{q}\,d\theta.
$$

The last equality uses $\int\pi=\int q=1$. Its nonnegative integrand proves

$$
\boxed{q_{\rm opt}(\theta)=\pi(\theta)=p(\theta\mid\mathcal D),\qquad \min\operatorname{Var}(\widehat p_1)=0}.
$$

Indeed, all [importance weights](../../../../../importance-weight.md) then equal $Z$. This is a formal optimum: evaluating the normalized [posterior density](../../../../../posterior-density.md) generally already requires the unknown [marginal likelihood](../../../../../bayesian-model-evidence.md).

**Poor coverage of regions with substantial posterior mass produces large weights.** In particular, excessively light proposal tails, a proposal that is too narrow, or a missed mode can make $\int r^2/q$ enormous or infinite. A proposal that is unnecessarily diffuse can also waste nearly all draws on negligible [posterior probability](../../../../../posterior-probability.md). Omitting target support altogether violates unbiasedness, rather than merely increasing [variance](../../../../../variance-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
