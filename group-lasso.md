# Group Lasso

↑ **Parent:** [Lasso](lasso.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_Lasso)

The group Lasso partitions a coefficient vector into groups $G_1,\ldots,G_q$ and replaces the coordinatewise $\ell^1$ penalty with a weighted sum of group norms,

$$
P(\beta)=\sum_{j=1}^q m_j\lVert\beta_{G_j}\rVert_2.
$$

It tends to retain or discard an entire group at once. Its dual norm is

$$
P^*(v)=\max_j m_j^{-1}\lVert v_{G_j}\rVert_2,
$$

so the corresponding [Holder inequality](holder-inequality.md) is $|u^Tv|\leq P(u)P^*(v)$.

**Table of contents**

- [Paired group Lasso for Gaussian graph estimation](paired-group-lasso-for-gaussian-graph-estimation.md)
  - [Paired group Lasso optimality conditions](paired-group-lasso-optimality-conditions.md)

## ↑ Ancestors (5)

1. [Lasso](lasso.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-205/4/solution.md)
