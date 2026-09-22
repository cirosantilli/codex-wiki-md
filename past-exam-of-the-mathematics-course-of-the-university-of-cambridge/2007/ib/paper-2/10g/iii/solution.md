<h1 id="10g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $d$ variables, integrate over the product of $d$ unit circles:

$$
\langle f,g\rangle=\frac1{(2\pi)^d}
\int_{[0,2\pi]^d}f(e^{i\theta_1},\ldots,e^{i\theta_d})
\overline{g(e^{i\theta_1},\ldots,e^{i\theta_d})}\,d\theta_1\cdots d\theta_d.
$$

For [multi-indices](../../../../../../multi-index-notation.md) $\alpha,\beta\in\mathbb Z_{\ge0}^d$, applying one-variable [Fourier orthogonality](../../../../../../fourier-orthogonality.md) in each variable gives

$$
\langle z^\alpha,z^\beta\rangle=\prod_{j=1}^d\delta_{\alpha_j\beta_j}.
$$

If $f=\sum_\alpha a_\alpha z^\alpha$, its squared norm is $\sum_\alpha|a_\alpha|^2$, a finite sum. The form is therefore a positive definite [Hermitian form](../../../../../../hermitian-form.md) and

$$
\boxed{\{z_1^{\alpha_1}\cdots z_d^{\alpha_d}:\alpha_j\ge0\}
\quad\text{is an orthonormal basis}.}
$$

This is the [monomial orthonormal basis on the unit torus](../../../../../../monomial-orthonormal-basis-on-the-unit-torus.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [10G](../../10g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
