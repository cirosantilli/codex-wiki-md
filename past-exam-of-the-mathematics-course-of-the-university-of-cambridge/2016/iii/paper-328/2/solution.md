<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the printed coordinate derivative $u_x(0,t)$, not an outward [normal derivative](../../../../../normal-derivative.md); at the left endpoint these have opposite signs. Assume the usual bounded or admissibly growing solution at infinity, with an initial trace $b_0=u_0(0)$ and forcing possessing a [Laplace transform](../../../../../laplace-transform.md). Set $a=\alpha/2$, so $\beta=a^2$, and use $z=\sqrt p$ on the [principal square root](../../../../../principal-square-root-of-a-complex-number.md) branch. Define

$$
I(z)=\int_0^\infty e^{-zy}u_0(y)\,dy,\qquad F(p)=\int_0^\infty e^{-pt}f(t)\,dt.
$$

The half-line [Dirichlet Green function](../../../../../dirichlet-green-function.md) for $p-\partial_x^2$ gives

$$
U_D(x,p)=\int_0^\infty\frac{e^{-z|x-y|}-e^{-z(x+y)}}{2z}u_0(y)\,dy,\qquad U_D(0,p)=0,\qquad U_{D,x}(0,p)=I(z).
$$

Write the transformed solution as $U=U_D+e^{-zx}B(p)$. The [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md) in the dynamic [boundary condition](../../../../../boundary-condition.md) is $pB-b_0$, so

$$
(p+\beta)B-b_0+\alpha[I(z)-zB]=F(p).
$$

The special choice of $\beta$ gives the perfect square

$$
p-\alpha\sqrt p+\beta=(z-a)^2,\qquad \boxed{B(p)=\frac{F(p)+b_0-\alpha I(\sqrt p)}{(\sqrt p-a)^2}.}
$$

In particular, the initial boundary trace cannot be omitted. With

$$
K_D(x,y,t)=\frac{e^{-(x-y)^2/(4t)}-e^{-(x+y)^2/(4t)}}{\sqrt{4\pi t}},
$$

an [integral representation](../../../../../integral-representation.md) is

$$
\boxed{u(x,t)=\int_0^\infty K_D(x,y,t)u_0(y)\,dy+\frac1{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}e^{pt-x\sqrt p}\frac{F(p)+b_0-\alpha I(\sqrt p)}{(\sqrt p-a)^2}\,dp.}
$$

Choose the [Bromwich contour](../../../../../bromwich-contour.md) to the right of the forcing's growth abscissa and every pole; $\gamma>\max(0,a^2)$ and sufficiently large for the data is a safe choice for real $a$. No sign of $\alpha$ is explicitly imposed in this question.

The inverse transform can also be performed explicitly. For the [repeated-root dynamic-boundary heat kernel](../../../../../repeated-root-dynamic-boundary-heat-kernel.md), set

$$
J_a(x,t)=\mathcal L^{-1}\!\left\{\frac{e^{-x\sqrt p}}{(\sqrt p-a)^2}\right\}(t).
$$

First integrate the [Heat Poisson kernel](../../../../../heat-poisson-kernel.md) against $e^{ar}$, or differentiate the result with respect to $a$:

$$
\mathcal L^{-1}\!\left\{\frac{e^{-x\sqrt p}}{\sqrt p-a}\right\}=\frac{e^{-x^2/(4t)}}{\sqrt{\pi t}}+aE_a(x,t),\qquad E_a=e^{-ax+a^2t}\operatorname{erfc}\!\left(\frac{x}{2\sqrt t}-a\sqrt t\right).
$$

Since differentiation of $(\sqrt p-a)^{-1}$ with respect to $a$ produces $(\sqrt p-a)^{-2}$, and $\partial_aE_a=(-x+2at)E_a+2\sqrt{t/\pi}\,e^{-x^2/(4t)}$, the desired kernel is

$$
\boxed{J_a(x,t)=(1-ax+2a^2t)e^{-ax+a^2t}\operatorname{erfc}\!\left(\frac{x}{2\sqrt t}-a\sqrt t\right)+2a\sqrt{\frac t\pi}\,e^{-x^2/(4t)}.}
$$

Here $\operatorname{erfc}$ is the [complementary error function](../../../../../complementary-error-function.md). A direct integral characterization, also proving the sign and the transform, is

$$
J_a(x,t)=\int_0^\infty r e^{ar}\frac{x+r}{2\sqrt\pi\,t^{3/2}}e^{-(x+r)^2/(4t)}\,dr.
$$

The [convolution theorem for Laplace transforms](../../../../../convolution-theorem-for-laplace-transforms.md) now gives the fully real time-domain representation

$$
\boxed{u(x,t)=\int_0^\infty\left[K_D(x,y,t)-\alpha J_a(x+y,t)\right]u_0(y)\,dy+b_0J_a(x,t)+\int_0^tJ_a(x,t-s)f(s)\,ds.}
$$

All quantities here are known from the prescribed data. For $x>0$ it tends to $u_0(x)$ as $t\downarrow0$. At $x=0$, $J_a(0,t)\to1$ and the spatial correction tends to zero, recovering $b_0$. A solution classical through the initial corner additionally needs $u_0''(0)+\alpha u_0'(0)+a^2b_0=f(0)$; weaker corner regularity does not invalidate the formula for positive times.

The [repeated-root unstable heat boundary mode](../../../../../repeated-root-unstable-heat-boundary-mode.md) gives a useful sign check on the [dynamic boundary condition for the heat equation](../../../../../dynamic-boundary-condition-for-the-heat-equation.md). If $a>0$, $(\sqrt p-a)^2$ has a genuine double pole at $p=a^2$ on the physical branch, and the exact homogeneous mode $e^{-ax+a^2t}$ satisfies both the [heat equation](../../../../../heat-equation.md) and the printed boundary condition. Generic data can also excite a $t e^{a^2t}$ contribution. A contour deformation must retain this repeated-pole contribution. If $a<0$, the putative root $\sqrt p=a$ is outside the chosen branch and is not a physical pole. At $a=0$, $J_0=\operatorname{erfc}(x/(2\sqrt t))$, as expected when the boundary trace satisfies $b'(t)=f(t)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
