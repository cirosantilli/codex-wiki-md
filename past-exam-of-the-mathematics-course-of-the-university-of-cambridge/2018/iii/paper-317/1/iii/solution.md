<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Consider a spherical [stellar polytrope](../../../../../../stellar-polytrope.md) with $P=K\rho^{1+1/n}$, constant $K$, $0<n<5$, zero surface pressure and finite radius $R$. Its [specific enthalpy](../../../../../../specific-enthalpy.md), measured from zero density, is $h=\int_0^P dP'/\rho=(n+1)P/\rho$. [Hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) gives $h+\Phi=\Phi(R)=-GM/R$. Integrating over mass therefore yields

$$
(n+1)\int P\,dV=-\frac{GM^2}{R}-\int\Phi\,dm=-\frac{GM^2}{R}-2\Omega.
$$

The static [stellar virial theorem](../../../../../../stellar-virial-theorem.md) gives $3\int P\,dV=-\Omega$, and eliminating the pressure integral proves the [gravitational energy of a stellar polytrope](../../../../../../gravitational-energy-of-a-stellar-polytrope.md):

$$
\boxed{\Omega=-\frac{3}{5-n}\frac{GM^2}{R}.}
$$

For an [ideal gas](../../../../../../ideal-gas.md) with constant [specific-heat ratio](../../../../../../heat-capacity-ratio.md), the accompanying [internal energy](../../../../../../internal-energy.md) is

$$
U=\frac{1}{(5-n)(\gamma-1)}\frac{GM^2}{R}.
$$

To express both energies using $\gamma$ alone one additionally identifies the model as an [adiabatic stellar polytrope](../../../../../../adiabatic-stellar-polytrope.md), so $n=1/(\gamma-1)$. Then

$$
\boxed{\Omega=-\frac{3(\gamma-1)}{5\gamma-6}\frac{GM^2}{R},\qquad U=\frac{1}{5\gamma-6}\frac{GM^2}{R}.}
$$

For $\gamma=5/3$ these become $\Omega=-6GM^2/(7R)$ and $U=3GM^2/(7R)$. A general [polytropic index](../../../../../../polytropic-index.md) need not be determined by the thermodynamic [specific-heat ratio](../../../../../../heat-capacity-ratio.md); without the adiabatic identification both $n$ and $\gamma$ remain.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
