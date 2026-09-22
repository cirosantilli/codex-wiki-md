# Heat-kernel convergence from a conditionally convergent Gaussian integral

↑ **Parent:** [Heat-kernel solution](heat-kernel-solution.md)

Let $\varphi$ be continuous and suppose that the displayed [improper integral](improper-integral.md) converges separately at both infinite endpoints for some $T>0$. Absolute convergence is not required. Then its [heat-kernel solution](heat-kernel-solution.md) exists, is smooth and solves the [heat equation](heat-equation.md) for $0<t<T$, and tends to $\varphi(x)$ as $t\downarrow0$ at each fixed $x$.

To prove the smoothing claim, take a primitive $H$ of $\varphi(\xi)e^{-\xi^2/(4T)}$. The assumed convergence makes $H$ bounded. For $q(x,\xi,t)=K_t(x-\xi)e^{\xi^2/(4T)}$, [integration by parts](integration-by-parts.md) gives

$$
\int\varphi(\xi)K_t(x-\xi)\,d\xi=-\int H(\xi)q_\xi(x,\xi,t)\,d\xi.
$$

The endpoint term vanishes. The coefficient of $\xi^2$ in the exponent of $q$ is $-(T-t)/(4tT)<0$. Its [derivatives](derivative.md) therefore have Gaussian decay on every compact subset of $\mathbb R\times(0,T)$, justifying [differentiation under the integral sign](differentiation-under-the-integral-sign.md) in the absolutely convergent right-hand expression. Since $q_t=q_{xx}$, it satisfies the [heat equation](heat-equation.md).

For the initial limit, apply the same construction to $\varphi(\xi)-\varphi(x)$ and split at $|\xi-x|=\delta$. [Continuity](continuous-function.md) controls the local part by its small oscillation times the unit kernel mass. On each remaining tail, $q$ is monotone for sufficiently small $t$: its maximum lies at $\xi=xT/(T-t)$, approaching $x$. If the relevant primitive has absolute bound $M$, [integration by parts](integration-by-parts.md) bounds that tail by $2M$ times the value of $q$ at its finite endpoint. For either endpoint $\xi=x\pm\delta$, that value tends to zero like $t^{-1/2}e^{-\delta^2/(4t)}$ times a fixed constant. Both tails vanish, proving the limit. Separate endpoint convergence matters here; merely assuming a symmetric [Cauchy principal value](cauchy-principal-value.md) does not provide the bounded primitive used in this proof.

## ↑ Ancestors (9)

1. [Heat-kernel solution](heat-kernel-solution.md)
2. [Heat kernel](heat-kernel.md)
3. [Heat equation](heat-equation.md)
4. [Diffusion equation](diffusion-equation-split.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/20/b/solution.md)
