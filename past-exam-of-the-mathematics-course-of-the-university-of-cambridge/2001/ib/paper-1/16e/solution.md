<h1 id="16e/solution">Solution</h1>

↑ **Parent:** [16E](../16e.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat F(k)=\int_{\mathbb R}F(x)e^{-ikx}\,dx$. First compute the [Fourier coefficients](../../../../../fourier-coefficient.md) of the periodized sum. Absolute integrability gives

$$
\sum_{j\in\mathbb Z}\int_0^{2\pi}|F(2\pi j+\tau)|\,d\tau=\int_{\mathbb R}|F(x)|\,dx<\infty.
$$

Thus [Fubini's theorem](../../../../../fubini-s-theorem.md) justifies termwise integration. For integer $m$, the change of variable $x=2\pi j+\tau$ and $e^{2\pi imj}=1$ give

$$
c_m=\frac1{2\pi}\int_0^{2\pi}f(\tau)e^{-im\tau}\,d\tau
=\frac1{2\pi}\sum_j\int_{2\pi j}^{2\pi(j+1)}F(x)e^{-imx}\,dx
=\boxed{\frac{\widehat F(m)}{2\pi}}.
$$

Reindexing a convergent periodization gives periodicity; the [integral](../../../../../integral.md) argument always gives its periodic representative almost everywhere. This proves the Fourier-coefficient content of the [Poisson summation formula](../../../../../poisson-summation-formula.md).

There is a genuine qualification to the printed pointwise claim: the [periodization of an integrable function](../../../../../periodization-of-an-integrable-function.md) need not agree pointwise with its [Fourier series](../../../../../fourier-series-split.md) under the stated hypotheses alone. Set $F(0)=1$ and $F(x)=0$ for $x\ne0$. This is absolutely integrable, and on one closed period the periodization has only two possibly nonzero summands, so the series is uniformly convergent. Yet $f(0)=1$, while $\widehat F(m)=0$ for every $m$. The claimed pointwise equality at zero is therefore false. This counterexample also works for Riemann integrability, not only for an almost-everywhere convention.

The coefficient identity gives a rigorous general replacement: the weighted [Fejér sums](../../../../../fejer-sum.md)

$$
\sigma_Nf(\tau)=\frac1{2\pi}\sum_{|m|\leq N}\left(1-\frac{|m|}{N+1}\right)\widehat F(m)e^{im\tau}
$$

converge to the periodization in the [integral](../../../../../integral.md) norm, and at every [continuity](../../../../../continuous-function.md) point. Indeed they are its convolution with the normalized [Fejér kernel](../../../../../fejer-kernel.md); that kernel is nonnegative, has [integral](../../../../../integral.md) one, and has [integral](../../../../../integral.md) tending to zero outside every fixed neighbourhood of zero. For convergence in the [L1 norm](../../../../../l1-norm.md), split the convolution error into small translations, controlled by [continuity](../../../../../continuous-function.md) of translation in the [integral](../../../../../integral.md) norm, and the remaining tail. The same split gives [pointwise convergence](../../../../../pointwise-convergence.md) at a [continuity](../../../../../continuous-function.md) point. If the periodization is piecewise continuously differentiable, the ordinary [Fourier series](../../../../../fourier-series-split.md) has the usual midpoint limit; if it is continuous and its coefficients are absolutely summable, the displayed unweighted formula holds pointwise. These are sufficient interpretations of the intended identity.

For the specified exponential example all the needed [Fourier series](../../../../../fourier-series-split.md) convergence properties do hold. Split its [Fourier transform](../../../../../fourier-transform.md) at zero to obtain

$$
\widehat F(k)=\int_0^\infty e^{-(1+ik)x}\,dx+\int_0^\infty e^{-(1-ik)x}\,dx
=\frac{2}{1+k^2}.
$$

Its periodization is continuous, with uniformly geometrically bounded tails, and the sampled coefficients are absolutely summable. The absolutely summable coefficients define a uniformly convergent [Fourier series](../../../../../fourier-series-split.md) with the computed coefficients. Its continuous sum equals the continuous periodization: their difference has every [Fourier coefficient](../../../../../fourier-coefficient.md) zero, hence is zero in the [L2 norm](../../../../../l2-norm.md) by Fourier completeness, and continuity upgrades that to equality everywhere. Therefore its ordinary [Poisson summation formula](../../../../../poisson-summation-formula.md) is valid. Evaluate it at zero:

$$
\sum_{j\in\mathbb Z}e^{-2\pi|j|}=1+\frac{2e^{-2\pi}}{1-e^{-2\pi}}=\coth\pi
=\frac1\pi\sum_{n\in\mathbb Z}\frac1{1+n^2}.
$$

Thus the fully justified requested sum is

$$
\boxed{\sum_{n=-\infty}^{\infty}\frac1{1+n^2}=\pi\coth\pi}.
$$

## ↑ Ancestors (10)

1. [16E](../16e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
