<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The truncated [Fourier cosine series](../../../../../../../fourier-cosine-series.md) gives the better approximation over the whole closed interval. Its [Fourier coefficients](../../../../../../../fourier-coefficient.md) obey $|a_n|\leq4/(\pi n^2)$, so [absolute convergence](../../../../../../../absolute-convergence.md) and the tail bound

$$
\boxed{\sup_{0\leq x\leq\pi}|f(x)-C_N(x)|
\leq\frac4\pi\sum_{n>N}\frac1{n^2}
\leq\frac4{\pi N}}
$$

give [uniform convergence](../../../../../../../uniform-convergence.md). The even [periodic extension](../../../../../../../periodic-extension.md) is continuous; its slope changes only cause corners.

By contrast $b_n=(-1)^{n+1}/n+O(n^{-2})$. The odd [periodic extension](../../../../../../../periodic-extension.md) has a jump at $\pi$, giving slower coefficient decay and the [Gibbs phenomenon](../../../../../../../gibbs-phenomenon.md) near that endpoint. Every truncated [Fourier sine series](../../../../../../../fourier-sine-series.md) satisfies $S_N(\pi)=0$, so

$$
\boxed{|f(\pi)-S_N(\pi)|=\pi/2\quad\text{for every }N.}
$$

It therefore cannot converge uniformly to $f$ on $[0,\pi]$, although it converges at every point of $[0,\pi)$. This comparison concerns approximation across the interval; it does not assert that the cosine truncation has smaller error at every individual interior point for every $N$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
