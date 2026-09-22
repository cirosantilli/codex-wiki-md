<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $\widetilde\phi(x)=\overline{\phi(-x)}$. This is a [Schwartz function](../../../../../schwartz-function.md) and its [Fourier transform](../../../../../fourier-transform-split.md) is $\widehat{\widetilde\phi}(\xi)=\overline{\widehat\phi(\xi)}$. The [convolution theorem](../../../../../convolution-theorem.md) gives

$$
\widehat{\phi*\widetilde\phi}(\xi)=|\widehat\phi(\xi)|^2.
$$

The [convolution](../../../../../convolution.md) of two [Schwartz functions](../../../../../schwartz-function.md) is again a [Schwartz function](../../../../../schwartz-function.md): differentiating under the [integral](../../../../../integral-split.md) and expanding $x^m=(y+(x-y))^m$ bounds every weighted [derivative](../../../../../derivative.md) by products of integrable and bounded weighted [derivatives](../../../../../derivative.md). Evaluate [Fourier inversion](../../../../../fourier-inversion-theorem.md) for this [convolution](../../../../../convolution.md) at zero:

$$
\boxed{\int_{\mathbb R}|\phi(x)|^2\,dx
=(\phi*\widetilde\phi)(0)
=\frac1{2\pi}\int_{\mathbb R}|\widehat\phi(\xi)|^2\,d\xi.}
$$

The [Schwartz space](../../../../../schwartz-space.md) is dense in the [L2 space](../../../../../l2-space-is-a-hilbert-space.md). For $f\in L^2(\mathbb R)$ choose [Schwartz functions](../../../../../schwartz-function.md) $\phi_j\to f$ in the [L2 norm](../../../../../l2-norm.md). The identity makes $\widehat\phi_j$ a [Cauchy sequence](../../../../../cauchy-sequence.md) in the [L2 space](../../../../../l2-space-is-a-hilbert-space.md), and its limit defines $\mathcal Ff$, independently of the approximation. It agrees with the [distributional Fourier transform](../../../../../fourier-transform-of-a-tempered-distribution.md), because [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) makes convergence in the [L2 norm](../../../../../l2-norm.md) imply convergence when paired with every [Schwartz function](../../../../../schwartz-function.md). For $f\in L^1\cap L^2$ it therefore agrees [almost everywhere](../../../../../almost-everywhere.md) with the ordinary [Fourier transform](../../../../../fourier-transform-split.md).

The extension is onto: its image is closed by the norm identity and contains the [Schwartz space](../../../../../schwartz-space.md), since [Fourier inversion](../../../../../fourier-inversion-theorem.md) maps that space to itself. This proves [Plancherel theorem](../../../../../plancherel-theorem.md):

$$
\boxed{\|\mathcal Ff\|_2^2=2\pi\|f\|_2^2,\qquad
(2\pi)^{-1/2}\mathcal F:L^2(\mathbb R)\longrightarrow L^2(\mathbb R)\text{ is unitary}.}
$$

Its inverse is the extension of the [inverse Fourier transform](../../../../../inverse-fourier-transform.md), with limits understood in the [L2 norm](../../../../../l2-norm.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
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
