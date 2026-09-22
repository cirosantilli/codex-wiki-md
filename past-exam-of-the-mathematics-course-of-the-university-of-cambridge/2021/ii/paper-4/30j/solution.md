<h1 id="30j/solution">Solution</h1>

↑ **Parent:** [30J](../30j.md)

A random forest independently bootstrap-resamples the data for each tree, and at each split considers a fresh random subset of features. It averages the resulting regression trees: $f_{\rm rf}=B^{-1}\sum_b\widehat T^{(b)}$. Each leaf prediction is an average of responses, so it lies in $[-M,M]$.

The [Bounded differences inequality](../../../../../mcdiarmid-s-inequality.md) says that if changing coordinate $i$ changes $G$ by at most $c_i$, then $\mathbb P(G-\mathbb EG\geq t)\leq\exp(-2t^2/\sum c_i^2)$. Replacing one tree changes the forest pointwise by at most $2M/B$, and hence changes the supremum $G$ by at most that amount. Therefore

$$
G\leq\mathbb EG+M\sqrt{2\log(1/δ)/B}
$$

with probability at least $1-δ$.

## ↑ Ancestors (10)

1. [30J](../30j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
