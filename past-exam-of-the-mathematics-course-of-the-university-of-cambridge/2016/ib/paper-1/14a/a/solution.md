<h1 id="14a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the real coefficients of the stated [self-adjoint](../../../../../../self-adjoint-operator.md) [Sturm-Liouville problem](../../../../../../sturm-liouville-problem.md), define the weighted [inner product](../../../../../../inner-product.md)

$$
\boxed{\langle u,v\rangle_w=\int_a^b w(x)\overline{u(x)}v(x)\,dx.}
$$

Since $w>0$, a nonzero eigenfunction has positive squared [norm](../../../../../../norm.md). Let $L y=-(py')'+qy$. [Integration by parts](../../../../../../integration-by-parts.md) and the [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) give

$$
\int_a^b\overline u\,Lv\,dx=\int_a^b\bigl(p\overline{u'}v'+q\overline uv\bigr)\,dx=\int_a^b\overline{Lu}\,v\,dx.
$$

Taking $u=v$ to be an [eigenfunction](../../../../../../eigenfunction.md) shows that its [eigenvalue](../../../../../../eigenvalue.md) is real, since $\lambda\int w|u|^2=\int(p|u'|^2+q|u|^2)$ is real. For two eigenfunctions with [eigenvalues](../../../../../../eigenvalue.md) $\lambda,\mu$, the same identity gives

$$
(\mu-\lambda)\langle u,v\rangle_w=0.
$$

Hence **distinct eigenvalues imply orthogonality in the weighted inner product**. This is the [orthogonality of Sturm-Liouville eigenfunctions](../../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md). The calculation assumes the regularity needed for the stated self-adjoint boundary problem, so all boundary terms and integrals are defined.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14A](../../14a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
