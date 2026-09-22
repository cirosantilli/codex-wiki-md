<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $D=\sum_{k\in\mathbb Z}\delta_{2\pi k}$ be the [Dirac comb](../../../../../dirac-comb.md). Pair the given identity $D=(2\pi)^{-1}\sum_{n\in\mathbb Z}e^{in\cdot}$ with the [Schwartz function](../../../../../schwartz-function.md) $y\mapsto\phi(x-y)$. On the left this gives $\sum_k\phi(x-2\pi k)=P\phi(x)$. On the right,

$$
\int_{\mathbb R}e^{iny}\phi(x-y)\,dy
=e^{inx}\int_{\mathbb R}\phi(z)e^{-inz}\,dz
=e^{inx}\widehat\phi(n).
$$

Therefore the [Fourier series](../../../../../fourier-series-split.md) is

$$
\boxed{P\phi(x)=\frac1{2\pi}\sum_{n\in\mathbb Z}\widehat\phi(n)e^{inx}.}
$$

The [Fourier bounds for Schwartz functions](../../../../../fourier-bounds-for-schwartz-functions.md) imply $|\widehat\phi(n)|\leq C_N(1+|n|)^{-N}$ for every $N$. For each nonnegative integer $j$, choose $N>j+1$ to obtain $\sum_n|n|^j|\widehat\phi(n)|<\infty$. Thus the [Fourier series](../../../../../fourier-series-split.md) and every differentiated [Fourier series](../../../../../fourier-series-split.md) converge absolutely and uniformly on all of $\mathbb R$. In particular convergence holds in the topology of [smooth](../../../../../smooth-function.md) $2\pi$ [periodic functions](../../../../../periodic-function.md), defined by uniform convergence of every [derivative](../../../../../derivative.md) on one period, and also in [tempered distributions](../../../../../tempered-distribution.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
