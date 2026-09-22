<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Insert the expansion in the time-dependent [Schrödinger equation](../../../../schrodinger-equation.md), cancel the unperturbed evolution, and project onto $\langle\psi_n|$. With $V_{nm}(t)=\langle\psi_n|V(t)|\psi_m\rangle$,

$$
i\hbar\dot c_n(t)=\sum_m e^{i(\omega_n-\omega_m)t}V_{nm}(t)c_m(t).
$$

In first-order [time-dependent perturbation theory](../../../../time-dependent-perturbation-theory.md), put $c_m(t)=\delta_{m0}$ on the right and use $c_n(-\infty)=0$ for $n\ne0$. Integration gives

$$
\boxed{c_n(t)=\frac1{i\hbar}\int_{-\infty}^t e^{i(\omega_n-\omega_0)t'}V_{n0}(t')\,dt'+O(V^2).}
$$

The initial state must be the specified unperturbed eigenstate, the integral must exist under the switching prescription, and total transition probability must stay small. The diagonal term produces a first-order phase; setting $c_0=1$ in the off-diagonal integral changes those amplitudes only at second order. A weak peak perturbation alone is insufficient if its accumulated action invalidates this expansion.

For the [infinite square well](../../../../infinite-square-well.md), retain the source's zero-based labels:

$$
\psi_n(x)=\sqrt{\frac2w}\sin\frac{(n+1)\pi x}{w},\qquad E_n=\frac{\pi^2\hbar^2(n+1)^2}{2m_ew^2},\qquad n=0,1,\ldots.
$$

An electron in a field along $+x$ has perturbation $V(t)=+eE_0xe^{-t/\tau}$ for $t\geq0$. About the well centre, $x-w/2$ is odd, whereas $\psi_0$ and $\psi_2$ are both even. The constant $w/2$ has zero off-diagonal matrix element, so the [first-order parity selection in an infinite well](../../../../first-order-parity-selection-in-an-infinite-well.md) gives **$\langle\psi_2|x|\psi_0\rangle=0$**. Excitation to that state is forbidden at first order, not necessarily at higher orders.

For the first excited state, direct integration or the supplied integral gives

$$
x_{10}=\frac2w\int_0^w x\sin\frac{2\pi x}w\sin\frac{\pi x}w\,dx=-\frac{16w}{9\pi^2},\qquad
\omega_{10}=\frac{3\pi^2\hbar}{2m_ew^2}.
$$

The Fourier amplitude of the [exponentially decaying electric-field pulse](../../../../exponentially-decaying-electric-field-pulse.md) is $\int_0^\infty e^{-t/\tau+i\omega t}dt=\tau/(1-i\omega\tau)$. Thus

$$
c_1(\infty)=\frac{eE_0x_{10}\tau}{i\hbar(1-i\omega_{10}\tau)},\qquad
\boxed{P_{0\to1}=\frac{256e^2E_0^2w^2\tau^2}{81\pi^4\hbar^2\left[1+\left(3\pi^2\hbar\tau/(2m_ew^2)\right)^2\right]}.}
$$

This is the leading, quadratic-in-field transition probability; the total probability of all excitations must remain small.

Starting instead in $\psi_1$, which is odd about the centre, the pulse can transfer amplitude to the ground state and to even-labelled excited states $\psi_2,\psi_4,\ldots$. Other odd-labelled states have zero first-order dipole amplitude. Both downward and upward transitions are possible; their relative probabilities depend on dipole matrix elements and the pulse's spectral weight at the corresponding energy gaps. Most population remains in $\psi_1$, with a small depletion equal to the summed leading transition probabilities. The [common diagonal dipole phase in an infinite well](../../../../common-diagonal-dipole-phase-in-an-infinite-well.md) is $-eE_0w\tau/(2\hbar)$ and has no population effect. After the pulse, the remaining coherent superposition evolves under the unperturbed [Hamiltonian](../../../../hamiltonian.md); no spontaneous relaxation is implied by this closed-system model.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
