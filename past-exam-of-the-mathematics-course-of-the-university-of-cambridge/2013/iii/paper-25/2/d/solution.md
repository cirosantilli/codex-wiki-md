<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Multiply the representation in part (c) by $\int_0^\infty\alpha_u\,dW_u$ and take expectations. This [Itô integral](../../../../../../ito-integral.md) has mean zero, and the bilinear form of the [Itô isometry](../../../../../../ito-isometry.md) gives

$$
\mathbb E\left[\phi(W_T)\int_0^\infty\alpha_u\,dW_u\right]=\mathbb E\int_0^\infty\beta_u\alpha_u\,du.
$$

Equating this with part (b), and writing both ordinary integrals with the same time variable, yields

$$
\boxed{\mathbb E\int_0^\infty\left(\beta_u-\phi'(W_T)\mathbf1_{\{u\le T\}}\right)\alpha_u\,du=0.}
$$

All terms are integrable by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), the assumed square integrability of $\alpha$, and boundedness of $\phi'$. This is an orthogonality statement against [predictable processes](../../../../../../predictable-process.md); its second term need not itself be predictable.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
