<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

Here $V(x)$ is [potential energy](../../../../../potential-energy.md), $E$ is the stationary state's total [energy](../../../../../energy-split.md), and $\psi(x)$ is its spatial [probability amplitude](../../../../../probability-amplitude.md). The [wave function](../../../../../wave-function-split.md) has time factor $e^{-iEt/\hbar}$; $|\psi|^2$ is a position [probability density](../../../../../probability-density.md) for a normalized state. Stationary plane-wave scattering solutions are idealizations described by probability-current ratios, or components of a normalizable [wave packet](../../../../../wave-packet.md).

Above an upward step, a classical particle is fully transmitted with reduced [speed](../../../../../speed.md). Quantum mechanically the abrupt [wavelength](../../../../../wavelength.md) change generally produces both reflected and transmitted [amplitudes](../../../../../wave-amplitude.md) even though both regions are classically allowed. With unit incident [amplitude](../../../../../wave-amplitude.md) and no [wave](../../../../../wave-split.md) arriving from the right,

$$
\psi(x)=\begin{cases}e^{ik_1x}+r e^{-ik_1x},&x<0,\\t e^{ik_2x},&x>0,\end{cases}\qquad k_1=\frac{\sqrt{2mE}}{\hbar},\quad k_2=\frac{\sqrt{2m(E-V_0)}}{\hbar}.
$$

The reflected component has signed wavevector $-k_1$ and the same [wavenumber](../../../../../wavenumber.md) magnitude as the incident component. A finite potential jump with constant [mass](../../../../../mass.md) and no delta interaction requires continuity of $\psi$ and $\psi'$:

$$
1+r=t,\qquad k_1(1-r)=k_2t,\qquad\boxed{r=\frac{k_1-k_2}{k_1+k_2},\quad t=\frac{2k_1}{k_1+k_2}.}
$$

The [probability current](../../../../../probability-current.md) $j=(\hbar/m)\operatorname{Im}(\psi^*\psi')$ gives probability reflection and transmission $\mathcal R=|r|^2$ and $\mathcal T=(k_2/k_1)|t|^2$, with $\mathcal R+\mathcal T=1$. The [amplitude](../../../../../wave-amplitude.md) $t$ may exceed one without violating conservation of total probability, because the transmitted group [speed](../../../../../speed.md) is smaller.

For $0<E<V_0$, let $\kappa=\sqrt{2m(V_0-E)}/\hbar$. The bounded right-hand solution is $t e^{-\kappa x}$, an [evanescent wave](../../../../../evanescent-wave.md) tail with [amplitude](../../../../../wave-amplitude.md) penetration scale $1/\kappa$. It carries no outgoing [probability current](../../../../../probability-current.md) in an infinitely long forbidden half-space, so reflection is total. This differs from transmission through a finite [potential barrier](../../../../../potential-barrier.md), where a second boundary can support [quantum tunnelling](../../../../../quantum-tunnelling.md).

For a downward step, replace $k_2$ by $\sqrt{2m(E+V_0)}/\hbar>k_1$. The same [boundary conditions](../../../../../boundary-condition.md) give a nonzero negative $r$, corresponding to a reflected [amplitude](../../../../../wave-amplitude.md) with [phase](../../../../../phase-waves.md) reversal. If reflection were forbidden, $r=0$ would require both $t=1$ and $k_1=k_2$, impossible for a nonzero step. Reflection therefore does not require a classical [potential barrier](../../../../../potential-barrier.md); the discontinuity of [wavenumber](../../../../../wavenumber.md) mismatch is enough.

For the specified [electron](../../../../../electron.md) energies, $k_2/k_1=\sqrt{40/100}=\sqrt{0.4}$, so the requested [amplitude](../../../../../wave-amplitude.md) coefficients are

$$
\boxed{r=0.22515,\qquad t=1.22515.}
$$

The corresponding probability coefficients are approximately $\mathcal R=0.05069$ and $\mathcal T=0.94931$. [electron mass](../../../../../electron-mass.md) cancels from these ratios; there is no need to invent an additional material [effective mass](../../../../../band-effective-mass.md).

## ↑ Ancestors (13)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
