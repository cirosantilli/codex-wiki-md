<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At stage 1, the [maximum-likelihood estimators](../../../../../../../maximum-likelihood-estimator.md) of the two normal arm means are their sample means. Their difference estimates the treatment effect:

$$
\widehat\delta_1=Y_{11}-Y_{01}.
$$

Each arm has $n_1$ patients and [variance](../../../../../../../variance-split.md) $\sigma^2/n_1$, so [independence](../../../../../../../independent-random-variables.md) across arms gives

$$
\boxed{\widehat\delta_1\sim N\left(\delta,\frac{2\sigma^2}{n_1}\right)
=N(\delta,I_1^{-1}),\qquad I_1=\frac{n_1}{2\sigma^2}.}
$$

The quantity $I_1$ is the [Fisher information](../../../../../../../fisher-information-matrix.md) for the mean difference when the common [variance](../../../../../../../variance-split.md) is known. The PDF's preliminary expression uses $n_i$ for the [variance](../../../../../../../variance-split.md) denominator, although $i$ indexes arms and $n_0$ is not defined. The stage-specific [sample size](../../../../../../../sample-size.md) is $n_j$; the calculation uses this intended reading, consistent with the specified $n_1,n_2$ per-arm recruitment and the later weighted [estimator](../../../../../../../estimator.md). Fresh stage-2 patients are independent of stage-1 patients in the usual trial model; the cumulative stage means themselves are not independent across stages.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
