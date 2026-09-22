# Truncated lognormal moment

↑ **Parent:** [Log-normal distribution](log-normal-distribution.md)

If $\log S=m+sZ$ with $s>0$, $K>0$ and $Z$ having the [standard normal distribution](standard-normal-distribution.md), then for every real $p$,

$$
\begin{aligned}
\mathbb E[S^p\mathbf1_{\{S>K\}}]&=e^{pm+p^2s^2/2}\Phi\!\left(\frac{m+ps^2-\log K}{s}\right),\\
\mathbb E[S^p\mathbf1_{\{S<K\}}]&=e^{pm+p^2s^2/2}\Phi\!\left(\frac{\log K-m-ps^2}{s}\right).
\end{aligned}
$$

Here $\Phi$ is the [standard normal distribution function](standard-normal-distribution-function.md). Multiplying the [normal distribution](normal-distribution.md) density by $e^{psZ}$ and completing the square shifts its mean by $ps$ and supplies the factor $e^{p^2s^2/2}$; this is a [Gaussian exponential tilt](exponential-tilting-of-an-isonormal-gaussian-process.md). Integrating above or below the shifted threshold proves both formulas. They apply to noninteger and negative powers, including the inverse-price moment $p=-1$. The lower-tail formula gives the [European power put formula](european-power-put-formula.md) after a [binomial theorem](binomial-theorem.md) expansion.

## ↑ Ancestors (8)

1. [Log-normal distribution](log-normal-distribution.md)
2. [Normal distribution](normal-distribution.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Conditional lognormal layer recovery](conditional-lognormal-layer-recovery.md)
- [European power put formula](european-power-put-formula.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2021/2/c/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2021/2/e/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2023/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-27/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-45/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/27k/iii/solution.md)
