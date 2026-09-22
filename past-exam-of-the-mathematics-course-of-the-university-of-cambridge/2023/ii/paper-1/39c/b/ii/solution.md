<h1 id="39c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Only the axisymmetric and $\cos2\theta$ modes are needed. The exterior biharmonic forms compatible with the far-field velocity are

$$
\psi_0(r)=\frac\gamma4r^2+C_0\log r+D_0,
$$



$$
\psi_2(r,\theta)
=\left(-\frac\gamma4r^2+C_2+D_2r^{-2}\right)\cos2\theta.
$$

Terms $r^2\log r$ and $r^4\cos2\theta$ are excluded because they would dominate the imposed shear.

The two conditions at $r=a$ applied separately to each Fourier mode give

$$
C_0=-\frac{\gamma a^2}{2},
\qquad
D_0=-\frac{\gamma a^2}{4}+\frac{\gamma a^2}{2}\log a,
$$



$$
C_2=\frac{\gamma a^2}{2},
\qquad
D_2=-\frac{\gamma a^4}{4}.
$$

Hence

$$
\boxed{
\psi(r,\theta)
=\frac\gamma4\left[
 r^2-a^2-2a^2\log\frac ra
-\left(r^2-2a^2+\frac{a^4}{r^2}\right)\cos2\theta
\right]
}.
$$

Direct differentiation gives $\psi=\psi_r=0$ at $r=a$. At infinity the remaining disturbance velocity is $O(r^{-1})$, so the imposed shear is recovered. This is the [Biharmonic stream function for a fixed disk in planar shear](../../../../../../../biharmonic-stream-function-for-a-fixed-disk-in-planar-shear.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [39C](../../../39c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
