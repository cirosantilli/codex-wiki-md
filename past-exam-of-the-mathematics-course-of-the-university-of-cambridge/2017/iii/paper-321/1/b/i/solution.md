<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the vertical equations, $\mu$ denotes [dynamic viscosity](../../../../../../../dynamic-viscosity.md), while $\mu_m$ is the [mean molecular weight](../../../../../../../mean-molecular-weight.md) in units of the proton mass $m_p$. The symbol $k$ denotes the [Boltzmann constant](../../../../../../../boltzmann-constant.md). For the intended [hydrostatic equilibrium](../../../../../../../hydrostatic-equilibrium.md) calculation, put $P=K\rho^\gamma$ with $K>0$, $\gamma>1$, and set $\mathcal R=k/(\mu_m m_p)$. Dividing the hydrostatic equation by $\rho$ and integrating from the symmetric midplane gives

$$
\frac{\gamma K}{\gamma-1}\rho^{\gamma-1}=\frac{\gamma K}{\gamma-1}\rho_m^{\gamma-1}-\frac{\Omega^2z^2}{2}.
$$

The [specific enthalpy](../../../../../../../specific-enthalpy.md) vanishes at the free surface. Hence the [polytropic vertical structure in stellar gravity](../../../../../../../polytropic-vertical-structure-in-stellar-gravity.md) is

$$
\boxed{\rho(z)=\rho_m\left(1-\frac{z^2}{H^2}\right)^{1/(\gamma-1)},\qquad H^2=\frac{2\gamma K\rho_m^{\gamma-1}}{(\gamma-1)\Omega^2}=\frac{2\gamma\mathcal R T_m}{(\gamma-1)\Omega^2}.}
$$

On $|z|<H$, the [ideal gas](../../../../../../../ideal-gas.md) relation gives $T=T_m(1-z^2/H^2)$ and $P=P_m(1-z^2/H^2)^{\gamma/(\gamma-1)}$; the vacuum extension sets $\rho=P=0$ outside. The formula needs $\gamma>1$ for a finite positive semi-thickness and assumes the harmonic vertical gravity remains valid through this height.

There is a genuine inconsistency if all four printed structure equations are imposed literally with $F=0$ and finite positive [opacity](../../../../../../../opacity.md): [radiative diffusion](../../../../../../../radiative-diffusion.md) then requires $dT/dz=0$, whereas the polytropic [temperature](../../../../../../../temperature.md) above has a nonzero [gradient](../../../../../../../gradient.md) away from the midplane. The intended result is valid for the hydrostatic [polytropic equation of state](../../../../../../../polytropic-equation-of-state.md) with the radiative closure replaced or neglected, for example an adiabatic opaque limit. It is not an exact simultaneous solution of the stated finite-opacity radiative system. With that radiative system and a nonvacuum [ideal gas](../../../../../../../ideal-gas.md), $\gamma=1$ instead gives an isothermal solution

$$
\rho=\rho_m\exp\left[-\frac{\Omega^2z^2}{2\mathcal R T_m}\right],
$$

which has no finite free surface. For $\gamma\ne1$, constant $T$ and constant $K$ would force constant density, contradicting hydrostatic balance on a nontrivial vertical interval. This is the [zero-radiative-flux obstruction for a polytropic ideal gas](../../../../../../../zero-radiative-flux-obstruction-for-a-polytropic-ideal-gas.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
