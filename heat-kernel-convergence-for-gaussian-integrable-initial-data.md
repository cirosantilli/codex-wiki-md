# Heat-kernel convergence for Gaussian-integrable initial data

↑ **Parent:** [Heat-kernel solution](heat-kernel-solution.md)

Suppose $\varphi$ is continuous at $x$ and, for some $T>0$,

$$
\int_{\mathbb R}|\varphi(\xi)|e^{-\xi^2/(4T)}\,d\xi<\infty.
$$

For $0<t<T$, its [convolution](convolution.md) with the [heat kernel](heat-kernel.md) $K_t(s)=(4\pi t)^{-1/2}e^{-s^2/(4t)}$ is smooth and solves the [heat equation](heat-equation.md). On every [compact set](compact-space.md) in $\mathbb R\times(0,T)$, spatial or time [derivatives](derivative.md) of the [heat kernel](heat-kernel.md) are bounded by the displayed integrable weight times a constant: their [polynomial](polynomial-split.md) factors are absorbed by the strictly narrower Gaussian. This justifies [differentiation under the integral sign](differentiation-under-the-integral-sign.md).

Moreover, $\int K_t=1$, so

$$
(K_t*\varphi)(x)-\varphi(x)=\int K_t(x-\xi)\bigl(\varphi(\xi)-\varphi(x)\bigr)\,d\xi.
$$

Inside $|\xi-x|<\delta$, [continuity](continuous-function.md) makes the difference uniformly small. Outside that interval, for $t\leq T/4$, the inequality $\xi^2\leq2(\xi-x)^2+2x^2$ gives

$$
K_t(x-\xi)e^{\xi^2/(4T)}
\leq\frac{e^{x^2/(2T)}}{\sqrt{4\pi t}}e^{-\delta^2/(8t)}.
$$

The right side tends to zero, proving that the weighted tail contribution vanishes; the constant term $\varphi(x)$ is controlled by the vanishing Gaussian tail mass. Thus $(K_t*\varphi)(x)\to\varphi(x)$ as $t\downarrow0$. In particular, continuous data of [polynomial growth](polynomial-growth.md) satisfy this hypothesis, even when they are unbounded. This extends the [Gaussian approximate identity](gaussian-approximate-identity.md) argument beyond bounded data.

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

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/20/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/20/b/solution.md)
