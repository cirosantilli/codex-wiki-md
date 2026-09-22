<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Box-Muller transform](../../../../../../../box-muller-transform.md) uses independent uniforms to set

$$
R=\sqrt{-2\log U_2},\qquad A=2\pi U_3,\qquad
\boxed{X_1=R\cos A,\quad X_2=R\sin A.}
$$

The radius has the unit [Rayleigh distribution](../../../../../../../rayleigh-distribution.md), with density $re^{-r^2/2}$ for $r>0$, and the angle is independently uniform on $[0,2\pi)$. Their joint density is $(2\pi)^{-1}re^{-r^2/2}$. The Cartesian change of variables has absolute [Jacobian determinant](../../../../../../../jacobian-determinant.md) $r$, so the joint density of $(X_1,X_2)$ is

$$
\frac1{2\pi}e^{-(x_1^2+x_2^2)/2}
=\left(\frac1{\sqrt{2\pi}}e^{-x_1^2/2}\right)
\left(\frac1{\sqrt{2\pi}}e^{-x_2^2/2}\right).
$$

The factorization proves that the outputs are [independent random variables](../../../../../../../independent-random-variables.md), each with a [standard normal distribution](../../../../../../../standard-normal-distribution.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
