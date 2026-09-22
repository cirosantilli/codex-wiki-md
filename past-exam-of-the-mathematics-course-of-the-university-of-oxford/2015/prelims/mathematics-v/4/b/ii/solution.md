<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First, the [Fourier coefficients](../../../../../../../fourier-coefficient.md) of the [Fourier cosine series](../../../../../../../fourier-cosine-series.md) decay as $O(n^{-2})$, whereas those of the [Fourier sine series](../../../../../../../fourier-sine-series.md) are of order $n^{-1}$. In particular, the [absolute convergence](../../../../../../../absolute-convergence.md) bound for the [Fourier cosine series](../../../../../../../fourier-cosine-series.md) gives a uniform tail estimate

$$
\sup_{0\leq x\leq L}|g(x)-C_N(x)|
\leq2(e+1)\sum_{n>N}\frac1{1+n^2\pi^2}=O(N^{-1}).
$$

Thus its tail is absolutely controlled using fewer [Fourier harmonics](../../../../../../../fourier-harmonic.md). The [Fourier sine series](../../../../../../../fourier-sine-series.md) does not have an absolutely summable sequence of [Fourier coefficients](../../../../../../../fourier-coefficient.md).

Second, the [even extension](../../../../../../../even-extension.md) is continuous, so its [Fourier cosine series](../../../../../../../fourier-cosine-series.md) converges uniformly on the closed interval and approximates the nonzero endpoint limits correctly. The [odd periodic extension](../../../../../../../odd-periodic-extension.md) has jumps, producing the [Gibbs phenomenon](../../../../../../../gibbs-phenomenon.md) in its [Fourier sine series](../../../../../../../fourier-sine-series.md) near zero and $L$. Every [Fourier sine series](../../../../../../../fourier-sine-series.md) [partial sum](../../../../../../../partial-sum.md) is zero at both endpoints, so by approaching $L$ from inside $(0,L)$ one obtains

$$
\sup_{0<x<L}|g(x)-S_N(x)|\geq e.
$$

Hence the [Fourier sine series](../../../../../../../fourier-sine-series.md) approximation cannot converge uniformly even on the whole open interval, despite [pointwise convergence](../../../../../../../pointwise-convergence.md) at each interior point. **The [Fourier cosine series](../../../../../../../fourier-cosine-series.md) approximation has faster [coefficient decay](../../../../../../../fourier-coefficient-decay.md) and avoids the persistent errors near the endpoints.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
