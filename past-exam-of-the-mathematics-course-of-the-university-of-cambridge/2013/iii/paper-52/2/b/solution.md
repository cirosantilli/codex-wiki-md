<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrating each [conservation law](../../../../../../conservation-law.md) across a vanishingly thin interval around the stationary [shock wave](../../../../../../shock-wave.md) leaves equal [conservation law fluxes](../../../../../../conservation-law-flux.md) on its two sides. Hence

$$
\boxed{\rho_2u_2=\rho_1u_1,\quad
p_2+\rho_2u_2^2=p_1+\rho_1u_1^2,\quad
u_2\left(\frac{\rho_2u_2^2}{2}+\frac{\gamma p_2}{\gamma-1}\right)=u_1\left(\frac{\rho_1u_1^2}{2}+\frac{\gamma p_1}{\gamma-1}\right).}
$$

These are the [Rankine-Hugoniot conditions for a perfect gas](../../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md). Signed velocities may both be negative when the material travels from positive to negative $z$; no sign change is needed in the [conservation law fluxes](../../../../../../conservation-law-flux.md).

Put $r=\rho_2/\rho_1=u_1/u_2$, $P=p_2/p_1$ and $m=M_1^2=\rho_1u_1^2/(\gamma p_1)$. Momentum conservation gives

$$
P=1+\gamma m\left(1-\frac1r\right).
$$

Divide the energy condition by the nonzero mass flux. Equality of kinetic energy plus [specific enthalpy](../../../../../../specific-enthalpy.md) gives

$$
\frac{\gamma m}{2}+\frac{\gamma}{\gamma-1}
=\frac{\gamma m}{2r^2}+\frac{\gamma P}{(\gamma-1)r}.
$$

Substituting $P$ and multiplying by $2(\gamma-1)r^2/\gamma$ yields

$$
(r-1)\left[\bigl((\gamma-1)m+2\bigr)r-(\gamma+1)m\right]=0.
$$

The factor $r-1$ is the continuous, no-shock solution. On the nontrivial [normal shock wave](../../../../../../normal-shock-wave.md) branch,

$$
\boxed{\frac{\rho_2}{\rho_1}=\frac{u_1}{u_2}=\frac{(\gamma+1)M_1^2}{(\gamma-1)M_1^2+2},\qquad
\frac{p_2}{p_1}=\frac{2\gamma M_1^2-(\gamma-1)}{\gamma+1}.}
$$

An admissible compressive gas [shock wave](../../../../../../shock-wave.md) has $M_1>1$, so $r>1$ and $P>1$. The algebraic jump equations alone also allow a reversed expansive discontinuity; the [entropy production in a perfect-gas shock](../../../../../../entropy-production-in-a-perfect-gas-shock.md) excludes that branch. At $M_1=1$ the nontrivial branch joins the continuous solution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
