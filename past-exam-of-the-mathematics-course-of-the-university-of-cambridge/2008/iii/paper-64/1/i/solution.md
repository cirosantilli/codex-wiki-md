<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\rho=\bar\rho(1+\delta)$, take a constant barotropic equation-of-state parameter $w$, and keep first-order terms in $\delta$, $v^i$ and $h_{ij}$. In [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md), the inverse metric is $g^{00}=-a^{-2}$, $g^{0i}=0$, $g^{ij}=a^{-2}(\delta^{ij}-h^{ij})$. The normalization $u^\mu u_\mu=-1$ gives $u^0=a^{-1}+O(v^2)$ and $u^i=a^{-1}v^i$. Substitution in the [perfect fluid](../../../../../../perfect-fluid.md) stress tensor gives the [linear perfect-fluid stress tensor in synchronous gauge](../../../../../../linear-perfect-fluid-stress-tensor-in-synchronous-gauge.md):

$$
\boxed{\begin{aligned}
T^{00}&=a^{-2}\bar\rho(1+\delta),\\
T^{0i}&=a^{-2}\bar\rho(1+w)v^i,\\
T^{ij}&=a^{-2}w\bar\rho[(1+\delta)\delta^{ij}-h^{ij}].
\end{aligned}}
$$

In the first component the pressure contributions cancel; in the last, the velocity product is second order and the inverse-metric perturbation supplies the minus sign.

Use projections of [stress-energy conservation](../../../../../../stress-energy-conservation.md), $\nabla_\mu T^{\mu\nu}=0$, to retain all connection terms efficiently. Let $\mathcal H=a'/a$ be the [conformal Hubble parameter](../../../../../../conformal-hubble-parameter.md) and $h=\delta^{ij}h_{ij}$. Since $\sqrt{-g}=a^4(1+h/2)$, the fluid expansion is

$$
\vartheta=\nabla_\mu u^\mu=\frac1{\sqrt{-g}}\partial_\mu(\sqrt{-g}u^\mu)=a^{-1}\left(3\mathcal H+\partial_iv^i+\frac12h'\right).
$$

The energy projection is $u^\mu\partial_\mu\rho+(\rho+P)\vartheta=0$. Its background is $\bar\rho'+3\mathcal H(1+w)\bar\rho=0$. Expanding and subtracting that background leaves the [synchronous perfect-fluid density equation](../../../../../../synchronous-perfect-fluid-density-equation.md)

$$
\delta'+(1+w)\left(\partial_iv^i+\frac12h'\right)=0.
$$

For momentum, the spatial projection is $(\rho+P)u^\nu\nabla_\nu u_i+(\delta_i{}^\nu+u_i u^\nu)\partial_\nu P=0$. The given connections yield $u^\nu\nabla_\nu u_i=v_i'+\mathcal H v_i$ at first order. The pressure projection contains both $\partial_i\delta P$ and $v_i\bar P'$; retaining the latter is essential. With $\delta P=w\bar\rho\delta$ and $\bar P'=-3w\mathcal H(1+w)\bar\rho$, division by $\bar\rho(1+w)$ gives the [Cosmological Euler equation in synchronous gauge](../../../../../../cosmological-euler-equation-in-synchronous-gauge.md),

$$
v_i'+(1-3w)\mathcal H v_i+\frac{w}{1+w}\partial_i\delta=0.
$$

For Fourier convention $e^{i\mathbf k\cdot\mathbf x}$, these results are

$$
\boxed{\delta'+(1+w)i\mathbf k\cdot\mathbf v+\frac12(1+w)h'=0,\qquad\mathbf v'+(1-3w)\mathcal H\mathbf v+\frac{w}{1+w}i\mathbf k\delta=0.}
$$

The velocity equation assumes nonzero enthalpy $\bar\rho+\bar P$, so a cosmological constant with $w=-1$ is not a propagating fluid-velocity case. A time-dependent $w$ would also introduce additional terms and is not the constant-barotropic system used here.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
