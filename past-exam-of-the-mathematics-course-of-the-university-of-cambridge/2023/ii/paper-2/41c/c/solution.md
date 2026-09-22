<h1 id="41c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The matrix $C$ from part (a) is [Hermitian positive definite](../../../../../../hermitian-positive-definite-matrix.md), while the real [diagonal matrix](../../../../../../diagonal-matrix.md) $D$ is Hermitian. The stated product theorem, or similarity

$$
CD=C^{1/2}(C^{1/2}DC^{1/2})C^{-1/2},
$$

shows that every [eigenvalue](../../../../../../eigenvalue.md) of $CD$ is real. Hence every eigenvalue of $B=-CD$ is real; this is the [real spectrum of a positive-Hermitian times Hermitian product](../../../../../../real-spectrum-of-a-positive-hermitian-times-hermitian-product.md).

Moreover, $C$ is invertible and $D$ has rank $2d$, so for $d\geq1$ the matrix $B$ has nonzero real eigenvalues. If $\lambda\ne0$ is one of them, the corresponding mode of the semidiscrete equation has eigenvalue $i\pi\lambda$. The [explicit Euler method](../../../../../../euler-method.md) has amplification factor

$$
G=1+i\pi\lambda\Delta t,
\qquad
|G|=\sqrt{1+\pi^2\lambda^2\Delta t^2}>1
$$

for every $\Delta t>0$. Therefore the explicit Euler discretization is unstable, as in [explicit Euler instability on a nonzero imaginary eigenvalue](../../../../../../explicit-euler-instability-on-a-nonzero-imaginary-eigenvalue.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [41C](../../41c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
