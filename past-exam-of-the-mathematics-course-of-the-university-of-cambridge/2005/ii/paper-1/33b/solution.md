<h1 id="33b/solution">Solution</h1>

↑ **Parent:** [33B](../33b.md)

The [differential scattering cross-section](../../../../../differential-scattering-cross-section.md) is scattered rate per unit solid angle divided by incident flux. For the outgoing scattering solution, the incident plane wave has current magnitude $\hbar k/m$, while the outgoing spherical wave has radial current $(\hbar k/m)|f(\widehat x)|^2/r^2$. Therefore

$$
\boxed{\frac{d\sigma}{d\Omega}=|f(\widehat x)|^2.}
$$

The incoming plane-wave normalization and outgoing radiation condition select the physical scattering state.

The [Time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) is $[-\hbar^2\nabla^2/(2m)+V]\psi=E\psi$, equivalently $(\nabla^2+k^2)\psi=(2m/\hbar^2)V\psi$. The given outgoing Helmholtz fundamental solution has source $-4\pi\delta$. Multiplying it by the source and adding the incident homogeneous solution gives

$$
\psi(x)=e^{i\mathbf k\cdot x}-\frac{m}{2\pi\hbar^2}\int\frac{e^{ik|x-x'|}}{|x-x'|}V(r')\psi(x')\,d^3x'.
$$

Applying $\nabla^2+k^2$ verifies its equation and sign. At large $r$, $|x-x'|=r-\widehat x\cdot x'+O(r^{-1})$ and $|x-x'|^{-1}=r^{-1}+O(r^{-2})$ over the potential's support. Consequently

$$
f(\widehat x)=-\frac{m}{2\pi\hbar^2}\int e^{-ik\widehat x\cdot x'}V(r')\psi(x')\,d^3x'.
$$

The [Born approximation](../../../../../born-approximation.md) replaces $\psi(x')$ by the incident wave, giving

$$
\boxed{f_B(\widehat x)=F(k\widehat x-\mathbf k),\qquad F(q)=-\frac{m}{2\pi\hbar^2}\int e^{-iq\cdot x}V(r)\,d^3x.}
$$

It requires weak wave distortion. A sufficient smallness condition from the [integral](../../../../../integral.md) equation is $(m/2\pi\hbar^2)\sup_x\int |V(x')|/|x-x'|\,d^3x'\ll1$; for a bounded potential of range $R$ this is of order $m|V_0|R^2/\hbar^2\ll1$. At high [energy](../../../../../energy.md) a small accumulated phase and weak deflection can also justify the approximation, but small potential relative to [energy](../../../../../energy.md) alone is not sufficient for an arbitrarily long interaction range.

For the exponentially screened potential, angular integration in its [Fourier transform](../../../../../fourier-transform.md) gives

$$
\int e^{-iq\cdot x}\frac{Ke^{-\mu r}}r\,d^3x=\frac{4\pi K}{q}\int_0^\infty e^{-\mu r}\sin(qr)\,dr=\frac{4\pi K}{q^2+\mu^2}.
$$

It is not compactly supported, but for $\mu>0$ its decay gives the same scattering asymptotics and convergent [integrals](../../../../../integral.md). Since $q=2k\sin(\theta/2)$,

$$
\boxed{f_B(\theta)=-\frac{2mK}{\hbar^2[4k^2\sin^2(\theta/2)+\mu^2]}\ \longrightarrow\ -\frac{K}{4E\sin^2(\theta/2)}\quad(\mu\to0,\ \theta\ne0).}
$$

Thus the Born amplitude in this limit is independent of $\hbar$ when expressed using $E$ and angle; its squared magnitude is the Rutherford cross-section. This is a fixed-nonzero-angle limit of the Born formula. It does not establish uniform validity in the forward direction or preserve the short-range outgoing-wave asymptotics for the unscreened Coulomb potential.

## ↑ Ancestors (10)

1. [33B](../33b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
