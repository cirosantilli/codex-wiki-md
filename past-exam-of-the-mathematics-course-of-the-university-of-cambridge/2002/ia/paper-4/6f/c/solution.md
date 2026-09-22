<h1 id="6f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [set](../../../../../../set-split.md) of all $n!$ [permutations](../../../../../../permutation.md), let $A_i$ consist of those fixing $i$. For a prescribed collection of $k$ fixed points, its intersection has $(n-k)!$ members. Applying the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) to the complement of $\bigcup_iA_i$ gives the number of [derangements](../../../../../../derangement-of-a-permutation.md):

$$
\boxed{d_n=\sum_{k=0}^n(-1)^k\binom nk(n-k)!=n!\sum_{k=0}^n\frac{(-1)^k}{k!}}.
$$

The convergent [power series](../../../../../../power-series.md) for the [exponential function](../../../../../../exponential-function.md) at $-1$ therefore gives $\boxed{d_n/n!\longrightarrow e^{-1}}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6F](../../6f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
