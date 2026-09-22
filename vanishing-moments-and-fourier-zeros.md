# Vanishing moments and Fourier zeros

↑ **Parent:** [Vanishing moment](vanishing-moment.md)

Use the [Fourier transform](fourier-transform.md) convention $\widehat\psi(\omega)=\int\psi(x)e^{-i\omega x}\,dx$. If $ψ$ and $x^r\psi$ for $r<q$ are [integrable functions](lebesgue-integrable-function.md), [moment differentiation of the Fourier transform](moment-differentiation-of-the-fourier-transform.md) yields a $C^{q-1}$ [Fourier transform](fourier-transform.md) and

$$
\widehat\psi^{(r)}(0)=(-i)^r\int_{\mathbb R}x^r\psi(x)\,dx,\qquad 0\leq r<q.
$$

The [dominated convergence theorem](dominated-convergence-theorem.md) justifies these [derivatives](derivative.md). Under these assumptions, $q$ [vanishing moments](vanishing-moment.md) are equivalent to vanishing [derivatives](derivative.md) through order $q-1$ at zero. For $q>1$ this gives a [Peano zero](peano-zero.md) $\widehat\psi(\omega)=o(|\omega|^{q-1})$; for $q=1$ it gives $\widehat\psi(\omega)=o(1)$. It does not by itself justify a $q$th [derivative](derivative.md) or an $O(|\omega|^q)$ estimate.

If also $\int|x|^q|\psi(x)|\,dx<\infty$, subtract the degree-$(q-1)$ [Taylor polynomial](taylor-polynomial.md) of $e^{-i\omega x}$ inside the [integral](integral.md). Its [Taylor remainder](taylor-remainder.md) gives the stronger bound

$$
|\widehat\psi(\omega)|\leq\frac{|\omega|^q}{q!}\int_{\mathbb R}|x|^q|\psi(x)|\,dx.
$$

For an [integrable function](lebesgue-integrable-function.md) with [compact support](compact-support.md), every weighted [integral](integral.md) exists and its [Fourier transform](fourier-transform.md) extends to an [entire function](entire-function.md). The language “zero of order at least $q$” is then literal [analytic function](holomorphic-function.md) terminology. If the next [integral](integral.md) is nonzero, the order is exactly $q$. The [smooth-mask vanishing-moment criterion](smooth-mask-vanishing-moment-criterion.md) relates these cancellations to a refinement mask under its additional hypotheses.[Wavelet Bases, §7.2.1, printed p. 206, Theorem 7.4 and proof of (i) ⇔ (ii): decay assumptions and differentiation of the Fourier transform](a-wavelet-tour-of-signal-processing-by-stephane-mallat/wavelet-bases.md)

## ↑ Ancestors (7)

1. [Vanishing moment](vanishing-moment.md)
2. [Wavelet](wavelet.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
