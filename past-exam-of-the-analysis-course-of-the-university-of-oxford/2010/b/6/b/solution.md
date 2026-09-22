<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [inner product](../../../../../inner-product-split.md) convention $\langle f,h\rangle=\int_{-\pi}^{\pi}f\bar h$. For $h=\mathbf1_{[-\pi/2,\pi/2]}$, integration gives

$$
\langle e_0,h\rangle=\sqrt{\pi/2},\qquad\langle e_k,h\rangle=\sqrt{2/\pi}\,\frac{\sin(k\pi/2)}k\quad(k\ne0).
$$

The nonzero even coefficients vanish, while $\sin((2n+1)\pi/2)=(-1)^n$. The preceding polarized [Parseval identity](../../../../../parseval-identity.md) therefore yields

$$
\boxed{\int_{-\pi/2}^{\pi/2}f(t)dt=\sqrt{\frac\pi2}\langle f,e_0\rangle+\sqrt{\frac2\pi}\sum_{n\in\mathbb Z}(-1)^n\frac{\langle f,e_{2n+1}\rangle}{2n+1}.}
$$

Absolute [convergence](../../../../../convergence.md) follows from square summability of the [Fourier coefficients](../../../../../fourier-coefficient.md) and of $((2n+1)^{-1})_{n\in\mathbb Z}$.

For the convolution identity, fix any real $t$ and define $h_t(s)=\overline{g(t-s)}$. Periodicity makes $h_t\in L^2(-\pi,\pi)$ with $\|h_t\|_2=\|g\|_2$. A change of variable and integration over one full period give

$$
\langle e_n,h_t\rangle=\frac1{\sqrt{2\pi}}\int_{-\pi}^{\pi}e^{ins}g(t-s)ds=e^{int}\langle g,e_n\rangle.
$$

Applying polarized [Parseval identity](../../../../../parseval-identity.md) to $f,h_t$ gives, for every fixed $t$,

$$
\boxed{\int_{-\pi}^{\pi}f(s)g(t-s)ds=\sum_{n\in\mathbb Z}\langle f,e_n\rangle\langle g,e_n\rangle e^{int}.}
$$

The integral exists by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). The same inequality gives $\sum_n|\langle f,e_n\rangle\langle g,e_n\rangle|\leq\|f\|_2\|g\|_2$, so the displayed series converges absolutely and uniformly in $t$. In particular the equality holds at every $t$, without requiring [pointwise](../../../../../pointwise-convergence.md) [convergence](../../../../../convergence.md) of either original [Fourier series](../../../../../fourier-series-split.md). This is [Fourier convolution of two periodic L2 functions](../../../../../fourier-convolution-of-two-periodic-l2-functions.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
