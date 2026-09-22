<h1 id="section-b/9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) is the [energy eigenvalue](../../../../../energy-eigenvalue-split.md) equation $\widehat H\psi=E\psi$ for a particle of [mass](../../../../../mass.md) $m$. The [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is the sum of the kinetic operator $-(\hbar^2/2m)d^2/dx^2$ and the prescribed [potential energy](../../../../../potential-energy.md) $V(x)$. Here $\hbar$ is the [reduced Planck constant](../../../../../reduced-planck-constant.md). A corresponding [stationary state](../../../../../stationary-state.md) is $\Psi(x,t)=\psi(x)e^{-iEt/\hbar}$. The [Born rule](../../../../../born-rule.md) identifies $|\Psi|^2=|\psi|^2$ as [probability density](../../../../../probability-density.md) for a state with [wavefunction normalization](../../../../../wavefunction-normalization.md) $\int|\Psi|^2dx=1$; integrating it over an interval gives a position [probability](../../../../../probability.md). A [plane wave](../../../../../plane-wave.md) scattering state is not a [normalizable wavefunction](../../../../../normalizable-wavefunction.md) on the whole line, but its [probability currents](../../../../../probability-current.md) give the reflection and transmission fractions of an incident [wave packet](../../../../../wave-packet.md).

There is a notation discrepancy in the sources: the original PDF prints an unbarred $h^2$ in the kinetic term, whereas the local TeX uses $\hbar^2$. The standard physical equation uses the [reduced Planck constant](../../../../../reduced-planck-constant.md) $\hbar=h/(2\pi)$, where $h$ is the [Planck constant](../../../../../planck-constant.md); that convention is used below. Reading the printed $h$ literally as the [Planck constant](../../../../../planck-constant.md) would scale all lengths in this model by $2\pi$ relative to the standard answers, but would leave the amplitude ratios unchanged.

For $E>V_0$, both sides allow oscillatory [wavefunctions](../../../../../wave-function-split.md). A classical particle always crosses the [potential step](../../../../../step-potential.md) and slows because its [kinetic energy](../../../../../kinetic-energy.md) falls from $E$ to $E-V_0$. In [quantum mechanics](../../../../../quantum-mechanics-split.md) there is generally both reflection and transmission even though the particle is above the step. Define the positive [wavenumbers](../../../../../wavenumber.md)

$$
k=\frac{\sqrt{2mE}}\hbar,\qquad q=\frac{\sqrt{2m(E-V_0)}}\hbar.
$$

With no wave incident from the right, write

$$
\psi(x)=\begin{cases}Ae^{ikx}+Be^{-ikx},&x\le0,\\Ce^{iqx},&x>0.\end{cases}
$$

A finite [potential step](../../../../../step-potential.md) with constant [mass](../../../../../mass.md) makes both the [wavefunction](../../../../../wave-function-split.md) and its first [derivative](../../../../../derivative.md) continuous. The two [boundary conditions](../../../../../boundary-condition.md) at $x=0$ are

$$
A+B=C,\qquad k(A-B)=qC.
$$

Solving gives the reflected and transmitted [wavefunctions](../../../../../wave-function-split.md)

$$
\boxed{\psi_{\rm ref}(x)=A\frac{k-q}{k+q}e^{-ikx},\qquad\psi_{\rm tr}(x)=A\frac{2k}{k+q}e^{iqx}.}
$$

For the specified [electron](../../../../../electron.md) energies, $q/k=\sqrt{10/50}=1/\sqrt5$, so the relative [probability amplitudes](../../../../../probability-amplitude.md) are

$$
\boxed{\frac BA=\frac{\sqrt5-1}{\sqrt5+1}=0.381966,\qquad\frac CA=\frac{2\sqrt5}{\sqrt5+1}=1.381966.}
$$

The transmitted [probability amplitude](../../../../../probability-amplitude.md) exceeding one is compatible with [conservation of quantum probability](../../../../../conservation-of-quantum-probability.md), since the outgoing [speed](../../../../../speed.md) is smaller. In fact the [probability current](../../../../../probability-current.md) $j=(\hbar/m)\operatorname{Im}(\psi^*\psi')$ gives

$$
\boxed{\mathcal R=\left|\frac BA\right|^2=0.145898,\qquad\mathcal T=\frac qk\left|\frac CA\right|^2=0.854102,\qquad\mathcal R+\mathcal T=1.}
$$

These are the [quantum reflection probability](../../../../../quantum-reflection-probability.md) and [transmission probability](../../../../../transmission-probability.md), which must be distinguished from the requested relative [amplitudes](../../../../../wave-amplitude.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
