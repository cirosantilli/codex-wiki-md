<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

For a time-independent reference [Hamiltonian](../../../../../hamiltonian.md), define interaction-picture states and observables by

$$
|\psi_I(t)\rangle=e^{iH_0t/\hbar}|\psi_S(t)\rangle,\qquad
O_I(t)=e^{iH_0t/\hbar}O_S(t)e^{-iH_0t/\hbar}.
$$

The transformation is unitary, so matrix elements and expectation values are unchanged; the two pictures make the same physical predictions. Differentiating the state and using the Schrödinger equation cancels the $H_0$ term and gives the [interaction picture](../../../../../interaction-picture.md) evolution

$$
\boxed{i\hbar\partial_t|\psi_I\rangle=V_I(t)|\psi_I\rangle,\quad
V_I=e^{iH_0t/\hbar}V(t)e^{-iH_0t/\hbar}.}
$$

Integrating once and replacing the evolving state in the integral by its initial state gives $|\psi_I(t)\rangle=|n\rangle-(i/\hbar)\int_0^tV_I(t')|n\rangle dt'+O(V^2)$. For $m\ne n$, the first-order transition amplitude therefore yields

$$
\boxed{P_{n\to m}(t)=\frac1{\hbar^2}\left|\int_0^te^{i(E_m-E_n)t'/\hbar}\langle m|V(t')|n\rangle dt'\right|^2+O(V^3).}
$$

For the oscillator, $a|n\rangle=\sqrt n|n-1\rangle$ and $a^\dagger|n\rangle=\sqrt{n+1}|n+1\rangle$. Only neighboring levels have a first-order amplitude. Write $\Delta=\nu-\omega$. The two phase integrals are $\int_0^te^{i\Delta t'}dt'$ and its conjugate, whose squared modulus is $4\sin^2(\Delta t/2)/\Delta^2$. To order $\lambda^2$,

$$
\boxed{P_{n\to n-1}=4\lambda^2n\frac{\sin^2(\Delta t/2)}{\Delta^2},\qquad
P_{n\to n+1}=4\lambda^2(n+1)\frac{\sin^2(\Delta t/2)}{\Delta^2}.}
$$

At resonance take their continuous limits, $\lambda^2nt^2$ and $\lambda^2(n+1)t^2$. All other distinct-level probabilities vanish to this order. Normalization gives $P_{n\to n}=1-4\lambda^2(2n+1)\sin^2(\Delta t/2)/\Delta^2$ to this order, and the downward probability is zero when $n=0$.

The allowed transition rate is proportional to $t\operatorname{sinc}^2(\Delta t/2)$, so its central peak has width of order $1/t$ about $\nu=\omega$. Distributionally, $4\sin^2(\Delta t/2)/(t\Delta^2)\to2\pi\delta(\Delta)$. Thus **both allowed transitions become sharply resonant at the oscillator frequency**. Near the peak, perturbation theory still requires $\lambda^2(n+1)t^2\ll1$; its coherent $t^2$ growth cannot be extrapolated indefinitely at fixed coupling.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
