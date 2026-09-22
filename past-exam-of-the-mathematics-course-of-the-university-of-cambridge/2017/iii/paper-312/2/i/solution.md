<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a local [orthonormal tetrad](../../../../../../orthonormal-frame-in-spacetime.md) and units in which the [speed of light](../../../../../../speed-of-light.md) is one. A particle has [four-momentum](../../../../../../four-momentum.md) $p^{\hat a}=E(1,\mathbf e)$ and moves with [velocity](../../../../../../velocity.md) $\mathbf e$. Thus its [energy density](../../../../../../energy-density.md) contributes $E$, its [momentum density](../../../../../../momentum-density.md) contributes $Ee^i$, and its [momentum flux](../../../../../../momentum-flux.md) contributes $Ee^ie^j$. Integrating the [phase-space distribution function](../../../../../../phase-space-distribution-function.md) gives the [kinetic stress-energy tensor](../../../../../../kinetic-stress-energy-tensor.md). The measure $d^3p/E$ is the future mass-shell [Lorentz-invariant phase-space measure](../../../../../../lorentz-invariant-phase-space-measure.md), so the same expression transforms as a spacetime [stress-energy tensor](../../../../../../stress-energy-tensor.md); fixed state-counting or polarization factors are understood to be included in $f$.

Define $\langle F\rangle_\Omega=(4\pi)^{-1}\int F\,d\Omega$. The [photon](../../../../../../photon.md) momentum measure is $d^3p=E^2dE\,d\Omega$, so every component of the [kinetic stress-energy tensor](../../../../../../kinetic-stress-energy-tensor.md) has a radial factor $E^3dE=a^{-4}\epsilon^3d\epsilon$. An isotropic background has $\langle e^i\rangle_\Omega=0$ and $\langle e^ie^j\rangle_\Omega=\delta^{ij}/3$. Hence

$$
\boxed{\bar\rho=\frac{4\pi}{a^4}\int_0^\infty\epsilon^3\bar f(\epsilon)\,d\epsilon,\qquad \bar P=\frac{\bar\rho}{3}.}
$$

This [radiation pressure](../../../../../../radiation-pressure.md) equation of state requires isotropy and masslessness, not a thermal spectrum.

The distribution perturbation is $\delta f=-\epsilon\bar f'(\epsilon)\Theta$. Assume finite [energy density](../../../../../../energy-density.md) and endpoint behavior $\epsilon^4\bar f(\epsilon)\to0$ at zero and infinity, as for the [Planck photon distribution](../../../../../../planck-photon-distribution.md). [Integration by parts](../../../../../../integration-by-parts.md) then gives

$$
-\int_0^\infty\epsilon^4\bar f'(\epsilon)\,d\epsilon=4\int_0^\infty\epsilon^3\bar f(\epsilon)\,d\epsilon.
$$

Consequently the perturbed [energy density](../../../../../../energy-density.md) and [momentum density](../../../../../../momentum-density.md) are

$$
\delta\rho=4\bar\rho\langle\Theta\rangle_\Omega,\qquad q^i=4\bar\rho\langle\Theta e^i\rangle_\Omega.
$$

Since $q^i=(\bar\rho+\bar P)v^i=(4\bar\rho/3)v^i$, the [photon angular temperature moments](../../../../../../photon-angular-temperature-moments.md) give $\delta=4\langle\Theta\rangle_\Omega$ and $v^i=3\langle\Theta e^i\rangle_\Omega$.

The sign of [anisotropic stress](../../../../../../anisotropic-stress.md) must be specified. Direct kinetic integration gives the conventional trace-free spatial stress $\pi^{ij}=T^{ij}-P\delta^{ij}=+4\bar\rho\langle\Theta(e^ie^j-\delta^{ij}/3)\rangle_\Omega$. The PDF uses the opposite sign, $\Pi^{ij}=-\pi^{ij}$, equivalently $T^{ij}=P\delta^{ij}-\Pi^{ij}$. With that convention, all requested moments are

$$
\boxed{\delta=4\langle\Theta\rangle_\Omega,\qquad v^i=3\langle\Theta e^i\rangle_\Omega,\qquad \Pi^{ij}=-4\bar\rho\left\langle\Theta\left(e^ie^j-\frac{\delta^{ij}}3\right)\right\rangle_\Omega.}
$$

Taking the spatial [trace](../../../../../../matrix-trace.md) also gives

$$
\boxed{\delta P=\frac{\bar\rho\delta}{3}.}
$$

The angular temperature description assumes $\Theta$ is independent of [photon](../../../../../../photon.md) energy; independent spectral distortions would require additional energy-dependent moments.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
