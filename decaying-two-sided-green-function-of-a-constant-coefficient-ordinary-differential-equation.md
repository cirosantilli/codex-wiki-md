# Decaying two-sided Green function of a constant-coefficient ordinary differential equation

↑ **Parent:** [Green's function](green-s-function-split.md)

Let $p(D)$ be a constant-coefficient differential operator, $D=d/dt$, with distinct characteristic roots $\lambda_j$ having nonzero real parts. The solution of $p(D)K=\delta$ decaying at both temporal infinities is

$$
K(t)=H(t)\sum_{\operatorname{Re}\lambda_j<0}\frac{e^{\lambda_jt}}{p'(\lambda_j)}-H(-t)\sum_{\operatorname{Re}\lambda_j>0}\frac{e^{\lambda_jt}}{p'(\lambda_j)},
$$

where $H$ is the [Heaviside step function](heaviside-step-function.md). This follows by [partial fraction decomposition](partial-fraction-decomposition.md) of $1/p(z)$ and the first-order kernels $e^{\lambda t}H(t)$ for $\operatorname{Re}\lambda<0$, or $-e^{\lambda t}H(-t)$ for $\operatorname{Re}\lambda>0$. Both first-order kernels jump by one and solve $(D-\lambda)K_\lambda=\delta$ as [distributions](distribution-mathematical-analysis.md).

For example, $p(D)=(D+1)(D-2)(D+2)$ gives

$$
K(t)=\begin{cases}-e^{2t}/12,&t<0,\\-e^{-t}/3+e^{-2t}/4,&t>0.\end{cases}
$$

It is continuous together with its first derivative; its second derivative jumps by one, as required by the [jump conditions for a third-order Green function](jump-conditions-for-a-third-order-green-function.md). A solution of $p(D)y=f$ is the [convolution](convolution.md) $K*f$ when it exists. If positive-real-part roots occur, decay at both ends generally requires a nonzero negative-time branch: this is the distinction captured by [causality versus stability of a Green function](causality-versus-stability-of-a-green-function.md). A causal kernel would retain growing positive-time terms and need not have a real-axis [Fourier transform](fourier-transform-split.md).

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/5/c/solution.md)
