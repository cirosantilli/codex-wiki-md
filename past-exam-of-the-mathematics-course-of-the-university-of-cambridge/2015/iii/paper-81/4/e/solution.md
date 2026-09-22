<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator.md), set $\mu=0$ and $\Omega=\hbar\omega$. The normal symbol is $H_N(\bar\psi,\psi)=\Omega(\bar\psi\psi+1/2)$, so the thermal [coherent-state time slicing](../../../../../../coherent-state-time-slicing.md) gives

$$
Z=\int_{\mathrm{periodic}}\mathcal D(\bar\psi,\psi)\exp\left[-\int_0^\beta\big(\bar\psi\partial_\tau\psi+\Omega\bar\psi\psi+\Omega/2\big)d\tau\right].
$$

The connection with a [phase-space path integral](../../../../../../phase-space-path-integral.md) uses the canonical real coordinates

$$
\psi=\frac{\sqrt{m\omega}\,q+ip/\sqrt{m\omega}}{\sqrt{2\hbar}},\qquad \bar\psi=\frac{\sqrt{m\omega}\,q-ip/\sqrt{m\omega}}{\sqrt{2\hbar}}.
$$

Their derivative term satisfies $\bar\psi\dot\psi=-ip\dot q/\hbar$ up to total derivatives that vanish for periodic paths. The [normal and Weyl symbols of a harmonic oscillator](../../../../../../normal-and-weyl-symbols-of-a-harmonic-oscillator.md) must be distinguished: in midpoint phase-space time slicing, the [Weyl ordering](../../../../../../weyl-ordering.md) symbol of $a^\dagger a$ is $\bar\psi\psi-1/2$. Thus the appropriate midpoint Hamiltonian is $H_W=p^2/(2m)+m\omega^2q^2/2$, with no additional constant. The change from the adjacent-label normal prescription to the midpoint prescription includes this ordering correction.

In physical imaginary time $u=\hbar\tau$, the resulting [phase-space path integral](../../../../../../phase-space-path-integral.md) is

$$
Z=\int_{\mathrm{periodic}}\mathcal Dq\,\mathcal Dp\,\exp\left[-\frac1\hbar\int_0^{\hbar\beta}\left(-ip\frac{dq}{du}+\frac{p^2}{2m}+\frac{m\omega^2q^2}{2}\right)du\right].
$$

[Gaussian momentum integration in a phase-space path integral](../../../../../../gaussian-momentum-integration-in-a-phase-space-path-integral.md) produces the usual oscillator [configuration-space path integral](../../../../../../configuration-space-path-integral.md). An exact check follows directly from the coherent kernel $\langle\psi'|e^{-\beta\Omega a^\dagger a}|\psi\rangle=\exp(e^{-\beta\Omega}\bar\psi'\psi)$:

$$
\boxed{Z=e^{-\beta\Omega/2}\int_{\mathbb C}\frac{d^2\psi}{\pi}e^{-(1-e^{-\beta\Omega})|\psi|^2}=\frac{e^{-\beta\hbar\omega/2}}{1-e^{-\beta\hbar\omega}}=\frac1{2\sinh(\beta\hbar\omega/2)}}.
$$

This is the [thermal partition function of a quantum harmonic oscillator](../../../../../../thermal-partition-function-of-a-quantum-harmonic-oscillator.md). Keeping the $\Omega/2$ normal-ordering constant a second time after switching to the Weyl symbol would double count the zero-point energy.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
