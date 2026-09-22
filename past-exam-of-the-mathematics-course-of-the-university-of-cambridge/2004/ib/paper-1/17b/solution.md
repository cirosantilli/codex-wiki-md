<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

The fixed-end [wave equation](../../../../../wave-equation-split.md) has spatial modes $\sin(n\pi x)$ and temporal factors $\cos(n\pi t),\sin(n\pi t)$. The zero initial velocity removes every temporal sine term. Expand the initial displacement in a [Fourier sine series](../../../../../fourier-sine-series.md), whose coefficients are

$$
b_n=2\int_0^1x(1-x)\sin(n\pi x)\,dx
=\frac{4[1-(-1)^n]}{\pi^3n^3}.
$$

Two integrations by parts give the last equality; the endpoint terms from $x(1-x)$ vanish and the remaining derivative endpoints distinguish even from odd $n$. Consequently

$$
\boxed{y(x,t)=\frac8{\pi^3}\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{\sin(n\pi x)\cos(n\pi t)}{n^3}.}
$$

This solves the initial-boundary problem in the finite-[energy](../../../../../energy.md) sense, with convergent first-derivative series. At $t=0$ the [energy](../../../../../energy.md) in the question is $\int_0^1(1-2x)^2dx=1/3$. At any time, sine/cosine [orthogonality](../../../../../orthogonal-vectors.md) gives the contribution of mode $n$ as $(n\pi)^2b_n^2/2$: its kinetic and elastic pieces have factors $\sin^2(n\pi t)$ and $\cos^2(n\pi t)$ summing to one. Therefore

$$
\frac13=\frac{32}{\pi^4}\sum_{\substack{n\geq1\\n\text{ odd}}}\frac1{n^4},\qquad
\boxed{\sum_{\substack{n\geq1\\n\text{ odd}}}n^{-4}=\frac{\pi^4}{96}.}
$$

The square summability of the derivative coefficients justifies the [orthogonality](../../../../../orthogonal-vectors.md) calculation and its limit.

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
