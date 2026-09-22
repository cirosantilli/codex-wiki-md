<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the orthonormal [Fourier series](../../../../../../fourier-series-split.md) basis $e_n(x)=(2\pi)^{-1/2}e^{inx}$, indexed by $n\in\mathbb Z$, and the [Hilbert space](../../../../../../hilbert-space-split.md) [inner product](../../../../../../inner-product.md) $\langle f,g\rangle=\int_0^{2\pi}\overline{f(x)}g(x)dx$. The integral operator is a [periodic convolution operator](../../../../../../periodic-convolution-operator.md). Changing variables $s=x-x'$ and using periodicity gives

$$
(Ae_n)(x)=\frac{e^{inx}}{\sqrt{2\pi}}\int_0^{2\pi}K(s)e^{-ins}ds=c_n e_n(x).
$$

There is no extra factor $2\pi$: the paper's $c_n$ already includes the full integral, rather than its normalized Fourier-series coefficient. The adjoint kernel is $\overline{K(x'-x)}$, so $A^*e_n=\overline{c_n}e_n$.

A [singular system of a periodic convolution operator](../../../../../../singular-system-of-a-periodic-convolution-operator.md) is therefore

$$
\boxed{\sigma_n=|c_n|,\qquad v_n=e_n,\qquad u_n=\frac{c_n}{|c_n|}e_n\quad(n\in\mathbb Z).}
$$

Indeed $Av_n=\sigma_nu_n$ and $A^*u_n=(c_n/|c_n|)\overline{c_n}e_n=\sigma_nv_n$. The unit factor determined by the [complex argument](../../../../../../argument-complex-analysis.md) of $c_n$ in $u_n$ is necessary when the complex [Fourier coefficients](../../../../../../fourier-coefficient.md) are not positive real numbers. Both families are orthonormal and complete, since every $c_n\ne0$. One may enumerate $\mathbb Z$ by $\mathbb N$, or order the positive [singular values](../../../../../../singular-value.md) by decreasing magnitude.

The continuous kernel on a finite square makes $A$ a [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md), hence compact. Since $K$ is continuously differentiable and periodic, integration by parts gives, for $n\ne0$,

$$
c_n=\frac1{in}\int_0^{2\pi}K'(s)e^{-ins}ds=o(1/|n|)
$$

by the [Riemann-Lebesgue lemma](../../../../../../riemann-lebesgue-lemma.md). In particular the [singular values](../../../../../../singular-value.md) tend to zero. Nonzero multipliers imply both $\ker A=0$ and $\ker A^*=0$: the range is dense, but the inverse is unbounded and the range is not closed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
