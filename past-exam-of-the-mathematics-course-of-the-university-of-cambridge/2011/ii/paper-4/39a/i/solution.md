<h1 id="39a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For period two in each direction, use [Fourier coefficients](../../../../../../fourier-coefficient.md)

$$
f_k=\frac14\int_{-1}^1\int_{-1}^1f(x,y)e^{-i\pi(k_1x+k_2y)}\,dx\,dy,\qquad k\in\mathbb Z^2.
$$

Integration of the periodic [Poisson equation](../../../../../../poisson-equation.md) gives the necessary compatibility condition $f_0=0$. With it, the normalization fixes $u_0=0$ and every other [Fourier mode](../../../../../../fourier-mode.md) gives $-\pi^2|k|^2u_k=f_k$. The Fourier-Galerkin approximation is therefore

$$
\boxed{u_N(x,y)=-\sum_{\substack{|k_1|,|k_2|\le N\\k\ne0}}\frac{f_k}{\pi^2|k|^2}e^{i\pi(k_1x+k_2y)}.}
$$

One may evaluate the coefficients by a [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) for a pseudospectral implementation, with the corresponding quadrature/aliasing error distinguished from truncation.

Convergence with [spectral accuracy](../../../../../../spectral-accuracy.md) means faster decay than every fixed algebraic power of $N$. A smooth periodic extension gives this rate; an analytic periodic extension to a complex strip gives the stronger exponential rate $O(e^{-cN})$ on a slightly narrower strip. Division by $|k|^2$ preserves that Fourier decay, so the normalized solution has the same type of spectral convergence.

**Two qualifications are required by the literal source assumptions.** The mean-zero condition on $f$ was not stated: $f\equiv1$ meets the printed analyticity and endpoint equalities but has no periodic solution. Also endpoint equality of $f$ alone does not make its periodic extension analytic. For example $f(x,y)=x^2-1/3$ is analytic, has matching endpoint values and zero mean, but its nonzero [Fourier coefficients](../../../../../../fourier-coefficient.md) are $f_{(k,0)}=2(-1)^k/(\pi^2k^2)$. Then $u_{(k,0)}=-2(-1)^k/(\pi^4k^4)$, with only algebraic decay. Thus the standard spectral-speed conclusion is valid under the intended analytic-periodic torus assumption and compatibility, not for every function satisfying only the displayed endpoint values.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
