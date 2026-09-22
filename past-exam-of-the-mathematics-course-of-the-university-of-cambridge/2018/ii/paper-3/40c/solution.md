<h1 id="40c/solution">Solution</h1>

↑ **Parent:** [40C](../40c.md)

Let a slowly varying wave have phase $S(\mathbf x,t)$, [wavevector](../../../../../wavevector.md) $\mathbf k=\nabla S$, and [angular frequency](../../../../../angular-frequency.md) $\omega=-\partial_tS$. The local [dispersion relation](../../../../../dispersion-relation.md) is the Hamilton-Jacobi equation $\omega=\Omega(\mathbf k;\mathbf x,t)$. Equality of mixed derivatives, followed along a curve with velocity $\dot{\mathbf x}=\nabla_{\mathbf k}\Omega$, gives the [Hamiltonian ray-tracing equations](../../../../../hamiltonian-ray-tracing-equations.md)

$$
\boxed{\frac{dx_i}{dt}=\frac{\partial\Omega}{\partial k_i},
\qquad
\frac{dk_i}{dt}=-\frac{\partial\Omega}{\partial x_i},
\qquad
\frac{d\omega}{dt}=\frac{\partial\Omega}{\partial t}.}
$$

Here $d/dt=\partial_t+\dot{\mathbf x}\mathbin{\cdot}\nabla$ is the total derivative evaluated along a ray, and $\dot{\mathbf x}$ is the [group velocity](../../../../../group-velocity.md).

For $\Omega=kc(z)$, $\omega$, $k_x$, and $k_y$ are conserved. If $\psi$ is the angle between the ray and the $z$-axis, then $k\sin\psi=(k_x^2+k_y^2)^{1/2}$ and $k=\omega/c$. Hence [Snell's law](../../../../../snell-s-law.md) is

$$
\boxed{\frac{\sin\psi}{c}=\frac{(k_x^2+k_y^2)^{1/2}}\omega=\text{constant}.}
$$

For the ray launched with $\mathbf k=k(\cos\phi,0,\sin\phi)$ at $z=0$, this constant is $|\cos\phi|/c_0$. Therefore

$$
\sin\psi=|\cos\phi|(1+\beta^2z^2)\leq1,
$$

which proves

$$
\boxed{|z|\leq z_m=\frac1\beta
\left(\frac1{|\cos\phi|}-1\right)^{1/2}.}
$$

For $0<\phi<\pi/2$, write $a=\cos\phi$. Since the ray and wavevector are parallel,

$$
\left(\frac{dz}{dx}\right)^2
=\left[\frac1{a(1+\beta^2z^2)}\right]^2-1.
$$

Near the upper [turning point](../../../../../turning-point.md), put $z=z_m-\zeta$. Expansion gives

$$
\left(\frac{dz}{dx}\right)^2\simeq4a\beta^2z_m\zeta.
$$

If $x=x_m$ at the turn, integration yields the local ray path

$$
\boxed{z\simeq z_m-a\beta^2z_m(x-x_m)^2.}
$$

The ray is tangent to the line $z=z_m$, turns smoothly, crosses $z=0$, and repeats symmetrically between $-z_m$ and $z_m$. Increasing $\phi$ decreases $z_m$, while $\phi\downarrow0$ sends the turning level outward.

## ↑ Ancestors (10)

1. [40C](../40c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
