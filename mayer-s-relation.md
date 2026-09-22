<h1 id="mayer-s-relation">Mayer's relation</h1>

↑ **Parent:** [Ideal gas](ideal-gas-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mayer's_relation)

Mayer's relation states that the difference between [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) and [heat capacity at constant volume](heat-capacity-at-constant-volume.md) for a fixed-composition [ideal gas](ideal-gas-split.md) is

$$
C_p(T)-C_V(T)=nR=Nk_B.
$$

Here both capacities are total [heat capacities](heat-capacity.md) in $\mathrm{J\,K^{-1}}$, $n$ is [amount of substance](amount-of-substance.md), $N$ is the number of particles, $R$ is the [molar gas constant](molar-gas-constant.md) and $k_B$ is the [Boltzmann constant](boltzmann-constant.md). In other normalizations the same statement is

$$
C_{p,\mathrm m}(T)-C_{V,\mathrm m}(T)=R,\qquad
c_p(T)-c_V(T)=\frac{nR}{m}.
$$

The first is a difference of [molar heat capacities](molar-heat-capacity.md), in $\mathrm{J\,mol^{-1}\,K^{-1}}$; the second uses [specific heat capacities](specific-heat-capacity.md), in $\mathrm{J\,kg^{-1}\,K^{-1}}$. Writing $C_p-C_V=R$ with total capacities would omit the sample's [amount of substance](amount-of-substance.md). The relation holds pointwise even when the capacities depend on [temperature](temperature-split.md). [Samuel J. Ling, William Moebs and Jeff Sanny, University Physics Volume 2, §3.5: ideal-gas capacity difference](https://openstax.org/books/university-physics-volume-2/pages/3-5-heat-capacities-of-an-ideal-gas)

The proof outline is short: [enthalpy](enthalpy-split.md) is $H=U+pV=U+nRT$, and [internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md) is independent of [volume](volume-thermodynamics.md) at fixed [temperature](temperature-split.md). Differentiating at fixed composition and [amount of substance](amount-of-substance.md) therefore gives $C_p=dH/dT=dU/dT+nR=C_V+nR$. It uses the [ideal gas law](ideal-gas-law.md), rather than assuming any particular number of molecular [degrees of freedom](degree-of-freedom.md). At fixed [pressure](pressure-split.md), the additional [heat](heat-split.md) supplies expansion [work](work.md), $p\,dV=nR\,dT$. The two processes can have the same [temperature](temperature-split.md) endpoints and equal $\Delta U$ while requiring different [heat](heat-split.md) inputs.

For one [mole](mole-unit.md) of the rigid-rotation diatomic [ideal gas](ideal-gas-split.md) model, $C_V=5R/2$ and $C_p=7R/2$. Heating by $10\,\mathrm K$ with $R\simeq8.31446\,\mathrm{J\,mol^{-1}\,K^{-1}}$ gives $Q_V\simeq207.86\,\mathrm J$ in a rigid sealed vessel and $Q_p\simeq291.01\,\mathrm J$ under a frictionless piston at fixed [pressure](pressure-split.md). Both gain $207.86\,\mathrm J$ of [internal energy](internal-energy-split.md), while the piston delivers approximately $83.14\,\mathrm J$ of [work](work.md). This is a calculated model budget. If the capacities vary with [temperature](temperature-split.md), the corresponding finite statement is still

$$
Q_p-Q_V=nR(T_2-T_1),\qquad
Q_V=n\int_{T_1}^{T_2}C_{V,\mathrm m}(T)\,dT,
$$

under the fixed-[pressure](pressure-split.md) and fixed-[volume](volume-thermodynamics.md) heating assumptions in [heat capacity](heat-capacity.md). Their final [volume](volume-thermodynamics.md) values generally differ. Combining [Mayer's relation](mayer-s-relation.md) with [heat capacity ratio](heat-capacity-ratio.md) also gives $C_V=nR/(\gamma-1)$ and $C_p=\gamma nR/(\gamma-1)$ locally; constant values cannot be extrapolated across intervals in which $\gamma(T)$ changes.

For a smooth stable single [thermodynamic phase](thermodynamic-phase.md) of a general [simple compressible system](simple-compressible-system.md), the broader [Maxwell relation](maxwell-relations.md) identity is

$$
C_p-C_V=T\left(\frac{\partial p}{\partial T}\right)_V\left(\frac{\partial V}{\partial T}\right)_p
=\frac{TV\alpha^2}{\kappa_T},
$$

where $\alpha$ is the [coefficient of thermal expansion](coefficient-of-thermal-expansion.md) and $\kappa_T$ the [isothermal compressibility](isothermal-compressibility.md), with composition fixed throughout. Substituting the [ideal gas law](ideal-gas-law.md) gives $nR$; a [real gas](real-gas.md) need not do so. This distinction matters near a [phase transition](phase-transition.md) or when interactions appreciably change the [equation of state](equation-of-state.md). It explains why [Mayer's relation](mayer-s-relation.md) is useful: thermal measurements under different constraints become linked to a mechanical response, while the difference retains a particularly simple value for an [ideal gas](ideal-gas-split.md).[§4.4.2: Maxwell relations and the general heat-capacity difference](statistical-physics-by-david-tong/4-classical-thermodynamics.md)

## ↑ Ancestors (6)

1. [Ideal gas](ideal-gas-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Adiabatic compression](adiabatic-compression.md)
- [Heat capacity ratio](heat-capacity-ratio.md)
- [Internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md)
- [Maxwell relations](maxwell-relations.md)
- [Mayer's relation](mayer-s-relation.md)
