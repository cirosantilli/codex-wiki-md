<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The pulse height is the constant $t_0$, not the time variable. In the undamped case the [convolution](../../../../../convolution.md) therefore reduces to

$$
x(t)=\frac{t_0}{2}\int_0^{\min(t,t_0)}\sin[2(t-\tau)]\,d\tau.
$$

Integration gives the continuous displacement and velocity

$$
\boxed{x(t)=\begin{cases}
\displaystyle\frac{t_0}{4}(1-\cos2t),&0\leq t<t_0,\\
\displaystyle\frac{t_0}{4}\left[\cos2(t-t_0)-\cos2t\right],&t\geq t_0.
\end{cases}}
$$

The post-pulse expression is equivalently $x(t)=(t_0/2)\sin t_0\sin(2t-t_0)$. Since $t_0>0$, it vanishes for every subsequent time precisely when $\sin t_0=0$. Thus

$$
\boxed{t_0=n\pi,\qquad n=1,2,3,\ldots.}
$$

These are integer multiples of the oscillator's natural period $\pi$. At such switch-off times both $x(t_0)$ and $x'(t_0)$ are zero. Vanishing displacement alone would not suffice: a nonzero switch-off velocity would restart an oscillation. This is [rectangular-pulse cancellation of an undamped oscillator](../../../../../rectangular-pulse-cancellation-of-an-undamped-oscillator.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
