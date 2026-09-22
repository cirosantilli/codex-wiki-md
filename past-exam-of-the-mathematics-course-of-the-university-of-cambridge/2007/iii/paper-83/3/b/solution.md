<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An eddy at height $z$ cannot extend arbitrarily far through the ground, so its largest local vertical scale is proportional to $z$. Choose $\ell\sim z$ and absorb its constant of proportionality into the coefficient. With the prescribed constant turbulent [velocity](../../../../../../velocity.md) scale, write

$$
\nu_T=Cz,\qquad C=\alpha\hat u>0.
$$

The [mixing-length closure](../../../../../../mixing-length-closure.md) is $-\overline{u'w'}=\nu_TU_z$. Thus the full kinematic stress is

$$
T\equiv\frac{\tau_d}{\rho}=(\nu+\nu_T)U_z.
$$

For $z\gg\delta$, neglect the molecular term. With no internal momentum source, $T$ is constant, so

$$
U_z=\frac{T}{Cz}.
$$

Integrating between two heights gives

$$
\boxed{U(z)=U(z_r)+\frac{T}{\alpha\hat u}\log\frac{z}{z_r}.}
$$

Equivalently define an extrapolated [roughness length](../../../../../../roughness-length.md) $z_0$ and write $U=(T/C)\log(z/z_0)$. If $C=\kappa u_*$, the familiar [law of the wall](../../../../../../law-of-the-wall.md) is $U/u_*=(1/\kappa)\log(z/z_0)$. The logarithmic profile is valid outside the inner viscous region and below scales where the constant-stress or wall-distance assumptions fail. It cannot be continued to $z=0$ to impose the smooth-wall no-slip condition.

The part b notation $\tau=\nu_TU_z$ must therefore mean $\tau=T$, a stress divided by [density](../../../../../../density.md). Using the physical stress from part a on that right-hand side would omit a factor of $\rho$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
