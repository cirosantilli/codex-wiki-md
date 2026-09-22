<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Introduce a bookkeeping parameter $\lambda$ in $H=H_0+\lambda H_1$ and expand $|\phi_n\rangle=|\psi_n\rangle+\lambda|\eta_n\rangle+O(\lambda^2)$ and $\mathcal E_n=E_n+\lambda\Delta E_n+O(\lambda^2)$. Fix [phase](../../../../phase-waves.md) and normalization at this order by $\langle\psi_n|\eta_n\rangle=0$. The first-order Schrödinger equation is

$$
(H_0-E_n)|\eta_n\rangle=-(H_1-\Delta E_n)|\psi_n\rangle.
$$

[angular momentum](../../../../angular-momentum.md) projection onto $\langle\psi_n|$ gives $\Delta E_n=\langle\psi_n|H_1|\psi_n\rangle$. [angular momentum](../../../../angular-momentum.md) projection onto a different [eigenstate](../../../../eigenstate.md) gives

$$
\langle\psi_j|\eta_n\rangle=\frac{\langle\psi_j|H_1|\psi_n\rangle}{E_n-E_j},\qquad j\ne n.
$$

Completeness therefore yields the [first-order nondegenerate perturbation theory](../../../../first-order-nondegenerate-perturbation-theory.md) result

$$
\boxed{|\phi_n\rangle=|\psi_n\rangle+\sum_{j\ne n}
\frac{\langle\psi_j|H_1|\psi_n\rangle}{E_n-E_j}|\psi_j\rangle+O(H_1^2).}
$$

Nonzero [energy](../../../../energy-split.md) denominators are essential. The displayed state has unit norm through first order; exact normalization would change terms of second order. A continuum, if present, contributes its corresponding [integral](../../../../integral-split.md) as well as any discrete sum.

For the oscillator in a static [electric field](../../../../electric-field-split.md), electrostatic [potential energy](../../../../potential-energy.md) is $H_1=-q\epsilon x$ and $\omega=\sqrt{k/m}$. [parity](../../../../parity.md) gives $\langle0|x|0\rangle=0$, and the supplied Gaussian [wavefunctions](../../../../wave-function-split.md) give

$$
x_{\rm zp}\equiv\langle1|x|0\rangle
=\sqrt{2\alpha}\int x^2|\psi_0(x)|^2dx
=\frac1{\sqrt{2\alpha}}=\sqrt{\frac{\hbar}{2m\omega}}.
$$

Since $E_0-E_1=-\hbar\omega$, the two-state first-order [ground state](../../../../ground-state.md) is

$$
|\phi_0\rangle=|0\rangle+\eta|1\rangle+O(\epsilon^2),\qquad
\eta=\frac{q\epsilon x_{\rm zp}}{\hbar\omega}.
$$

Thus $\langle x\rangle=2\eta x_{\rm zp}+O(\epsilon^2)$, and the induced electric dipole is

$$
\boxed{d=q\langle x\rangle=\frac{q^2\epsilon}{m\omega^2}=\frac{q^2}{k}\epsilon
\quad\text{to first order}.}
$$

It is aligned with the field for either sign of $q$. The [harmonic-oscillator electric polarizability](../../../../harmonic-oscillator-electric-polarizability.md) is $q^2/k$. The [position operator](../../../../position-operator.md) connects $|0\rangle$ only to $|1\rangle$, so the requested two-state calculation contains the complete first-order dipole response, rather than dropping other first-order terms.

Complete the square to find the exact [electric-field displacement of a quantum harmonic oscillator](../../../../electric-field-displacement-of-a-quantum-harmonic-oscillator.md):

$$
H=\frac{p^2}{2m}+\frac12k(x-x_0)^2-\frac{q^2\epsilon^2}{2k},\qquad x_0=\frac{q\epsilon}{k}.
$$

The exact normalized ground [wavefunction](../../../../wave-function-split.md) is $\psi_0(x-x_0)$, with [energy](../../../../energy-split.md) $\hbar\omega/2-q^2\epsilon^2/(2k)$. Its mean displacement is $x_0$, so

$$
\boxed{d_{\rm exact}=q x_0=\frac{q^2\epsilon}{k}.}
$$

**The first-order dipole equals the exact dipole**, because the restoring force is exactly linear and translating a harmonic well does not change its width or [frequency](../../../../frequency.md). This agreement of one expectation value does not make the truncated [wavefunction](../../../../wave-function-split.md) exact. The [Hellmann–Feynman theorem](../../../../hellmann-feynman-theorem.md) provides an independent check: $d=-\partial E_0/\partial\epsilon$.

For [perturbation theory](../../../../perturbation-theory.md) to approximate the state, $|\eta|\ll1$, or $|x_0|\ll2x_{\rm zp}$. The exact translated [ground state](../../../../ground-state.md) has the original-oscillator expansion

$$
|0;x_0\rangle=e^{-\eta^2/2}\sum_{n=0}^{\infty}\frac{\eta^n}{\sqrt{n!}}|n\rangle.
$$

It is a [coherent state](../../../../coherent-state.md) with mean occupation $\eta^2$. Large fields require many oscillator levels, whereas the first-order state retains only two. The [normalized two-state truncation of a displaced oscillator](../../../../normalized-two-state-truncation-of-a-displaced-oscillator.md) instead gives

$$
|\phi_{01}\rangle=\frac{|0\rangle+\eta|1\rangle}{\sqrt{1+\eta^2}},\qquad
\langle x\rangle_{01}=\frac{x_0}{1+\eta^2},
$$

which incorrectly tends towards zero for large $|\eta|$ instead of following the displaced well. In [position](../../../../position.md) space the truncated polynomial times Gaussian also develops a node absent from the exact [ground state](../../../../ground-state.md). Taking a linearized formula outside its small-state-correction regime is therefore invalid even though its dipole coefficient happens to be exact.

<a id="3/image-exact-translated-ground-state-compared-with-its-normalized-two-state-truncation-at-weak-and-strong-displacement"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1-displaced-oscillator.png)

**[Figure 4](#3/image-exact-translated-ground-state-compared-with-its-normalized-two-state-truncation-at-weak-and-strong-displacement). Exact translated ground state compared with its normalized two-state truncation at weak and strong displacement**.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
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
