<h1 id="welch-s-t-test">Welch's t-test</h1>

↑ **Parent:** [Student's t-test](student-s-t-test.md)

For two [independent](independent-random-variables.md) samples from approximately [normal distributions](normal-distribution.md), [Welch's t-test](welch-s-t-test.md) compares their means without assuming equal unknown [variances](variance-split.md). The displayed [test statistic](test-statistic.md) uses sample [variances](variance-split.md) $s_X^2,s_Y^2$. Under the equal-mean [null hypothesis](null-hypothesis.md), its reference [Student t-distribution](student-s-t-distribution.md) has approximate [statistical degrees of freedom](statistical-degrees-of-freedom.md)

$$
\nu=\frac{(s_X^2/n_X+s_Y^2/n_Y)^2}{(s_X^2/n_X)^2/(n_X-1)+(s_Y^2/n_Y)^2/(n_Y-1)}.
$$

A [p-value](p-value.md) from this approximation addresses the specified statistical error model; it cannot distinguish a material effect from an unmeasured experimenter bias when sample and experimenter are confounded.

**Table of contents**

- [Welch degrees of freedom upper bound](welch-degrees-of-freedom-upper-bound.md)

## ↑ Ancestors (8)

1. [Student's t-test](student-s-t-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Bernard Lewis Welch](bernard-lewis-welch.md)
- [Consistency identities for a two-sided t-test](consistency-identities-for-a-two-sided-t-test.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/1/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/1/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/1/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2021/1/a/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2022/1/solution.md)
- [Solution](past-exam-of-the-experimental-design-and-methods-course-of-the-year-2-of-the-psychology-experimental-course-of-the-university-of-oxford/2022/3/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-a/5/solution.md)
- [Solution](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2023/paper-1/9/d/solution.md)
- [Welch degrees of freedom upper bound](welch-degrees-of-freedom-upper-bound.md)
- [Welch's t-test](welch-s-t-test.md)
