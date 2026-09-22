<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Symmetry of the real [inner product](../../../../../../../inner-product-split.md) gives $A^T=A$. Moreover, [i](../i.md) with $y=x$ shows that

$$
x^TAx=\left\|\sum_{i=1}^n x_iv_i\right\|^2\geq0
\qquad(x\in\mathbb R^n),
$$

so the [Gram matrix](../../../../../../../gram-matrix.md) is a [positive semidefinite matrix](../../../../../../../positive-semidefinite-matrix.md). To also check reality of every [eigenvalue](../../../../../../../eigenvalue.md), allow a nonzero [vector](../../../../../../../vector.md) $z=a+ib\in\mathbb C^n$ with $Az=\lambda z$. Since $A$ is a real [symmetric matrix](../../../../../../../symmetric-matrix.md),

$$
z^*Az=a^TAa+b^TAb+i(a^TAb-b^TAa)=a^TAa+b^TAb\geq0.
$$

Here $z^*$ is the [conjugate transpose](../../../../../../../conjugate-transpose.md), and $a^TAb=b^TAa$ cancels the imaginary part. Thus

$$
\boxed{\lambda=\frac{z^*Az}{z^*z}\in[0,\infty),}
$$

because $z^*z>0$. This proves both that every [eigenvalue](../../../../../../../eigenvalue.md) is real and that it is nonnegative.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [4](../../../4.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
