<h1 id="6g/solution">Solution</h1>

↑ **Parent:** [6G](../6g.md)

Take the divergence of the [Ampere-Maxwell law](../../../../../ampere-s-circuital-law.md) and use [Gauss's law](../../../../../gauss-s-law.md) $\nabla\cdot\boldsymbol E=\rho/\epsilon_0$. Since the divergence of a curl is zero, this gives the [charge continuity equation](../../../../../charge-continuity-equation.md) $\partial_t\rho+\nabla\cdot\boldsymbol j=0$. Uniform conductivity and [Ohm's law](../../../../../ohm-s-law.md) imply $\nabla\cdot\boldsymbol j=\sigma\nabla\cdot\boldsymbol E=\sigma\rho/\epsilon_0$. Therefore

$$
\boxed{\partial_t\rho=-\frac\sigma{\epsilon_0}\rho,\qquad\rho(t)=\rho_0e^{-t/\tau},\quad\tau=\frac{\epsilon_0}{\sigma}.}
$$

The spatially uniform initial density stays uniform in the interior; $\tau$ is the [charge relaxation](../../../../../charge-relaxation.md) time.

Denote the cylinder radius by $R$. Cylindrical symmetry makes the interior [electric field](../../../../../electric-field.md) radial. [Gauss's law](../../../../../gauss-s-law.md) on a coaxial cylinder of radius $r<R$ and length $\ell$ gives $2\pi r\ell E_r=\rho(t)\pi r^2\ell/\epsilon_0$. Thus

$$
\boxed{\boldsymbol E(r,t)=\frac{\rho_0r}{2\epsilon_0}e^{-t/\tau}\boldsymbol e_r,\qquad\boldsymbol j(r,t)=\frac{\sigma\rho_0r}{2\epsilon_0}e^{-t/\tau}\boldsymbol e_r\quad(r<R).}
$$

The current does not disappear at the interface: the vacuum conducts no current, so charge accumulates on the cylindrical surface. Initially taking the charge to be the stated [volume](../../../../../volume.md) charge alone, its [surface charge density](../../../../../surface-charge-density.md) satisfies $\dot\rho_s=j_r(R^-,t)$, giving the [charge relaxation in an isolated conducting cylinder](../../../../../charge-relaxation-in-an-isolated-conducting-cylinder.md) law

$$
\rho_s(t)=\frac{R\rho_0}{2}(1-e^{-t/\tau}).
$$

The total enclosed charge per unit length is $\pi R^2\rho(t)+2\pi R\rho_s(t)=\pi R^2\rho_0$. Consequently the exterior [electric field](../../../../../electric-field.md) is

$$
\boxed{\boldsymbol E(r,t)=\frac{\rho_0R^2}{2\epsilon_0r}\boldsymbol e_r\quad(r>R),}
$$

independent of time. The boundary jump obeys $E_r(R^+)-E_r(R^-)=\rho_s/\epsilon_0$, as it must. Applying [Gauss's law](../../../../../gauss-s-law.md) to the decaying [volume](../../../../../volume.md) charge alone would incorrectly predict a decaying exterior [electric field](../../../../../electric-field.md) and violate [electric charge conservation](../../../../../charge-conservation.md). The vector formulas also specify the inward direction if $\rho_0<0$.

## ↑ Ancestors (10)

1. [6G](../6g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
