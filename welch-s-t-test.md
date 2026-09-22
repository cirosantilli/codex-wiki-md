<h1 id="welch-s-t-test">Welch's t-test</h1>

↑ **Parent:** [Student's t-test](student-s-t-test.md)

For two [independent](independent-random-variables.md) samples from approximately [normal distributions](normal-distribution.md), [Welch's t-test](welch-s-t-test.md) compares their means without assuming equal unknown [variances](variance-split.md). The displayed [test statistic](test-statistic.md) uses sample [variances](variance-split.md) $s_X^2,s_Y^2$. Under the equal-mean [null hypothesis](null-hypothesis.md), its reference [Student t-distribution](student-s-t-distribution.md) has approximate [statistical degrees of freedom](statistical-degrees-of-freedom.md)

$$
\nu=\frac{(s_X^2/n_X+s_Y^2/n_Y)^2}{(s_X^2/n_X)^2/(n_X-1)+(s_Y^2/n_Y)^2/(n_Y-1)}.
$$

A [p-value](p-value.md) from this approximation addresses the specified statistical error model; it cannot distinguish a material effect from an unmeasured experimenter bias when sample and experimenter are confounded.

## ↑ Ancestors (8)

1. [Student's t-test](student-s-t-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-a/5/solution.md)
- [Welch's t-test](welch-s-t-test.md)
