<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Measure [optical depth](../../../../../../optical-depth.md) inward, so $d\tau/dr=-\kappa\rho$ and $\tau=0$ at the exterior boundary. The printed integral is shorthand with inconsistent integration labels; this differential definition fixes its meaning. In a [plane-parallel atmosphere](../../../../../../plane-parallel-atmosphere.md) in radiative equilibrium, $F=\sigma T_{\rm eff}^4$ is constant and $dP_{\rm rad}/d\tau=F/c$.

For the [Eddington surface boundary condition](../../../../../../eddington-surface-boundary-condition.md), approximate the outgoing frequency-integrated intensity by a constant $I_0$ over the outward hemisphere, with no incoming radiation. The angular moments at the surface are

$$
F=2\pi I_0\int_0^1\mu\,d\mu=\pi I_0,\qquad P_{\rm rad}(0)=\frac{2\pi I_0}{c}\int_0^1\mu^2\,d\mu=\boxed{\frac{2F}{3c}}.
$$

Integrating the moment equation then gives $P_{\rm rad}=F(\tau+2/3)/c$. The [Eddington closure approximation](../../../../../../eddington-closure-approximation.md), with [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md) and radiative equilibrium, identifies the radiation energy density with $a_{\rm rad}T^4$ and sets $P_{\rm rad}=a_{\rm rad}T^4/3$. Using $a_{\rm rad}c=4\sigma$ gives

$$
\boxed{T^4(\tau)=\frac34T_{\rm eff}^4\left(\tau+\frac23\right)=\frac12T_{\rm eff}^4\left(1+\frac32\tau\right).}
$$

The [photosphere](../../../../../../photosphere.md) is represented by $\tau=2/3$, where $T=T_{\rm eff}$; the exterior boundary instead has $T(0)=2^{-1/4}T_{\rm eff}$. The closure and angular boundary condition are approximations, rather than exact isotropy of radiation at the surface.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
