# Quadratic arch expansion in half-integer cosine modes

↑ **Parent:** [Fourier cosine series](fourier-cosine-series.md)

For $b>0$ and $-b\leq y\leq b$, the even [quadratic polynomial](quadratic-polynomial.md) $b^2-y^2$ has the displayed expansion in even [Dirichlet eigenfunctions](dirichlet-eigenfunction.md). Put $k_n=(2n+1)\pi/(2b)$. Their squared [norm](norm.md) on $[-b,b]$ is $b$. Two [integrations by parts](integration-by-parts.md), using $\cos(k_nb)=0$, give

$$
\int_{-b}^{b}(b^2-y^2)\cos(k_ny)\,dy
=\frac{2}{k_n}\int_{-b}^{b}y\sin(k_ny)\,dy
=\frac{4\sin(k_nb)}{k_n^3}.
$$

Division by $b$ gives the displayed [Fourier coefficients](fourier-coefficient.md). The cubic decay gives [uniform convergence](uniform-convergence.md). The half-integer frequencies arise from requiring both evenness and zero values at the endpoints, rather than from a periodic boundary condition. This expansion is useful in [rectangular duct flow](rectangular-duct-flow.md).

## ↑ Ancestors (6)

1. [Fourier cosine series](fourier-cosine-series.md)
2. [Fourier series](fourier-series-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-viscous-flow-course-of-the-university-of-oxford/2023/1/b/iii/solution.md)
