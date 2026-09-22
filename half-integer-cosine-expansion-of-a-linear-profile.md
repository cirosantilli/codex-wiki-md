# Half-integer cosine expansion of a linear profile

↑ **Parent:** [Fourier cosine series](fourier-cosine-series.md)

For $L>0$ and $0\leq x\leq L$, set $\mu_n=(2n+1)\pi/(2L)$. The [cosine](cosine.md) modes satisfy a homogeneous [Neumann boundary condition](neumann-boundary-condition.md) at zero and a homogeneous [Dirichlet boundary condition](dirichlet-boundary-condition.md) at $L$. Their squared [norm](norm.md) is $L/2$, and [integration by parts](integration-by-parts.md) gives

$$
\int_0^L(L-x)\cos(\mu_nx)\,dx=\frac{1-\cos(\mu_nL)}{\mu_n^2}=\frac1{\mu_n^2}.
$$

Thus their [Fourier coefficients](fourier-coefficient.md) are $2/(L\mu_n^2)$, proving the displayed formula by [Sturm-Liouville theory](sturm-liouville-theory-split.md). One can also obtain completeness by extending evenly across zero and oddly across $L$: the resulting continuous $4L$-[periodic extension](periodic-extension.md) has only odd-index [cosine](cosine.md) modes. The $n^{-2}$ coefficient bound proves [uniform convergence](uniform-convergence.md), including both endpoints. This expansion supplies the initial transient for a [heat equation](heat-equation.md) with mixed endpoint conditions.

## ↑ Ancestors (6)

1. [Fourier cosine series](fourier-cosine-series.md)
2. [Fourier series](fourier-series-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2023/prelims/mathematics-v/5/b/ii/solution.md)
