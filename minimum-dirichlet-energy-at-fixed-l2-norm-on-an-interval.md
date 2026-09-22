# Minimum Dirichlet energy at fixed L2 norm on an interval

↑ **Parent:** [Wirtinger inequality](wirtinger-inequality.md)

Expand a real function with zero endpoint values in its [Fourier sine series](fourier-sine-series.md), $y=\sum_{n\geq1}a_n\sin(n\pi x/L)$. The [Parseval identity](parseval-identity.md) gives $\int y^2=(L/2)\sum a_n^2$. For its [weak derivative](weak-derivative.md), the [Fourier cosine series](fourier-cosine-series.md) has coefficients $(n\pi/L)a_n$ and zero constant term, so

$$
\int_0^L|y'|^2\,dx=\frac L2\sum_{n\geq1}\left(\frac{n\pi}L\right)^2a_n^2
\geq\frac{\pi^2}{L^2}\int_0^Ly^2\,dx.
$$

The derivative coefficient identity follows by [integration by parts](integration-by-parts.md), rather than by assuming pointwise differentiation of an arbitrary series. This proves the [Wirtinger inequality](wirtinger-inequality.md) and its equality case. Under unit [L2 norm](l2-norm.md), the only real minimizers are $y=\pm\sqrt{2/L}\sin(\pi x/L)$.

## ↑ Ancestors (7)

1. [Wirtinger inequality](wirtinger-inequality.md)
2. [Second variation](second-variation.md)
3. [Calculus of variations](calculus-of-variations-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2017/6/b/iv/solution.md)
