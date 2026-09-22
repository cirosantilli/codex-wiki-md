<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [stellar polytrope](../../../../../../stellar-polytrope.md) replaces a detailed [equation of state](../../../../../../equation-of-state.md) and thermal structure by $P=K\rho^{1+1/n}$ for $n>0$, with spatially constant $K$ and [polytropic index](../../../../../../polytropic-index.md) $n$. Together with spherical [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) and mass conservation, it gives a tractable family of stellar density profiles. Introduce the [Lane-Emden variables for a stellar polytrope](../../../../../../lane-emden-variables-for-a-stellar-polytrope.md)

$$
\rho=\rho_c\theta^n,\qquad r=b\xi,\qquad b^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1}.
$$

Combining $dP/dr=-Gm\rho/r^2$ with $dm/dr=4\pi r^2\rho$ eliminates $m$ to give $r^{-2}d[r^2\rho^{-1}(dP/dr)]/dr=-4\pi G\rho$. Substitution of the pressure law and the dimensionless variables gives the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\frac1{\xi^2}\frac{d}{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n,\qquad\theta(0)=1,\quad\theta'(0)=0.
$$

A regular finite-radius model for $0\leq n<5$ ends at the first zero $\xi_1$. Its radius and mass are

$$
R=b\xi_1,\qquad M=4\pi b^3\rho_c[-\xi_1^2\theta'(\xi_1)].
$$

These formulas supply central-to-mean density ratios and [stellar homology](../../../../../../stellar-homology.md) scalings without solving a full evolutionary model. Eliminating $\rho_c$, for $0<n<5$ and $n\ne3$, gives the [polytropic mass-radius relation](../../../../../../polytropic-mass-radius-relation.md)

$$
R\propto K^{n/(3-n)}G^{-n/(3-n)}M^{(1-n)/(3-n)}.
$$

An efficient-convection [monatomic gas](../../../../../../monatomic-gas.md) has $n=3/2$. The same index describes a cold, nonrelativistic [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md) law; at fixed composition it gives $R\propto M^{-1/3}$ for a [white dwarf](../../../../../../white-dwarf.md). Ultrarelativistic [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md) has $n=3$, for which the mass is independent of $\rho_c$ and scales as $(K/G)^{3/2}$. This is the origin of the [Chandrasekhar limit](../../../../../../chandrasekhar-limit.md). A radiation-dominated, approximately constant-entropy interior also approaches $P\propto\rho^{4/3}$ and $n=3$. The [polytrope of index zero](../../../../../../polytrope-of-index-zero.md) is an incompressible comparison model, useful for illustrating the role of central concentration.

The [gravitational energy of a stellar polytrope](../../../../../../gravitational-energy-of-a-stellar-polytrope.md), $\Omega=-3GM^2/[(5-n)R]$, and the [stellar virial theorem](../../../../../../stellar-virial-theorem.md) make polytropes useful for contraction-energy estimates. They also provide structural models for perturbation and stability calculations. **A polytrope is a structural approximation, not a complete stellar evolution calculation.** One must still specify [stellar nuclear fusion](../../../../../../stellar-nuclear-fusion.md), [opacity](../../../../../../opacity.md), energy transport, composition and boundary conditions to determine the [luminosity](../../../../../../luminosity.md) and history. Moreover, the structural exponent $1+1/n$ need not equal the [adiabatic exponent](../../../../../../heat-capacity-ratio.md) relevant to a rapid perturbation. Real stars can have different effective indices in their cores and envelopes, as well as [ionization](../../../../../../ionization.md) zones or varying [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
