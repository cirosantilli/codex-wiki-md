<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

The [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) with no body force is $\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla p/\rho$. For [irrotational flow](../../../../../irrotational-flow.md) $\mathbf u=\nabla\phi$, the identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times(\nabla\times\mathbf u)$ removes the last term. Thus the [gradient](../../../../../gradient.md) of $\phi_t+|\nabla\phi|^2/2+p/\rho$ is zero, giving the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md)

$$
\boxed{\frac p\rho+\phi_t+\frac12|\nabla\phi|^2=F(t).}
$$

The function is spatially constant on the [connected](../../../../../connected-space.md) fluid region; adding a time-dependent constant to the potential changes its gauge.

For [spherically symmetric incompressible radial flow](../../../../../spherically-symmetric-incompressible-radial-flow.md), $r^2u_r$ is independent of $r$. The bubble boundary moves with the fluid, so $u_r(R)=\dot R$, giving $u_r=R^2\dot R/r^2$. Fix $\phi\to0$ at infinity, obtaining $\phi=-R^2\dot R/r$ and $F=p_\infty/\rho$. The time [derivative](../../../../../derivative.md) is taken at fixed $r$, then evaluated at the moving boundary: $\phi_t(R)=-(2\dot R^2+R\ddot R)$. With pressure continuity at the interface and no capillary or viscous correction, Bernoulli gives the [Rayleigh equation for an inviscid spherical bubble](../../../../../rayleigh-equation-for-an-inviscid-spherical-bubble.md)

$$
\boxed{R\ddot R+\frac32\dot R^2=\frac{p_g-p_\infty}\rho.}
$$

The gas law and initial pressure fix $CM^2=p_\infty R_0^6/2$. Multiply the radius equation by $2R^2\dot R$; its left side is $d(R^3\dot R^2)/dt$. Integrating from the zero-speed initial state gives the [first integral of polytropic spherical-bubble motion](../../../../../first-integral-of-polytropic-spherical-bubble-motion.md)

$$
\boxed{R^3\dot R^2=\frac{p_\infty}\rho\left[R_0^3-\frac{R_0^6}{3R^3}-\frac23R^3\right].}
$$

To find the permitted radii, put $s=R^3/R_0^3$. The bracket becomes $R_0^3(1-s)(2s-1)/(3s)$, nonnegative exactly for $1/2\leq s\leq1$. Therefore

$$
\boxed{\frac{R_0}{2^{1/3}}\leq R\leq R_0.}
$$

Initially $\ddot R=-p_\infty/(2\rho R_0)<0$, so the radius decreases from the upper endpoint. At the lower endpoint the gas pressure is $2p_\infty$, giving positive acceleration and an outward reversal. The first-integral zeros are simple, so the travel-time integrals near either endpoint behave as an integrable inverse square root. The bubble reaches both turning radii in finite time, and the autonomous undamped equation repeats this motion periodically. Thus the stated interval describes oscillation, rather than an irreversible approach to one endpoint.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
