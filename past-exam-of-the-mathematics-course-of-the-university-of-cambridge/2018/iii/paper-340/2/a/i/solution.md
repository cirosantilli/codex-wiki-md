<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../../../fourier-transform.md) convention $\widehat\varphi(\xi)=\int\varphi(x)e^{-ix\xi}\,dx$. Nesting and the [orthonormal basis](../../../../../../../orthonormal-basis.md) of $V_1$ give the [scaling refinement equation](../../../../../../../scaling-refinement-equation.md)

$$
\varphi(x)=\sqrt2\sum_kh_k\varphi(2x-k),\qquad
m(\xi)=\frac1{\sqrt2}\sum_kh_ke^{-ik\xi},\qquad
\widehat\varphi(2\xi)=m(\xi)\widehat\varphi(\xi).
$$

Here $h_k=\langle\varphi,\sqrt2\varphi(2\cdot-k)\rangle$. [Compact support](../../../../../../../compact-support.md) makes these [inner products](../../../../../../../inner-product.md) zero for all but finitely many $k$, so $m$ is a [trigonometric polynomial](../../../../../../../trigonometric-polynomial.md). Expanding the orthogonality of the integer translates of $\varphi$ in the [orthonormal basis](../../../../../../../orthonormal-basis.md) of $V_1$ yields

$$
\sum_kh_k\overline{h_{k-2n}}=\delta_{n0}.
$$

Consequently

$$
|m(\xi)|^2+|m(\xi+\pi)|^2
=\sum_n\left(\sum_kh_k\overline{h_{k-2n}}\right)e^{-2in\xi}
=\boxed{1}.
$$

This holds everywhere because $m$ is continuous. The invoked properties are nesting, dyadic dilation, orthonormal integer translates, and [compact support](../../../../../../../compact-support.md); mere finite-energy refinement would not imply the [quadrature mirror filter](../../../../../../../quadrature-mirror-filter.md) identity.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 340](../../../../paper-340-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
