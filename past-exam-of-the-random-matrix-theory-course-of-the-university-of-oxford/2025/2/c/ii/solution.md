<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Evaluate the [orthogonal polynomial projection kernel](../../../../../orthogonal-polynomial-projection-kernel.md) on its diagonal:

$$
\begin{aligned}
R_3^{(1)}(\lambda)
&=\sum_{\ell=0}^2\phi_\ell(\lambda)^2\\
&=\frac{e^{-\lambda^2/2}}{\sqrt{2\pi}}
\left[1+\lambda^2+\frac{(\lambda^2-1)^2}{2}\right]\\
&=\boxed{\frac{\lambda^4+3}{2\sqrt{2\pi}}e^{-\lambda^2/2}.}
\end{aligned}
$$

The $\lambda^2$ terms cancel. Integrating against [Lebesgue measure](../../../../../lebesgue-measure.md) gives $(\mathbb EZ^4+3)/2=3$ for a [standard normal random variable](../../../../../standard-normal-random-variable.md) $Z$, checking the [correlation function of a point process](../../../../../correlation-function-of-a-point-process.md) normalization.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
