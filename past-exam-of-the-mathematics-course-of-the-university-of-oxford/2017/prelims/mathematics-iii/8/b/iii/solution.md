<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**No, not from the stated assumptions alone.** The centered slope is a weighted sum,

$$
\widehat\beta_1-\beta_1=\frac{\sum_i x_i\epsilon_i}{S_{xx}},
$$

and the weighted errors need not be identically distributed. The ordinary [central limit theorem](../../../../../../../central-limit-theorem.md) therefore does not apply directly.

For a concrete counterexample, for every $n\ge3$ choose

$$
x=(1,-1,0,\ldots,0),\qquad z=(1,1,-2,0,\ldots,0).
$$

These satisfy all three centring and [orthogonality](../../../../../../../orthogonal-vectors.md) assumptions, and both explanatory columns are nonzero. Let the errors be [independent](../../../../../../../independent-random-variables.md) with [Rademacher distribution](../../../../../../../rademacher-distribution.md), taking values $\pm1$ with equal [probability](../../../../../../../probability.md). Then

$$
\widehat\beta_1-\beta_1=\frac{\epsilon_1-\epsilon_2}{2},
$$

which takes values $-1,0,1$ with [probabilities](../../../../../../../probability.md) $1/4,1/2,1/4$ for every $n$. Increasing the sample size adds no information about this slope, and the standardized estimator does not approach a [normal distribution](../../../../../../../normal-distribution.md).

A useful additional assumption for [asymptotic normality of a weighted regression slope](../../../../../../../asymptotic-normality-of-a-weighted-regression-slope.md) is that no single design value dominates:

$$
\frac{\max_i x_i^2}{\sum_i x_i^2}\longrightarrow0.
$$

Under this condition and the given finite error [variance](../../../../../../../variance-split.md), the [Lindeberg-Feller central limit theorem](../../../../../../../lindeberg-feller-central-limit-theorem.md) yields

$$
\frac{\sqrt{S_{xx}}(\widehat\beta_1-\beta_1)}{\sigma}\xrightarrow d N(0,1),
$$

justifying the approximation $N(\beta_1,\sigma^2/S_{xx})$ for the slope as well.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
