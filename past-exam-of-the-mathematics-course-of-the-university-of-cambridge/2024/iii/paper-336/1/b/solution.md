<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The exponential phase is

$$
\Phi(s)=-s+2\lambda-\frac{\lambda^2}{s}.
$$

Its [saddle points](../../../../../../saddle-point.md) satisfy

$$
\Phi'(s)=-1+\frac{\lambda^2}{s^2}=0,
\qquad
s=\mathord\pm\lambda.
$$

For positive real $\lambda$, the original positive-real contour passes through $s=\lambda$; the singularity at $s=0$ separates it from the other saddle. At the contributing saddle,

$$
\Phi(\lambda)=0,
\qquad
\Phi''(\lambda)=-\frac2\lambda.
$$

Set $s=\lambda+\lambda^{1/2}t$. Then

$$
\Phi(s)=-t^2+O(\lambda^{-1/2}t^3),
\qquad
ds=\lambda^{1/2}dt.
$$

The [method of steepest descent](../../../../../../method-of-steepest-descent.md) therefore gives

$$
I(\lambda)
\sim\lambda^{-1/2}\lambda^{1/2}
\int_{-\infty}^{\infty}e^{-t^2}\,dt
=\boxed{\sqrt\pi}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
