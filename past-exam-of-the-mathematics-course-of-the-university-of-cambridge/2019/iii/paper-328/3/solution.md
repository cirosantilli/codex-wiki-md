<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Apply the time [Laplace transform](../../../../../laplace-transform.md) to the [Airy equation](../../../../../airy-equation.md). Extend $g$ past $T$ in any suitable way and write

$$
U(x,p)=\int_0^\infty e^{-pt}u(x,t)dt,\qquad G(p)=\int_0^\infty e^{-pt}g(t)dt.
$$

For example, setting $g=0$ after $T$ makes $G(p)=\int_0^T e^{-pt}g(t)dt$; the final solution for $t<T$ is independent of this extension. The [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md) gives

$$
U_{xxx}+pU=u_0(x),\qquad U_x(0,p)=G(p).
$$

Take the [principal cube root](../../../../../principal-cube-root.md) $\lambda=p^{1/3}$ for $\operatorname{Re}p>0$. The three [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) of the spatial [ordinary differential equation](../../../../../ordinary-differential-equation.md) are

$$
-\lambda,\qquad r_1=\lambda e^{i\pi/3},\qquad r_2=\lambda e^{-i\pi/3}.
$$

Since $|\arg\lambda|<\pi/6$, only $-\lambda$ has negative [real part](../../../../../real-part.md). Thus spatial decay leaves just one homogeneous exponential, which the single prescribed [Neumann boundary condition](../../../../../neumann-boundary-condition.md) determines.

The [Airy resolvent kernel](../../../../../airy-resolvent-kernel.md) on the whole real line is

$$
R_p(s)=\begin{cases}
\displaystyle\frac{e^{-\lambda s}}{3\lambda^2},&s\geq0,\\
\displaystyle-\frac{e^{r_1s}}{3r_1^2}-\frac{e^{r_2s}}{3r_2^2},&s<0.
\end{cases}
$$

It decays at both ends, is continuous together with its first [derivative](../../../../../derivative.md), and satisfies $R_p''(0+)-R_p''(0-)=1$. Consequently $(\partial_s^3+p)R_p=\delta_0$ as a [distribution](../../../../../distribution-mathematical-analysis.md). A particular solution is the [Green-function representation](../../../../../green-function-representation.md)

$$
V(x,p)=\int_0^\infty R_p(x-y)u_0(y)\,dy.
$$

Adding the decaying homogeneous mode to impose the boundary derivative gives

$$
U(x,p)=V(x,p)+\frac{e^{-\lambda x}}\lambda\left[V_x(0,p)-G(p)\right],
\qquad
V_x(0,p)=\int_0^\infty R_p'(-y)u_0(y)\,dy.
$$

Every term is known. If $\widetilde u_0(r)=\int_0^\infty e^{-ry}u_0(y)dy$ denotes the spatial [Laplace transform](../../../../../laplace-transform.md), then

$$
V_x(0,p)=-\frac13\left[\frac{\widetilde u_0(r_1)}{r_1}+\frac{\widetilde u_0(r_2)}{r_2}\right].
$$

The [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) now gives the required [integral representation](../../../../../integral-representation.md):

$$
\boxed{u(x,t)=\frac1{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}e^{pt}\left\{\int_0^\infty R_p(x-y)u_0(y)\,dy+\frac{e^{-p^{1/3}x}}{p^{1/3}}\left[\int_0^\infty R_p'(-y)u_0(y)\,dy-G(p)\right]\right\}dp.}
$$

Here $\gamma>0$ is to the right of any singularities required by the growth of the data. The usual decay or growth hypotheses are understood for this [Laplace transform](../../../../../laplace-transform.md) construction; when absolute inversion is unavailable, the vertical integral is interpreted as the limit of truncated [Bromwich contours](../../../../../bromwich-contour.md). The transformed [ordinary differential equation](../../../../../ordinary-differential-equation.md) verifies the [partial differential equation](../../../../../partial-differential-equation-split.md) and [initial condition](../../../../../initial-condition.md), while differentiating at $x=0$ gives exactly $G(p)$ and hence $u_x(0,t)=g(t)$. The derivative compatibility $u_0'(0)=g(0)$ makes the two data agree at the corner.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
