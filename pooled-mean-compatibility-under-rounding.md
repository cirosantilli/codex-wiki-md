# Pooled-mean compatibility under rounding

↑ **Parent:** [Weighted arithmetic mean](weighted-arithmetic-mean.md)

For a [partition of a set](partition-of-a-set.md) of complete sample observations into groups of known sizes $n_g$ and total $N$, its [sample mean](sample-mean.md) is the [weighted mean](weighted-arithmetic-mean.md) of the group [sample means](sample-mean.md). Indeed, dividing $\sum_g\sum_{i\in g}y_i=\sum_g n_g\overline y_g$ by $N$ proves the identity. If the printed group means $m_g$ each have absolute [rounding error](round-off-error.md) at most $\delta_g$, their compatible pooled mean lies in

$$
\left[\sum_g\frac{n_g}{N}(m_g-\delta_g),\ \sum_g\frac{n_g}{N}(m_g+\delta_g)\right].
$$

This follows because all the weights are nonnegative. Equivalently, the pooled absolute [rounding error](round-off-error.md) is at most $\sum_g(n_g/N)\delta_g$, by the [triangle inequality](triangle-inequality.md). A printed overall mean must have a [rounding](rounding.md) interval intersecting this interval. Disjoint intervals prove incompatibility, rather than merely a difference of displayed decimals. This is a necessary consistency check for means of the same complete sample; it cannot silently equate a full-sample mean with a different complete-case mean or establish a unique repair to inconsistent output.

## ↑ Ancestors (8)

1. [Weighted arithmetic mean](weighted-arithmetic-mean.md)
2. [Sum](sum.md)
3. [Summation](summation.md)
4. [Addition](addition.md)
5. [Arithmetic](arithmetic-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/1/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/1/solution.md)
