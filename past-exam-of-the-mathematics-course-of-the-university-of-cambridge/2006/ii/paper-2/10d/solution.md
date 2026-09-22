<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

An adiabatic change of box size preserves the mode labels, whose momenta scale as $p\propto L^{-1}$. Since $V=L^3$, differentiation gives $dp/dV=-p/(3V)$. [Occupation numbers](../../../../../occupation-number.md) are fixed under this slow mechanical change, so summing the changes in the individual particle energies gives

$$
dE=\int_0^\infty E'(p)\,\overline n(p)\,dp\left(-\frac{p}{3V}dV\right).
$$

Comparison with $dE=-P\,dV$ at fixed [entropy](../../../../../entropy.md) and particle number yields

$$
\boxed{P=\frac1{3V}\int_0^\infty pE'(p)\overline n(p)\,dp.}
$$

The integration notation means summing over the original momentum-mode labels; it does not assume that the density in momentum space is unchanged after rescaling. In the ultrarelativistic limit $E(p)=cp$, so $pE'(p)=E(p)$ and **$P=E/(3V)=\rho c^2/3$**.

Adiabatic radiation obeys $d(Ea^3)=-P\,d(a^3)$, giving [energy density](../../../../../energy-density.md) proportional to $a^{-4}$. Equilibrium [photon energy density](../../../../../photon-energy-density.md) is proportional to $T^4$, so $T\propto a^{-1}$. Therefore the photon number in a [comoving volume](../../../../../comoving-volume.md), $n_\gamma a^3\propto T^3a^3$, is constant. Its [entropy](../../../../../entropy.md) is also constant: photon [entropy density](../../../../../entropy-density.md) is $(\epsilon_\gamma+P)/T\propto T^3$. Photon number is not a microscopic [conserved charge](../../../../../conserved-charge.md), but equilibrium processes maintaining the spectrum do not alter this comoving-number scaling in [adiabatic expansion](../../../../../adiabatic-expansion.md); entropy-producing processes would invalidate the assumptions.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
