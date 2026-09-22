<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A stationary microporous network removes fluid momentum through [linear drag](../../../../../../linear-drag.md) rather than through a domain-scale viscous stress. With $[\bar\eta]=\mathrm{M\,L^{-3}\,T^{-1}}$, the single-scale force estimate becomes

$$
\rho\left(\alpha\ddot L+\beta\frac{\dot L^2}{L}\right)=-c_d\bar\eta\dot L+c_s\frac\sigma{L^2},\qquad c_d,c_s>0.
$$

This [drag-limited hydrodynamic coarsening](../../../../../../drag-limited-hydrodynamic-coarsening.md) closure uses a fixed isotropic drag coefficient and domain sizes large compared with the pore scale. The only length and time made from $\rho,\sigma,\bar\eta$ are

$$
\boxed{L_1=\left(\frac{\sigma\rho}{\bar\eta^2}\right)^{1/3},\qquad t_1=\frac\rho{\bar\eta}.}
$$

Indeed $L_1^3=\sigma t_1^2/\rho$, while the choice of $t_1$ equates inertial and drag prefactors. With $L=L_1g(u)$ and $u=t/t_1$, all force terms share $\rho L_1/t_1^2=\bar\eta L_1/t_1=\sigma/L_1^2$. Therefore

$$
\boxed{\frac{L(t)}{L_1}=g(t/t_1),\qquad \alpha g''+\beta\frac{g'^2}{g}=-c_dg'+\frac{c_s}{g^2}.}
$$

As before, a parameter-free function of this one argument refers to the asymptotic advective scaling model with fixed morphology and negligible extra scales. Retaining the diffusive mobility or resolved network geometry can introduce additional dimensionless parameters. The original $\eta$ does not remain as an independent viscous coefficient after the stipulated replacement.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
