<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At exit, continuity gives $X_T^2=1$. The preceding density identity becomes

$$
Z_T=\exp\left(\frac12-\frac T2-\frac12\int_0^T X_s^2ds\right).
$$

Since $|X_s|\le1$ before exit, $\int_0^TX_s^2ds\le T$. On $\{T\le t\}$ it follows that $Z_T\ge e^{1/2-T}\ge e^{1/2-t}$. The definition of the changed measure now yields

$$
\boxed{\mathbb P(T\le t)
=\widetilde{\mathbb E}[Z_T\mathbf1_{\{T\le t\}}]
\ge e^{1/2-t}\widetilde{\mathbb P}(T\le t).}
$$

The positive sign of the [stochastic integral](../../../../../../stochastic-integral.md) in the density is what introduces the positive drift $X_tdt$; reversing that sign would give a different measure and would not prove this inequality.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
