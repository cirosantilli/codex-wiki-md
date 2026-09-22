<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [static Lindhard dielectric function](../../../../static-lindhard-dielectric-function.md) describes the real, zero-frequency [linear response](../../../../linear-response-theory.md) of a uniform [free electron gas](../../../../free-electron-model.md). Here $\epsilon_1=\operatorname{Re}\epsilon$, $\mathbf r$ is the position operator, and $\mathbf q$ is the perturbation [wavevector](../../../../wavevector.md), $q=|\mathbf q|$, $V$ the normalization volume, $e>0$ the elementary charge, and $\epsilon_0$ the vacuum [permittivity](../../../../permittivity-split.md). The normalized one-electron states are $\psi_{\mathbf k}=V^{-1/2}e^{i\mathbf k\cdot\mathbf r}$ with $E_{\mathbf k}=\hbar^2k^2/(2m_e)$; $f(E)$ is their [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) occupation. Both momentum sums exclude spin; the prefactor two counts the two equal [spin](../../../../spin.md) populations. The density-operator matrix element is $\delta_{\mathbf k',\mathbf k+\mathbf q}$. Coincident energy denominators are interpreted by the static limit or [Cauchy principal value](../../../../cauchy-principal-value.md).

A weak total [electric potential](../../../../electric-potential.md) $\phi_{\rm tot}$ perturbs an electron by $-e\phi_{\rm tot}$. First-order state mixing produces $\delta n=e\Pi_0(q)\phi_{\rm tot}$, where

$$
\Pi_0(q)=\frac2V\sum_{\mathbf k}\frac{f(E_{\mathbf k})-f(E_{\mathbf k+\mathbf q})}{E_{\mathbf k+\mathbf q}-E_{\mathbf k}}.
$$

The induced charge is $-e\delta n$. Self-consistent [Poisson equation](../../../../poisson-s-equation.md) screening then gives $\phi_{\rm ext}=\epsilon\phi_{\rm tot}$, with $\epsilon=1+e^2\Pi_0/(\epsilon_0q^2)$. This is the [random phase approximation](../../../../random-phase-approximation.md): use the independent-electron response to the self-consistent total field.[Chapter8,§8.3, printed pp.123–126: density response and the Lindhard function](../../../../lecture-notes-for-quantum-matter-by-steven-h-simon.md)

At zero temperature $f(E_{\mathbf k})=\Theta(k_F-k)$. Shifting the integration variable in the second occupation term gives

$$
\epsilon-1=\frac{4m_ee^2}{\epsilon_0\hbar^2q^2}\int_{k<k_F}\frac{d^3k}{(2\pi)^3}\left(\frac1{q^2+2\mathbf k\cdot\mathbf q}+\frac1{q^2-2\mathbf k\cdot\mathbf q}\right).
$$

The two angular integrals are equal. Using the supplied integral, with $x=q/(2k_F)$, gives

$$
\boxed{\epsilon(q,0)=1+\frac{\kappa^2}{q^2}F(x),\qquad
\kappa^2=\frac{m_ee^2k_F}{\epsilon_0\pi^2\hbar^2},\qquad
F(x)=\frac12+\frac{1-x^2}{4x}\log\left|\frac{1+x}{1-x}\right|.}
$$

The limits are $F(0)=1$, $F(1)=1/2$ and $F(x)\sim1/(3x^2)$ for large $x$. The first recovers [Thomas-Fermi screening](../../../../thomas-fermi-screening.md); the logarithm produces the [Kohn singularity of static Lindhard screening](../../../../kohn-singularity-of-static-lindhard-screening.md) at $q=2k_F$.

Use the [Fourier transform](../../../../fourier-transform-split.md) convention $\rho(\mathbf q)=\int d^3r\,e^{-i\mathbf q\cdot\mathbf r}\rho(\mathbf r)$. A point charge $Ze$ has total screened charge $Ze/\epsilon(q)$ and induced charge $-Ze[1-\epsilon(q)^{-1}]$. Angular inversion therefore gives the [radial induced-charge screening kernel](../../../../radial-induced-charge-screening-kernel.md)

$$
\rho_{\rm ind}(r)=-\frac{Ze}{r}\int_0^\infty dq\,g(q)\sin(qr),\qquad
\boxed{g(q)=\frac{q}{2\pi^2}\left[1-\frac1{\epsilon(q)}\right]=\frac{q\kappa^2F(q/2k_F)}{2\pi^2[q^2+\kappa^2F(q/2k_F)]}.}
$$

In particular, $\rho_{\rm ind}(\mathbf q=0)=-Ze$: the total screening charge is negative although its local density can oscillate in sign.

Integrate the sine transform by parts twice; $g(0)=g(\infty)=0$ removes the boundary terms. For the [Friedel density tail from a derivative singularity](../../../../friedel-density-tail-from-a-derivative-singularity.md), write $Q=2k_F$ and $g''(q)\sim C/(q-Q)$. Then

$$
\rho_{\rm ind}(r)=\frac{Ze}{r^3}\int_0^\infty g''(q)\sin(qr)\,dq
\sim\frac{ZeC\pi}{r^3}\cos(Qr).
$$

Indeed, near $Q$ the [principal value](../../../../cauchy-principal-value.md) transform is $\int_{-\infty}^{\infty}\sin[(Q+s)r]\,ds/s=\pi\cos(Qr)$ for $r>0$. Smooth terms do not remove this leading oscillatory long-range contribution. Thus **$\rho_{\rm ind}\propto\cos(2k_Fr)/r^3$**.

For a three-dimensional, single-valley gas with two [spin](../../../../spin.md) states, the [Friedel oscillation wavelength from carrier density](../../../../friedel-oscillation-wavelength-from-carrier-density.md) is

$$
\boxed{k_F=(3\pi^2n)^{1/3}=3.90\times10^8\,\mathrm{m^{-1}},\qquad
\lambda=\frac{\pi}{k_F}=8.06\,\mathrm{nm}.}
$$

Low-temperature [scanning tunneling spectroscopy](../../../../scanning-tunneling-spectroscopy.md) near exposed dopants can map the oscillatory [local density of states](../../../../local-density-of-states.md), with a Fourier feature near $2k_F$ at the [Fermi energy](../../../../fermi-energy.md). An energy-resolved tunnelling image measures local spectral weight, not directly the bulk energy-integrated charge: comparing occupied-bias maps and accounting for the surface geometry is necessary. In actual [GaAs](../../../../gallium-arsenide.md), the background [relative permittivity](../../../../relative-permittivity.md) and band [effective mass](../../../../band-effective-mass.md) change screening strengths; they do not change this wavelength at the stated density.

<a id="1/image-static-lindhard-screening-has-a-singular-slope-at-twice-the-fermi-wavevector-and-an-oscillatory-far-field-density-tail"></a>
![](../../../../past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2013/paper-1-aqc2013-screening-and-tail.png)

**[Figure 1](#1/image-static-lindhard-screening-has-a-singular-slope-at-twice-the-fermi-wavevector-and-an-oscillatory-far-field-density-tail). Static Lindhard screening has a singular slope at twice the Fermi wavevector and an oscillatory far-field density tail**. [Source](paper-1-aqc2013-screening-and-tail.py).

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
