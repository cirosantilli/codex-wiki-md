<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At a distinct event time $a_m$, estimate the conditional [probability](../../../../../../probability.md) of surviving that time by $1-d_m/r_m$. Multiplication of these conditional [survival probabilities](../../../../../../survival-probability.md) gives the [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md), and taking minus its logarithm gives an [integrated hazard](../../../../../../cumulative-hazard-function.md) estimate:

$$
\boxed{\widehat S_{\rm KM}(t)=\prod_{a_m\le t}\left(1-\frac{d_m}{r_m}\right),\qquad \widehat H_{\rm KM}(t)=-\log\widehat S_{\rm KM}(t)=\sum_{a_m\le t}-\log\left(1-\frac{d_m}{r_m}\right).}
$$

The conditional failure count has a [binomial likelihood](../../../../../../binomial-likelihood.md) whose maximizing event fraction is $d_m/r_m$. Tied failures therefore enter directly as one count. Even ordering $d_m$ failures arbitrarily, with no intervening [censoring](../../../../../../censoring-statistics.md), produces the same [survivor function](../../../../../../survival-function.md) factor because

$$
\prod_{s=0}^{d_m-1}\left(1-\frac1{r_m-s}\right)=\frac{r_m-d_m}{r_m}=1-\frac{d_m}{r_m}.
$$

The failure-versus-[censoring](../../../../../../censoring-statistics.md) ordering convention still matters when both have the same recorded time. If $d_m=r_m$, the [survivor function](../../../../../../survival-function.md) becomes zero and the logarithmic [integrated hazard](../../../../../../cumulative-hazard-function.md) is infinite.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
