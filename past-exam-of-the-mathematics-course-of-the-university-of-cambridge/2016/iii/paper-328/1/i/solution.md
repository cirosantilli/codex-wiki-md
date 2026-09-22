<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $a=\alpha/2$ and apply the [Dirichlet gauge transform for constant drift](../../../../../../dirichlet-gauge-transform-for-constant-drift.md) $w(x,t)=e^{ax}u(x,t)$. Taking [derivatives](../../../../../../derivative.md) directly removes the [advection](../../../../../../advection.md) term and gives the damped [heat equation](../../../../../../heat-equation.md) $w_t=w_{xx}-a^2w$. Thus $w_0(y)=e^{ay}u_0(y)$, while the two [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) become $w(0,t)=g_0(t)$ and $w(L,t)=e^{aL}h(t)$.

The [Dirichlet heat kernel on an interval](../../../../../../dirichlet-heat-kernel-on-an-interval.md) and its damped version are

$$
H_L(x,y,\tau)=\frac2L\sum_{n=1}^{\infty}e^{-q_n^2\tau}\sin(q_nx)\sin(q_ny),\qquad q_n=\frac{n\pi}{L},\qquad K_a=e^{-a^2\tau}H_L.
$$

The [method of images](../../../../../../method-of-images.md) gives an alternative, often better at short times:

$$
H_L(x,y,\tau)=\sum_{j\in\mathbb Z}\left[\frac{e^{-(x-y+2jL)^2/(4\tau)}}{\sqrt{4\pi\tau}}-\frac{e^{-(x+y+2jL)^2/(4\tau)}}{\sqrt{4\pi\tau}}\right].
$$

To determine the boundary signs, multiply the equation for $w$ by the backward [heat kernel](../../../../../../heat-kernel.md) $K_a(x,y,t-s)$ and use [integration by parts](../../../../../../integration-by-parts.md) in $y$. Since the kernel vanishes at $y=0,L$, the surviving boundary expression is $K_{a,y}(x,0,t-s)g_0(s)-K_{a,y}(x,L,t-s)e^{aL}h(s)$. Consequently an [integral representation](../../../../../../integral-representation.md) containing only the given data is

$$
\boxed{u(x,t)=e^{-ax}\left\{\int_0^L K_a(x,y,t)e^{ay}u_0(y)\,dy+\int_0^t\left[K_{a,y}(x,0,t-s)g_0(s)-K_{a,y}(x,L,t-s)e^{aL}h(s)\right]ds\right\}.}
$$

This is a [Dirichlet boundary-forcing heat-kernel formula](../../../../../../dirichlet-boundary-forcing-heat-kernel-formula.md). For $0<x<L$ the short-time Gaussian decay makes the forcing integral well defined. The endpoint values are interior limits of the complete formula: evaluating a termwise sine series at an endpoint before taking the time integral loses the nonzero boundary values. At the initial corners a continuous classical solution requires $u_0(0)=g_0(0)$ and $u_0(L)=h(0)$; otherwise the same formula describes the solution away from those corners.

Here is a second [integral representation](../../../../../../integral-representation.md), useful when the [integral transforms](../../../../../../integral-transform.md) are explicit. Extend $g_0,h$ by zero after $T$; the values of the extension cannot affect a solution at $t<T$. Write their [Laplace transforms](../../../../../../laplace-transform.md) as $G(p),H(p)$ and set $q=\sqrt{p+a^2}$ using the [principal square root](../../../../../../principal-square-root-of-a-complex-number.md). The transformed [Dirichlet Green function](../../../../../../dirichlet-green-function.md) for $-\partial_x^2+q^2$ is

$$
R_q(x,y)=\frac{\sinh(q\min(x,y))\sinh(q[L-\max(x,y)])}{q\sinh(qL)}.
$$

It vanishes at both endpoints and its first [derivative](../../../../../../derivative.md) in $x$ jumps by $-1$, which verifies the sign of its unit source. The [resolvent kernel for Dirichlet advection-diffusion on an interval](../../../../../../resolvent-kernel-for-dirichlet-advection-diffusion-on-an-interval.md) gives the transformed solution

$$
W(x,p)=\int_0^L R_q(x,y)e^{ay}u_0(y)\,dy+\frac{\sinh(q[L-x])}{\sinh(qL)}G(p)+e^{aL}\frac{\sinh(qx)}{\sinh(qL)}H(p).
$$

The [Bromwich inversion formula](../../../../../../bromwich-inversion-formula.md) therefore yields

$$
\boxed{u(x,t)=\frac{e^{-ax}}{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}e^{pt}W(x,p)\,dp,\qquad\gamma>0.}
$$

The square-root notation creates no genuine branch singularity here: all three kernels are even in $q$. Their only spatial [resolvent operator](../../../../../../resolvent-of-an-operator.md) poles are $p=-a^2-q_n^2$. This transformed formula and the causal [heat kernel](../../../../../../heat-kernel.md) formula represent the same solution in the usual smooth-data class.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 328](../../../paper-328-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
