<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Define the [interaction picture](../../../../../interaction-picture.md) by

$$
|\psi_I(t)\rangle=e^{iH_0t/\hbar}|\psi_S(t)\rangle,\qquad
V_I(t)=e^{iH_0t/\hbar}V(t)e^{-iH_0t/\hbar}.
$$

Differentiating and using the [Schrödinger equation](../../../../../schrodinger-equation.md) cancels the $H_0$ terms, leaving

$$
\boxed{i\hbar\frac d{dt}|\psi_I(t)\rangle=\lambda V_I(t)|\psi_I(t)\rangle}.
$$

Its integral equation, iterated once from the initial $|a\rangle$, gives $|\psi_I(t)\rangle=|a\rangle-(i\lambda/\hbar)\int_0^tV_I(t')|a\rangle\,dt'+O(\lambda^2)$.

Since $a,b$ are [orthogonal](../../../../../orthogonal-vectors.md) [energy eigenstates](../../../../../energy-eigenstate.md) with distinct [energies](../../../../../energy.md), the zeroth-order transition amplitude is zero, while

$$
\langle b|V_I(t')|a\rangle
=e^{i(E_b-E_a)t'/\hbar}\langle b|V(t')|a\rangle.
$$

Returning to the Schrodinger picture changes this component only by a unit-modulus phase. Squaring the first-order amplitude therefore gives

$$
\boxed{P_{a\to b}(t)=\frac{\lambda^2}{\hbar^2}
\left|\int_0^t\langle b|V(t')|a\rangle
e^{i(E_b-E_a)t'/\hbar}\,dt'\right|^2+O(\lambda^3)}.
$$

For exponential switching, put $\Delta=E_b-E_a$. The integral is

$$
\langle b|W|a\rangle\,
\frac{\hbar[1-e^{(-\mu+i\Delta)t/\hbar}]}{\mu-i\Delta}.
$$

Because $\mu>0$, its exponential vanishes at late time, yielding

$$
\boxed{P_{a\to b}(\infty)\simeq
\frac{\lambda^2|\langle b|W|a\rangle|^2}{\mu^2+\Delta^2}}.
$$

This is the leading weak-perturbation result, not an exact [probability](../../../../../probability.md) formula at arbitrary coupling.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
