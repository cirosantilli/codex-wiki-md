<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [mean first-passage time](../../../../../../mean-first-passage-time.md) obeys the backward equation

$$
D\tau''+\alpha\tau'=-1,
\qquad \tau(0)=0,
\qquad \tau'(L)=0.
$$

For $\alpha\ne0$, direct integration gives

$$
\boxed{\tau(y)=
\frac D{\alpha^2}e^{\alpha L/D}
\left(1-e^{-\alpha y/D}\right)-\frac y\alpha.}
$$

In particular,

$$
\tau(L)=\frac D{\alpha^2}
\left(e^{\alpha L/D}-1\right)-\frac L\alpha.
$$

This increases monotonically with drift away from the target, so the constrained optimum is

$$
\boxed{\alpha_*=-\bar\alpha.}
$$

Expanding the exponential at zero drift yields

$$
\boxed{\tau_0=\lim_{\alpha\to0}\tau(L)=\frac{L^2}{2D}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
