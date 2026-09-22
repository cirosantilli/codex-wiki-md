<h1 id="14e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Extend $q$ by zero to $x<0$ and apply the assumed [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md). For sufficiently regular, decaying data and $x>0$ this gives $q(x)=(2\pi)^{-1}\int_{\mathbb R}e^{ikx}\widehat q(k)\,dk$, with $\widehat q(k)=\int_0^\infty e^{-ikx}q(x)\,dx$. If $\operatorname{Im}k\leq0$, the exponential in this last integral is bounded in magnitude by one; it defines a holomorphic transform in the lower half-plane, with its boundary values on the real axis.

The PDF orients $L$ from $i\infty$ down to zero, then from zero to $+\infty$. The function $e^{ikx}\widehat q(-k)$ is holomorphic in the upper half-plane, and for $x>0$ its exponential decays there. Close the two rays through a large first-quadrant arc. [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) and [Jordan lemma](../../../../../../jordan-s-lemma.md) give

$$
\boxed{\int_L e^{ikx}\widehat q(-k)\,dk=0.}
$$

For example, if $q,q'$ are integrable, integration by parts gives $\widehat q(-k)=O(1/k)$ in that quadrant, which suffices for the arc estimate. Standard limiting arguments extend the identity to the admissible Fourier-inversion class. Adding any constant multiple of this zero integral to ordinary inversion proves

$$
\boxed{q(x)=\frac1{2\pi}\int_{\mathbb R}e^{ikx}\widehat q(k)\,dk+\frac c{2\pi}\int_L e^{ikx}\widehat q(-k)\,dk,\quad c\in\mathbb C.}
$$

The extra integral is a reflected, zero-supported contribution, not an extra datum.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [14E](../../14e.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
