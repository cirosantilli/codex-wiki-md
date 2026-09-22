<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use translating coordinates $Z=z-vt$ and a profile $\psi(\mathbf x,t)=\Phi(x,y,Z)$; the background condensate remains at rest in the laboratory. Then $\psi_t=-v\Phi_Z$, and the [Gross–Pitaevskii solitary wave](../../../../../../gross-pitaevskii-solitary-wave.md) equation is

$$
\boxed{2iv\Phi_Z=\nabla^2\Phi+(1-|\Phi|^2)\Phi,\qquad\Phi\to1\text{ far from the wave}.}
$$

This is a coordinate translation of a traveling solution, rather than an additional phase boost to change the background flow.

Set $\Phi=1+f+ig$ with small real $f,g$. Since $|\Phi|^2=1+2f+O(f^2+g^2)$, the real and imaginary linearized equations are

$$
\boxed{\nabla^2f-2f+2v g_Z=0,\qquad\nabla^2g-2v f_Z=0.}
$$

For a longitudinal sinusoid, choose $f=A\cos(kZ)$ and $g=B\sin(kZ)$. Their coefficients obey

$$
(k^2+2)A=2vkB,\qquad k^2B=2vkA.
$$

A nonzero solution therefore requires $4v^2=k^2+2$, giving the positive-direction [phase velocity](../../../../../../phase-velocity.md)

$$
\boxed{v(k)=\frac12\sqrt{k^2+2}.}
$$

Equivalently the time-dependent linear [Bogoliubov spectrum](../../../../../../bogoliubov-quasiparticle-dispersion.md) is $\omega^2=k^2(k^2+2)/4$ and $v=\omega/k$. Its long-wavelength [sound speed](../../../../../../speed-of-sound.md) is $1/\sqrt2$, which becomes $\sqrt{\mu/m}$ in physical units using $\ell_0/t_0=\sqrt{2\mu/m}$. For a general wavevector $\mathbf k$, the stationary resonance is $4v^2k_z^2=k^2(k^2+2)$; specifying only its magnitude does not determine the [velocity](../../../../../../velocity.md) unless its direction is also fixed. This sinusoidal dispersion describes linear radiation about the background, not an amplitude-independent dispersion law for every nonlinear solitary wave; localized subsonic waves do not require a real oscillatory far-field wavenumber.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
