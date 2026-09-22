<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

For $\operatorname{Re}s>1$, expand $(e^t-1)^{-1}=\sum_{n\geq1}e^{-nt}$. [Absolute convergence](../../../../../absolute-convergence.md) of the integrated series follows from the same expression with $\operatorname{Re}s$ in place of $s$. Integrating termwise and substituting $u=nt$ gives

$$
\int_0^\infty\frac{t^{s-1}}{e^t-1}\,dt=\sum_{n\geq1}n^{-s}\Gamma(s)=\Gamma(s)\zeta(s).
$$

This proves the [Mellin transform](../../../../../mellin-transform.md) representation of the [Riemann zeta function](../../../../../riemann-zeta-function.md).

Take the [Hankel contour](../../../../../hankel-contour.md) along the lower side of the negative axis towards zero, around zero counterclockwise, and back along the upper side. For $\operatorname{Re}s>1$ the small-circle contribution tends to zero. On the lower and upper rays, respectively, $\arg t=-\pi,+\pi$, so the two integrals combine to

$$
\int_H\frac{t^{s-1}}{e^{-t}-1}\,dt=\left(e^{-i\pi(s-1)}-e^{i\pi(s-1)}\right)\int_0^\infty\frac{x^{s-1}}{e^x-1}\,dx=2i\sin(\pi s)\Gamma(s)\zeta(s).
$$

The [gamma reflection formula](../../../../../gamma-reflection-formula.md) now proves agreement of the two representations. At an integer $s=m\geq2$, the contour integral has a zero while $\Gamma(1-s)$ has a pole: **their product is interpreted by its finite limit, equal to $\zeta(m)$**, not by multiplying literal zero and infinity.

For nonpositive integers the integrand is single-valued, and the contour closes around zero. Since

$$
\frac1{e^{-t}-1}=-\frac1t-\frac12+O(t),
$$

the [residue](../../../../../residue.md) of $t^{-1}/(e^{-t}-1)$ is $-1/2$, giving **$\zeta(0)=-1/2$**. Also

$$
\frac1{e^{-t}-1}+\frac12=-\frac12\coth(t/2)
$$

is odd. Its Laurent series therefore has only odd powers. Multiplication by $t^{-2n-1}$ cannot produce a $t^{-1}$ term, and the subtracted constant cannot do so when $n\geq1$. Hence the contour integral vanishes and **$\zeta(-2n)=0$ for every positive integer $n$**.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
