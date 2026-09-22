<h1 id="kendall-s-tau-b">Kendall's tau-b</h1>

↑ **Parent:** [Kendall rank correlation coefficient](kendall-rank-correlation-coefficient.md)

Let $C,D$ count [concordant pairs](concordant-pair.md) and [discordant pairs](discordant-pair.md), and let $T_X,T_Y$ count pairs tied only on the indicated variable. Then

$$
\tau_b=\frac{C-D}{\sqrt{(C+D+T_X)(C+D+T_Y)}}
$$

when both factors in the denominator are positive. Unlike [Goodman and Kruskal's gamma](goodman-and-kruskal-s-gamma.md), this coefficient accounts for ties. Its absolute value is at most one: form vectors of the comparison signs for all unordered pairs. Their [inner product](inner-product-split.md) is $C-D$ and their squared [norms](norm.md) are the two denominator factors, in reverse variable order. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) supplies the bound. A variable constant throughout gives a zero denominator, not a meaningful zero association.[KendallTauB: tie-adjusted rank association and relation to cor(method="kendall")](ordinal-association-measures-in-the-desctools-documentation.md)

## ↑ Ancestors (9)

1. [Kendall rank correlation coefficient](kendall-rank-correlation-coefficient.md)
2. [Ordinal categorical variable](ordinal-categorical-variable.md)
3. [Categorical variable](categorical-variable.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Kendall rank correlation coefficient](kendall-rank-correlation-coefficient.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/3/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/4/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/5/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/3/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/4/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/5/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/3/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/4/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/5/solution.md)
- [Sign reversal under reversal of one ordinal ordering](sign-reversal-under-reversal-of-one-ordinal-ordering.md)
- [Stuart's tau-c](stuart-s-tau-c.md)
- [Unordered-pair partition for ordinal data](unordered-pair-partition-for-ordinal-data.md)
