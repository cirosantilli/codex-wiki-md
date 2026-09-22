<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

For one molecule whose translational motion separates from its internal degrees of freedom, the classical one-particle [partition function](../../../../../canonical-partition-function.md) is

$$
z_1(T,V)=\frac{V}{\lambda^3}q_{\rm int}(T),
\qquad
\lambda=\sqrt{\frac{2\pi\hbar^2}{mk_BT}},
$$

where $q_{\rm int}$ contains rotational, vibrational, and other internal states. For $N$ indistinguishable noninteracting molecules, the [classical ideal-gas partition function](../../../../../classical-ideal-gas-partition-function.md) is $Z_N=z_1^N/N!$. The thermodynamic pressure therefore obeys

$$
P=k_BT\left(\frac{\partial\log Z_N}{\partial V}\right)_{T,N}
=\frac{Nk_BT}{V},
$$

so

$$
\boxed{PV=Nk_BT.}
$$

The internal structure changes the energy, entropy, and heat capacity through $q_{\rm int}(T)$, but it does not change the [ideal gas](../../../../../ideal-gas.md) law while the internal partition function is independent of volume and the molecules have negligible interactions.

For a dilute monatomic gas $q_{\rm int}=1$. Using the [Stirling formula](../../../../../stirling-formula.md) in $Z_N=(V/\lambda^3)^N/N!$ and differentiating the [Helmholtz free energy](../../../../../helmholtz-free-energy.md) $F=-k_BT\log Z_N$ gives the [Sackur-Tetrode equation](../../../../../sackur-tetrode-equation.md)

$$
\boxed{S=Nk_B\left[
\log\left(\frac{V}{N}\left(\frac{2\pi mk_BT}{h^2}\right)^{3/2}\right)
+\frac52\right].}
$$

With $N$ fixed, an [isentropic process](../../../../../isentropic-process.md) therefore satisfies $VT^{3/2}=\text{constant}$, or $TV^{2/3}=\text{constant}$. Eliminating $T$ with the ideal-gas law yields the monatomic [reversible ideal-gas adiabat](../../../../../reversible-ideal-gas-adiabat.md)

$$
\boxed{PV^{5/3}=\text{constant}.}
$$

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
