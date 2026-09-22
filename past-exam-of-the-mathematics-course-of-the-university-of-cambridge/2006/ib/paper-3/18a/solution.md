<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

For an [inviscid flow](../../../../../inviscid-flow.md) of constant density $\rho$, driven by a conservative body force $-\nabla\Phi$, the [Euler equation](../../../../../euler-equations-for-an-inviscid-fluid.md) is

$$
\partial_tu+(u\cdot\nabla)u=-\nabla(p/\rho)-\nabla\Phi.
$$

The vector identity $(u\cdot\nabla)u=\nabla(|u|^2/2)-u\times(\nabla\times u)$ and irrotationality give the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md). Specifically, wherever a single-valued potential $u=\nabla\phi$ is available,

$$
\nabla\left(\phi_t+\frac12|u|^2+\frac p\rho+\Phi\right)=0.
$$

On a connected potential-flow region this means

$$
\boxed{\phi_t+\frac12|u|^2+\frac p\rho+\Phi=C(t).}
$$

The integration function is spatially constant but need not be constant in time; it can be removed by changing the potential's time-dependent gauge. A simply connected irrotational region provides the requisite global potential. For a barotropic fluid the [pressure](../../../../../pressure.md) term is replaced by $\int dp/\rho(p)$; here the liquid density is constant.

For the tube, let $U(t)$ be its approximately uniform axial [velocity](../../../../../velocity.md). The large reservoir's surface [velocity](../../../../../velocity.md) is negligible and gravity is neglected as stipulated. Entrance-region inertia contributes an effective length of order $a$, negligible against $L$. The potential difference between the outlet and the reservoir is consequently $LU$ to leading order. Subtract Bernoulli at the reservoir surface, where [pressure](../../../../../pressure.md) is $P+p_a$, from its value at the outlet, where [pressure](../../../../../pressure.md) is $p_a$ and speed is $U$. This gives

$$
L\dot U+\frac12U^2=\frac P\rho,\qquad U(0)=0.
$$

The inertial term cannot be dropped during startup. With $U_\infty=\sqrt{2P/\rho}$, separate variables:

$$
\frac{d(U/U_\infty)}{1-(U/U_\infty)^2}=\frac{U_\infty}{2L}\,dt.
$$

Hence the [inviscid startup in a pressure-driven tube](../../../../../inviscid-startup-in-a-pressure-driven-tube.md) gives

$$
\boxed{Q(t)=\pi a^2\sqrt{\frac{2P}{\rho}}
\tanh\left(\frac tL\sqrt{\frac P{2\rho}}\right).}
$$

Initially $U\sim Pt/(\rho L)$, the acceleration of the stationary liquid column. At long times $U\to\sqrt{2P/\rho}$, the inviscid pressure-to-kinetic-energy limit. The result applies while the tube remains full and reservoir dimensions are large enough that surface motion and the neglected entrance inertia remain small.

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
