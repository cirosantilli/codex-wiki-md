<h1 id="36d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [geodesic Lagrangian](../../../../../../geodesic-lagrangian.md)

$$
\mathcal L=\frac12\left(
-\lambda^2\dot t^{\,2}
+\mu^2\dot r^{\,2}
+r^2\dot\theta^{\,2}
+r^2\sin^2\theta\,\dot\phi^{\,2}
\right),
$$

where here the overdot on a coordinate means differentiation with respect to the affine parameter. Applying the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) to each coordinate and comparing with the [geodesic equation](../../../../../../geodesic-equation.md)

$$
\ddot x^\alpha+\Gamma^\alpha_{\beta\gamma}
\dot x^\beta\dot x^\gamma=0
$$

determines the [Christoffel symbols](../../../../../../christoffel-symbol.md). To display derivatives of the metric coefficients unambiguously, write $\lambda_t=\partial_t\lambda$, $\lambda_r=\partial_r\lambda$, and similarly for $\mu$. The nonzero symbols, together with those obtained by symmetry in the two lower indices, are

$$
\boxed{
\begin{aligned}
&\Gamma^t_{tt}=\frac{\lambda_t}{\lambda},
&&\Gamma^t_{tr}=\Gamma^t_{rt}=\frac{\lambda_r}{\lambda},
&&\Gamma^t_{rr}=\frac{\mu\mu_t}{\lambda^2},\\
&\Gamma^r_{tt}=\frac{\lambda\lambda_r}{\mu^2},
&&\Gamma^r_{tr}=\Gamma^r_{rt}=\frac{\mu_t}{\mu},
&&\Gamma^r_{rr}=\frac{\mu_r}{\mu},\\
&\Gamma^r_{\theta\theta}=-\frac r{\mu^2},
&&\Gamma^r_{\phi\phi}=-\frac{r\sin^2\theta}{\mu^2},\\
&\Gamma^\theta_{r\theta}=\Gamma^\theta_{\theta r}=\frac1r,
&&\Gamma^\theta_{\phi\phi}=-\sin\theta\cos\theta,\\
&\Gamma^\phi_{r\phi}=\Gamma^\phi_{\phi r}=\frac1r,
&&\Gamma^\phi_{\theta\phi}=\Gamma^\phi_{\phi\theta}=\cot\theta.
\end{aligned}}
$$

This is the [Christoffel symbols of a diagonal spherical spacetime metric](../../../../../../christoffel-symbols-of-a-diagonal-spherical-spacetime-metric.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [36D](../../36d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
