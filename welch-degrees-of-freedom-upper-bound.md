# Welch degrees of freedom upper bound

↑ **Parent:** [Welch's t-test](welch-s-t-test.md)

For two samples of sizes $n_1,n_2>1$, write $a=s_1^2/n_1$ and $b=s_2^2/n_2$, with $a+b>0$. The reference [statistical degrees of freedom](statistical-degrees-of-freedom.md) in [Welch's t-test](welch-s-t-test.md) satisfy

$$
\nu=\frac{(a+b)^2}{a^2/(n_1-1)+b^2/(n_2-1)}\le n_1+n_2-2.
$$

Indeed the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) applied to $(a/\sqrt{n_1-1},b/\sqrt{n_2-1})$ and $(\sqrt{n_1-1},\sqrt{n_2-1})$ gives the inequality after division. Thus an independent two-sample [Welch's t-test](welch-s-t-test.md) on $N$ complete observations cannot have reference [statistical degrees of freedom](statistical-degrees-of-freedom.md) exceeding $N-2$. The [exact pooled two-sample t statistic](exact-pooled-two-sample-t-statistic.md) also uses $N-2$, under its stronger equal-variance assumptions.

## ↑ Ancestors (9)

1. [Welch's t-test](welch-s-t-test.md)
2. [Student's t-test](student-s-t-test.md)
3. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2022/1/solution.md)
