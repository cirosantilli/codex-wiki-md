<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a trajectory connecting the degenerate minima in infinite Euclidean time, the first integral gives $m\dot q^2/2=V(q)$. The [quartic double-well instanton](../../../../../../quartic-double-well-instanton.md) and its reverse are

$$
q_I(t)=a\tanh\frac{\omega(t-t_0)}2,\qquad q_{\bar I}(t)=-q_I(t).
$$

Their action is

$$
\boxed{S_0=\int_{-a}^a\sqrt{2mV(q)}\,dq=\frac{m\omega}{2a}\int_{-a}^a(a^2-q^2)\,dq=\frac23m\omega a^2.}
$$

The [instanton fluctuation prefactor](../../../../../../instanton-fluctuation-prefactor.md) $K$ has dimensions of inverse time. It incorporates nonzero Gaussian fluctuation [eigenvalues](../../../../../../eigenvalue.md) and the translation zero-mode Jacobian; a conventional [determinant](../../../../../../determinant.md) expression is

$$
K=\sqrt{\frac{S_0}{2\pi\hbar}}\left[\frac{\det(-\partial_t^2+\omega^2)}{\det'(-\partial_t^2+V''(q_I)/m)}\right]^{1/2},
$$

with common endpoint regularization and the prime removing the translation mode. Only its positive [quantum tunnelling](../../../../../../quantum-tunnelling.md) rate $\kappa=Ke^{-S_0/\hbar}$ is needed here.

In the [dilute instanton gas](../../../../../../dilute-instanton-gas.md), well-separated crossings alternate in direction. Integrating $n$ ordered centers gives $\tau^n/n!$. A path returning to the same well has $n$ an [even number](../../../../../../even-number.md), and one connecting opposite wells has $n$ an [odd number](../../../../../../odd-number.md). The common leading harmonic endpoint factor follows from the supplied [harmonic oscillator transition kernel](../../../../../../harmonic-oscillator-transition-kernel.md):

$$
\mathcal A_0=\sqrt{\frac{m\omega}{\pi\hbar}},\qquad
\begin{aligned}
\langle a|e^{-H\tau/\hbar}|a\rangle&\simeq\mathcal A_0e^{-\omega\tau/2}\cosh(\kappa\tau),\\
\langle a|e^{-H\tau/\hbar}|-a\rangle&\simeq\mathcal A_0e^{-\omega\tau/2}\sinh(\kappa\tau).
\end{aligned}
$$

Expanding these functions gives the sums over [even numbers](../../../../../../even-number.md) and [odd numbers](../../../../../../odd-number.md), with the position-kernel normalization $\mathcal A_0$ that its abbreviated formula suppresses. Validity requires $S_0/\hbar\gg1$, $\omega\tau\gg1$ and $\kappa\ll\omega$, so typical crossing separation greatly exceeds an [instanton](../../../../../../instanton.md) width. Local anharmonic corrections replace the harmonic well energy by its perturbatively corrected value; the leading formula does not claim uniformly negligible relative error at arbitrarily large $\tau$.

The two exponents identify the [double-well tunneling splitting](../../../../../../double-well-tunneling-splitting.md):

$$
\boxed{E_{\rm even}\simeq\hbar\omega/2-\hbar\kappa,\qquad
E_{\rm odd}\simeq\hbar\omega/2+\hbar\kappa,\qquad\Delta E=2\hbar\kappa.}
$$

The superposition with an [even](../../../../../../even-function.md) spatial [wavefunction](../../../../../../wave-function.md) is the lower state. Coherent [quantum tunnelling](../../../../../../quantum-tunnelling.md) removes the classical degeneracy, and the exponentially small splitting sets the long [quantum tunnelling](../../../../../../quantum-tunnelling.md) timescale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
