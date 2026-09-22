<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Rosseland mean opacity](../../../../../rosseland-mean-opacity.md) is the transport opacity appropriate to an optically thick region close to [local thermodynamic equilibrium](../../../../../local-thermodynamic-equilibrium.md). If $\kappa_\nu$ is monochromatic transport opacity and $B_\nu(T)$ the [Planck function](../../../../../planck-function.md), then

$$
\boxed{\frac1{\kappa_R}=\frac{\int_0^\infty\kappa_\nu^{-1}(\partial B_\nu/\partial T)\,d\nu}{\int_0^\infty(\partial B_\nu/\partial T)\,d\nu}.}
$$

It is a weighted harmonic mean: low-opacity frequency windows carry much of the diffusive flux. One must combine the monochromatic processes before averaging, rather than adding their separately averaged opacities.

In hot fully ionized material, [electron-scattering opacity](../../../../../electron-scattering-opacity.md) supplies an almost density- and temperature-independent contribution at fixed composition. In the nonrelativistic [Thomson scattering](../../../../../thomson-scattering.md) limit, $\kappa_{\rm es}=\sigma_Tn_e/\rho\simeq0.2(1+X)\ {\rm cm^2\,g^{-1}}$. [Free-free opacity](../../../../../free-free-opacity.md), the absorption counterpart of [thermal bremsstrahlung](../../../../../thermal-bremsstrahlung.md), comes from photon absorption during encounters between free electrons and ions. Its approximate mean obeys [Kramers' opacity law](../../../../../kramers-opacity-law.md), $\kappa_{\rm ff}\propto\rho T^{-7/2}$, with composition and quantum correction factors.

When ions retain bound electrons, bound-free absorption is [photoionization](../../../../../photoionization.md); edges, occupations and ionization fractions strongly affect its frequency dependence. Bound-bound absorption produces [absorption lines](../../../../../absorption-line.md). Numerous metal lines can close low-opacity windows and produce important opacity features in partially ionized layers. Line populations depend on excitation as well as ionization, while [Doppler broadening](../../../../../doppler-broadening.md), [pressure broadening](../../../../../pressure-broadening.md) and overlapping lines change the transport windows. Stimulated inverse processes must be included consistently with detailed balance and the local thermal radiation field.

In cooler hydrogen-rich atmospheres, [negative hydrogen ion opacity](../../../../../negative-hydrogen-ion-opacity.md) from both bound-free and free-free processes is often important. Its strong temperature dependence helps determine convective surface relations. In still cooler layers, molecular bands, and at sufficiently low temperatures dust absorption/scattering, may be important. These processes cannot be represented by one Kramers power law over the whole density-temperature plane.

An opacity calculation therefore needs the chemical abundances, the [equation of state](../../../../../equation-of-state.md), electron density and bound-state populations. [Saha ionization equation](../../../../../saha-ionization-equation.md) and thermal excitation populations give useful dilute LTE estimates; high-density pressure ionization, nonideal effects and altered level populations require corrections. Composition matters even when one writes only $\kappa(\rho,T)$: hydrogen, helium and the metal abundance pattern are additional fixed inputs.

In dense degenerate cores, [thermal conduction](../../../../../thermal-conduction.md) by electrons can dominate energy transport. An equivalent conductive opacity may be introduced so that $1/\kappa_{\rm eff}=1/\kappa_R+1/\kappa_{\rm cond}$, because the two diffusive fluxes add; conduction is not itself a photon absorption process. Very hot regimes also require departures from the simple nonrelativistic scattering approximation. Near the optically thin photosphere, a Rosseland diffusion description alone is inadequate, and frequency-dependent [radiative transfer](../../../../../radiative-transfer.md) with appropriate boundary conditions is required. These regime changes are why realistic stellar opacity tables, rather than one global power law, enter [stellar structure](../../../../../stellar-structure-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
