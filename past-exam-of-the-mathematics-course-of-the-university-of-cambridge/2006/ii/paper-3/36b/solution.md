<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

The [rate-of-strain tensor](../../../../../strain-rate-tensor.md) is $e_{ij}=\frac12(\partial_ju_i+\partial_iu_j)$. For an incompressible [Newtonian fluid](../../../../../newtonian-fluid.md), the [stress tensor](../../../../../cauchy-stress-tensor.md) is $\sigma_{ij}=-p\delta_{ij}+2\mu e_{ij}$. Dotting the momentum equation with velocity and using the product rule gives the local mechanical-energy balance

$$
\partial_t(\tfrac12\rho|u|^2)+\partial_j(\tfrac12\rho|u|^2u_j)=\partial_j(u_i\sigma_{ij})-\sigma_{ij}\partial_ju_i
$$

without body forces. Write $\partial_ju_i=e_{ij}+\omega_{ij}$, with $\omega_{ij}$ antisymmetric. The pressure contribution is $-p\partial_iu_i=0$, and $e_{ij}\omega_{ij}=0$ by symmetry. Thus the remaining loss is $2\mu e_{ij}e_{ij}\ge0$, proving **the local viscous dissipation rate is $2\mu e_{ij}e_{ij}$ per unit volume**.

For the oscillating boundary, take $u=(U(y,t),0,0)$ and constant pressure. The nonlinear advection vanishes, leaving $U_t=\nu U_{yy}$, $\nu=\mu/\rho$. Seek the real part of $V e^{i\omega t-\gamma y}$; decay at infinity selects $\gamma=(1+i)/\delta$, $\delta=\sqrt{2\nu/\omega}$. After transients,

$$
\boxed{U(y,t)=V e^{-y/\delta}\cos(\omega t-y/\delta).}
$$

Only $e_{xy}=e_{yx}=U_y/2$ is nonzero, so the dissipation is $\mu U_y^2$. Its time average is $\mu V^2\delta^{-2}e^{-2y/\delta}$: the two sine and cosine contributions each average to one half. Integrating over $y>0$ gives

$$
\boxed{\left\langle\frac{\text{dissipation}}{\text{boundary area}}\right\rangle=\frac{\mu V^2}{2\delta}=V^2\sqrt{\frac{\mu\rho\omega}{8}}.}
$$

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
