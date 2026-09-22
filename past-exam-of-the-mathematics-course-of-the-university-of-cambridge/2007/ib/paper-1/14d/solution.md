<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention

$$
\widetilde f(k)=\int_{\mathbb R}f(x)e^{-ikx}\,dx,\qquad
f(x)=\frac1{2\pi}\int_{\mathbb R}\widetilde f(k)e^{ikx}\,dk.
$$

Decay alone does not guarantee existence of the ordinary integrals, so impose the usual integrability and regularity assumptions. One sufficient version of the [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) is that $f$ and $\widetilde f$ are integrable and $f$ is [continuous](../../../../../continuous-function.md), in which case the inversion integral recovers $f$. Under the standard piecewise-smooth Dirichlet assumptions, inversion instead gives the midpoint of the two one-sided limits at a jump, with a suitable improper integral interpretation.

For integrable $f,g$, define $(f*g)(x)=\int_{\mathbb R}f(x-y)g(y)\,dy$. The [convolution theorem](../../../../../convolution-theorem.md) states

$$
\boxed{\widetilde{f*g}(k)=\widetilde f(k)\widetilde g(k).}
$$

To prove it, absolute integrability permits [Fubini's theorem](../../../../../fubini-s-theorem.md). Set $t=x-y$ in the inner integral:

$$
\begin{aligned}
\widetilde{f*g}(k)
&=\int_{\mathbb R}\int_{\mathbb R}f(x-y)g(y)e^{-ikx}\,dy\,dx\\
&=\int_{\mathbb R}g(y)e^{-iky}\,dy\int_{\mathbb R}f(t)e^{-ikt}\,dt.
\end{aligned}
$$

The absolute double integral is $\|f\|_1\|g\|_1$, justifying the interchange. The computations below assume $a,b>0$ and use the source PDF's factor $e^{ikx}$ in the final integral, omitted in the converted TeX.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
