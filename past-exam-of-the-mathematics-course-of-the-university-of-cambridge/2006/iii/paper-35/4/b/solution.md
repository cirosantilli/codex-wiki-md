<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Itô product rule](../../../../../../ito-product-rule.md) with a deterministic [integrating factor](../../../../../../integrating-factor.md) gives

$$
d(e^{-t}X_t)=e^{-t}dX_t-e^{-t}X_tdt=e^{-t}dB_t.
$$

Integrating from zero proves

$$
\boxed{X_t=e^t\int_0^t e^{-s}dB_s.}
$$

Both coefficients are globally [Lipschitz](../../../../../../lipschitz-continuity.md), so part (a) proves that this is the pathwise unique solution. Under a measure where $B$ is a [Brownian motion](../../../../../../brownian-motion-split.md), the solution is centered [Gaussian](../../../../../../normal-distribution.md) with variance $e^{2t}\int_0^te^{-2s}ds=(e^{2t}-1)/2$. The positive drift sign gives an unstable linear diffusion rather than a mean-reverting one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
