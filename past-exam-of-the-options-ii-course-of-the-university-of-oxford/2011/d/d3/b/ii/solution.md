<h1 id="d/d3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the nonnegative-part convention $h=h^+-h^-$, where $h^+=\max(h,0)$ and $h^-=\max(-h,0)$. The zero-mean assumption gives

$$
A=\int_0^\pi h^+=\int_0^\pi h^-.
$$

For $k\geq1$, write the [integral](../../../../../../integral-split.md) over the $k$th period as $I_k=P_k-N_k$, where

$$
P_k=\int_0^\pi\frac{h^+(t)}{k\pi+t}\,dt,
\qquad N_k=\int_0^\pi\frac{h^-(t)}{k\pi+t}\,dt.
$$

Both $P_k$ and $N_k$ lie in the [interval](../../../../../../interval-mathematics.md) $[A/((k+1)\pi),A/(k\pi)]$. Their difference therefore satisfies the stronger estimate

$$
|I_k|\leq\frac{A}{\pi k(k+1)}\leq\frac{A}{\pi k^2}.
$$

Consequently $\sum_{k\geq1}I_k$ converges absolutely as a [series](../../../../../../series-mathematics.md) of numbers, proving the requested limit of integrals over whole periods. This does not assert absolute integrability of the original function: the cancellation took place inside each period.

Indeed, setting $B=\int_0^\pi|h(t)|\,dt$, we have

$$
\int_{k\pi}^{(k+1)\pi}|g(x)|\,dx
\geq\frac{B}{(k+1)\pi}.
$$

The [harmonic series](../../../../../../harmonic-series.md) diverges, so $g$ is [Lebesgue integrable](../../../../../../integrability.md) only if $B=0$. Conversely $B=0$ means $h=0$ almost everywhere on one period, and hence on all periods, so $g=0$ almost everywhere. Therefore

$$
\boxed{g\in L^1(\pi,\infty)\iff h=0\text{ almost everywhere}.}
$$

This is an example of [integrating a mean-zero periodic function divided by x](../../../../../../integrating-a-mean-zero-periodic-function-divided-by-x.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [D3](../../../d3.md)
4. [D](../../../../d.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
