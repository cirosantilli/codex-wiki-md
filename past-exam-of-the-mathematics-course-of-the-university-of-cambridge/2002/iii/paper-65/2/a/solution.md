<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $A$ is a real symmetric [positive-definite matrix](../../../../../../positive-definite-matrix.md), its inverse exists and all its [eigenvalues](../../../../../../eigenvalue.md) are positive. [Completing the square](../../../../../../completing-the-square.md) gives

$$
-\frac12u^TAu+b^Tu
=-\frac12(u-A^{-1}b)^TA(u-A^{-1}b)+\frac12b^TA^{-1}b.
$$

The translation $v=u-A^{-1}b$ has unit [Jacobian determinant](../../../../../../jacobian-determinant.md). Choose an [orthogonal matrix](../../../../../../orthogonal-matrix.md) $O$ with $O^TAO=\operatorname{diag}(a_1,\ldots,a_n)$, where $a_i>0$. The change $v=Oz$ also has absolute Jacobian one. The remaining integral is the product of $n$ one-dimensional [Gaussian integrals](../../../../../../gaussian-integral.md), each equal to $\sqrt{2\pi/a_i}$. Consequently the [linear-source multivariate Gaussian integral](../../../../../../linear-source-multivariate-gaussian-integral.md) is

$$
\boxed{\int_{\mathbb R^n}d^nu\,e^{-u^TAu/2+b^Tu}
=\frac{(2\pi)^{n/2}}{\sqrt{\det A}}
\exp\left(\frac12b^TA^{-1}b\right).}
$$

The determinant square root is the positive one, as required by convergence of the original real integral.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
