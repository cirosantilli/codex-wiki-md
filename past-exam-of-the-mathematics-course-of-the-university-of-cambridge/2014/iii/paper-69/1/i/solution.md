<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [spectral parameter for a linear boundary value problem](../../../../../../spectral-parameter-for-a-linear-boundary-value-problem.md) $k\in\mathbb C$ and define the [dispersion relation](../../../../../../dispersion-relation.md) $\omega(k)=k^2-i\alpha k$. Direct differentiation gives the [divergence form](../../../../../../divergence-form.md)

$$
\boxed{\partial_t(e^{-ikx+\omega t}u)-\partial_x\left(e^{-ikx+\omega t}[u_x+(ik+\alpha)u]\right)=0.}
$$

Indeed the coefficient of $u$ left over after expansion is $\omega-k^2+i\alpha k=0$, and the remaining factor is $u_t-u_{xx}-\alpha u_x$. Thus this is equivalent to the [advection-diffusion equation](../../../../../../advection-diffusion-equation.md) for every $k$.

Introduce the [Half-range Fourier transforms](../../../../../../half-range-fourier-transform.md) and [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md)

$$
\widehat u(k,t)=\int_0^\infty e^{-ikx}u(x,t)\,dx,\qquad
\widehat u_0(k)=\int_0^\infty e^{-ikx}u_0(x)\,dx,\qquad
G_j(k,t)=\int_0^t e^{\omega(k)s}g_j(s)\,ds,
$$

where $g_1(t)=u_x(0,t)$ is the unknown [normal derivative](../../../../../../normal-derivative.md) with the positive-$x$ convention. The outward normal at zero instead gives $-g_1$. The spatial transforms are analytic for $\operatorname{Im}k<0$ and continuous on the real axis under the stated decay assumptions. Integrating the [divergence form](../../../../../../divergence-form.md) on $(0,\infty)\times(0,t)$ gives the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md)

$$
\boxed{\widehat u_0(k)-e^{\omega(k)t}\widehat u(k,t)
=G_1(k,t)+(ik+\alpha)G_0(k,t),\qquad \operatorname{Im}k\leq0.}
$$

The sign follows from the lower spatial endpoint: the integrated spatial derivative is minus its value at zero. This sign will determine the boundary-forcing term in the solution.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
