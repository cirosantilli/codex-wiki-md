# Fisher-Neyman factorization theorem

↑ **Parent:** [Sufficient statistic](sufficient-statistic.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fisher-Neyman_factorization_theorem)

Assume the full-data [sample space](sample-space.md) and the range of the [statistic](statistic.md) $T$ are [standard Borel spaces](standard-borel-space.md), $T$ is a [measurable function](measurable-function.md), and the [statistical model](statistical-model-split.md) $\{P_\theta\}$ is dominated by one common [sigma-finite measure](sigma-finite-measure.md) $\nu$. Write $f_\theta=dP_\theta/d\nu$ for its densities. Then $T$ is a [sufficient statistic](sufficient-statistic.md) if and only if there exist nonnegative [measurable functions](measurable-function.md) $g_\theta$ and $h$, with $h$ independent of $\theta$, such that

$$
f_\theta(x)=g_\theta(T(x))h(x)\quad\nu\text{-almost everywhere for each }\theta.
$$

The [statistical parameter](statistical-parameter.md) can enter $g_\theta$ only through $\theta$ and the observed $T(x)$. [Sufficiency, Will Fithian, “Factorization theorem”: common dominating measure and almost-everywhere factorization](sufficiency-stat-210a-fall-2025-by-will-fithian.md)

For discrete data, take [counting measure](counting-measure.md); for ordinary continuous data, take [Lebesgue measure](lebesgue-measure.md). Independence, identical sampling laws, smooth dependence on $\theta$, and a fixed positive [support of a probability distribution](support-of-a-probability-distribution.md) are not requirements of this theorem. Parameter-dependent support must nevertheless be included in $f_\theta$, usually through an [indicator function](indicator-function.md), and must fit the displayed factorization. The [sufficient statistic for a symmetric uniform sample](sufficient-statistic-for-a-symmetric-uniform-sample.md) illustrates exactly this: its [indicator function](indicator-function.md) depends on the unknown scale through the observed absolute maximum. The [null sets](null-set.md) in the theorem concern versions of densities; the factors are not generally themselves normalized [probability distributions](probability-distribution-split.md).

For a discrete [sample space](sample-space.md), the cancellation behind the theorem is particularly transparent. On a group with positive [probability](probability.md), factorization gives

$$
P_\theta(X=x\mid T=t)=\frac{h(x)\mathbf1_{\{T(x)=t\}}}{\sum_{z:T(z)=t}h(z)}.
$$

Conversely, multiply a common conditional [probability mass function](probability-mass-function.md) by $P_\theta(T=T(x))$ to obtain the required factorization. For continuous data, a sum over a group is not a density integral over the original [Lebesgue measure](lebesgue-measure.md): the group may have measure zero. Use the [regular conditional distribution](regular-conditional-distribution.md) formulation and the [Fisher-Neyman factorization theorem](fisher-neyman-factorization-theorem.md) instead of that discrete calculation.

## ↑ Ancestors (5)

1. [Sufficient statistic](sufficient-statistic.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Allele-sharing sufficiency for recessive linkage](allele-sharing-sufficiency-for-recessive-linkage.md)
- [Conditional multinomial sufficient statistics](conditional-multinomial-sufficient-statistics.md)
- [Fisher-Neyman factorization theorem](fisher-neyman-factorization-theorem.md)
- [Normal likelihood with variance equal to squared mean](normal-likelihood-with-variance-equal-to-squared-mean.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1/3h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/1/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/18c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/26i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/28j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/27j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/27k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/19h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/7h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/13j/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/19h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/13j/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/6h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1/18h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1/6h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1/6h/c/solution.md)
- [Sample mean sufficiency depends on the model](sample-mean-sufficiency-depends-on-the-model.md)
