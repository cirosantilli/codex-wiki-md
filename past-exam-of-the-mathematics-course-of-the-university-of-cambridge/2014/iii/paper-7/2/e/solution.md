<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take the positive integer $n\geq1$ and put $m=n+1\geq2$. From the preceding estimate and the absent zero [Fourier mode](../../../../../../fourier-mode.md), for $t\ne0$,

$$
 \begin{aligned}
 \sum_{k\in\mathbb Z}|\widehat r_t(k)|
 &\leq\frac{\|\partial_v^m f_0\|_1}{(2\pi)^m|t|^m}
 \sum_{k\ne0}\frac1{|k|^m}\\
 &=\frac{2\zeta(m)\|\partial_v^m f_0\|_1}{(2\pi)^m|t|^m}.
 \end{aligned}
$$

Here $\zeta$ is the [Riemann zeta function](../../../../../../riemann-zeta-function.md), and its displayed series is finite because $m>1$. One may replace the last derivative [norm](../../../../../../norm.md) by the given full mixed [Sobolev norm](../../../../../../sobolev-norm.md) to obtain the requested constant depending only on $n$ and $f_0$.

An absolutely summable sequence of [Fourier coefficients](../../../../../../fourier-coefficient.md) gives a uniformly and absolutely convergent [Fourier series](../../../../../../fourier-series-split.md), with supremum bounded by the sum of their absolute values. Its sum agrees almost everywhere with $r_t$ by uniqueness of [Fourier coefficients](../../../../../../fourier-coefficient.md) for integrable periodic functions. Hence

$$
 \boxed{\|\rho_t-\rho_\infty\|_{L^\infty(\mathbb T)}
 \leq\frac{2\zeta(n+1)}{(2\pi)^{n+1}}
 \frac{\|\partial_v^{n+1}f_0\|_1}{|t|^{n+1}}
 \longrightarrow0.}
$$

This is the [uniform phase-mixing bound from velocity derivatives](../../../../../../uniform-phase-mixing-bound-from-velocity-derivatives.md): uniform convergence for the continuous representative of the density, with rate $O(|t|^{-n-1})$. No uniform decay of the full phase-space distribution is asserted. The [free-transport phase mixing](../../../../../../free-transport-phase-mixing.md) acts by shifting nonzero spatial modes to large velocity frequency. If a convention allows $0\in\mathbb N$, that endpoint needs separate assumptions or an argument: the harmonic series in this proof would diverge.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
