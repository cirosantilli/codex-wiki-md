<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [martingale product identity](../../../../../../martingale-product-identity.md) and the Itô isometry for cross terms give

$$
\mathbb E\left[B_t\int_0^te^{B_s}\,dB_s\right]
=\mathbb E\int_0^te^{B_s}\,ds.
$$

Since $B_s\sim N(0,s)$, its [moment-generating function](../../../../../../moment-generating-function.md) gives $\mathbb Ee^{B_s}=e^{s/2}$. Therefore the answer is

$$
\boxed{\int_0^te^{s/2}\,ds=2(e^{t/2}-1).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
