<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

For the [heat kernel](../../../../../heat-kernel.md)

$$
K(x,t)=(4\pi t)^{-1/2}e^{-x^2/(4t)},
$$

direct [partial differentiation](../../../../../partial-derivative.md) gives

$$
K_t=\left(-\frac1{2t}+\frac{x^2}{4t^2}\right)K
=K_{xx}.
$$

Thus $K$ solves the [heat equation](../../../../../heat-equation.md). For bounded continuous $f$, [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) gives

$$
u_t=\int_{-\infty}^{\infty}K_t(x-y,t)f(y)\,dy
=\int_{-\infty}^{\infty}K_{xx}(x-y,t)f(y)\,dy=u_{xx}.
$$

With $Y=(x-y)/\sqrt{4t}$,

$$
u(x,t)=\frac1{\sqrt\pi}\int_{-\infty}^{\infty}
e^{-Y^2}f(x-2\sqrt t\,Y)\,dY.
$$

The [Gaussian integral](../../../../../gaussian-integral.md) makes the weight have total mass one, and the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives $u(x,t)\to f(x)$. This is the [Gaussian approximate identity](../../../../../gaussian-approximate-identity.md).

For the [viscous Burgers equation](../../../../../viscous-burgers-equation.md) with unit viscosity, the [Cole-Hopf transformation](../../../../../cole-hopf-transformation.md) $w=-2u_x/u$ reduces the equation to $u_t=u_{xx}$. To obtain initial value $g$, choose

$$
f(x)=\exp\left[-\frac12\int_0^x g(s)\,ds\right]
$$

(up to an irrelevant positive constant), and set $u=K_t*f$. Therefore

$$
\boxed{w(x,t)=-2\,\partial_x\log\!\left[
\int_{-\infty}^{\infty}K(x-y,t)f(y)\,dy
\right]}.
$$

Equivalently,

$$
w(x,t)=\frac1t
\frac{\int (x-y)K(x-y,t)f(y)\,dy}
{\int K(x-y,t)f(y)\,dy},
$$

and the approximate-identity limit gives $w(x,t)\to g(x)$.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
