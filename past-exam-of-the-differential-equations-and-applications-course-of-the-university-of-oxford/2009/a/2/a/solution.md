<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $y=e^xw$. Then $y''-2y'+y=e^xw''$ and the endpoint conditions become $w(0)=w(\pi)=0$. The transformed [eigenvalue](../../../../../eigenvalue.md) equation is $-w''=\lambda w$, so

$$
\boxed{\lambda_k=k^2,\qquad y_k(x)=e^x\sin(kx),\quad k=1,2,\ldots.}
$$

Zero and negative $\lambda$ yield no nonzero solution with both endpoint values zero.

For the usual unweighted $L^2(0,\pi)$ [inner product](../../../../../inner-product-split.md), the operator $D^2-2D+1$ is **not [self-adjoint](../../../../../self-adjoint-operator.md)**: its [formal adjoint](../../../../../formal-adjoint.md) is $D^2+2D+1$. The mismatch is already visible on compactly supported test functions, so endpoint conditions cannot remove it. With the different weight $e^{-2x}$ one does obtain a symmetric [Sturm-Liouville form](../../../../../sturm-liouville-form.md), since $e^{-2x}(y''-2y'+y)=(e^{-2x}y')'+e^{-2x}y$. Thus the inner-product convention matters; the real spectrum alone does not prove self-adjointness in the unweighted space.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
