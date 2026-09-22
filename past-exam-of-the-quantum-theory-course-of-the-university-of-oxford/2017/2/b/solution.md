<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\gamma=2m\hbar\omega$. If $\psi_n$ is a normalized [energy eigenstate](../../../../energy-eigenstate.md) at $E_n$, the factorization from part (a) gives

$$
\|a_+\psi_n\|^2=\langle\psi_n,a_-a_+\psi_n\rangle=\gamma(n+1).
$$

It follows inductively that $v_n=(a_+)^n\psi_0$ has squared [norm](../../../../norm.md) $\gamma^n n!$. The [commutator](../../../../commutator.md) with $H$ establishes its [energy eigenvalue](../../../../energy-eigenvalue-split.md) at each step. Hence

$$
\boxed{\psi_n=\frac{(a_+)^n\psi_0}{(2m\hbar\omega)^{n/2}\sqrt{n!}}}
$$

is normalized and has $E_n=(n+\tfrac12)\hbar\omega$. Distinct levels are [orthogonal](../../../../orthogonal-vectors.md) because $H$ is a [self-adjoint operator](../../../../self-adjoint-operator.md). In particular,

$$
a_+\psi_n=\sqrt{\gamma(n+1)}\,\psi_{n+1},\qquad a_-\psi_n=\sqrt{\gamma n}\,\psi_{n-1}.
$$

To decompose the specified initial [wavefunction](../../../../wave-function-split.md), retain this exact phase convention for the [creation and annihilation operators](../../../../creation-and-annihilation-operators.md). Their difference gives

$$
X=\frac{a_+-a_-}{2im\omega}.
$$

Since $a_-\psi_0=0$ and $a_-a_+\psi_0=\gamma\psi_0$,

$$
\begin{aligned}
X^2\psi_0&=-\frac1{4m^2\omega^2}(a_+^2-a_+a_--a_-a_++a_-^2)\psi_0\\
&=\frac{\hbar}{2m\omega}\left(\psi_0-\sqrt2\,\psi_2\right).
\end{aligned}
$$

This [quadratic excitation of an oscillator ground state](../../../../quadratic-excitation-of-an-oscillator-ground-state.md), $\Psi(x,0)=C_0^{-1}X^2\psi_0$, contains only the $n=0$ and $n=2$ [energy eigenstates](../../../../energy-eigenstate.md). The printed initial function has an unspecified overall normalization, so the [Born rule](../../../../born-rule.md) requires division by its squared [norm](../../../../norm.md). After [wavefunction normalization](../../../../wavefunction-normalization.md) the state is

$$
\frac1{\sqrt3}\psi_0-\sqrt{\frac23}\psi_2.
$$

The minus sign is consistent with the paper's convention: its $a_+$ is $i$ times the usual real-coordinate raising operator multiplied by $\sqrt\gamma$, so its $\psi_2$ has the opposite sign to the usual real second [harmonic oscillator eigenfunction](../../../../harmonic-oscillator-eigenfunction.md). The [energy measurement](../../../../energy-measurement.md) probabilities are independent of this choice of phase.

Therefore the complete answer is

$$
\boxed{\Pr\left(E=\frac12\hbar\omega\right)=\frac13,\qquad \Pr\left(E=\frac52\hbar\omega\right)=\frac23.}
$$

**Every other energy has probability zero.** At any later time the two coefficients only acquire their separate [dynamical phases](../../../../dynamical-phase.md), so these [probabilities](../../../../probability.md) remain the same. A direct check of the normalization is

$$
\int_{-\infty}^{\infty}x^4e^{-\alpha x^2}\,dx=\frac{d^2}{d\alpha^2}\sqrt{\frac\pi\alpha}=\frac{3\sqrt\pi}{4\alpha^{5/2}},\qquad \alpha=\frac{m\omega}{\hbar}.
$$

This also confirms the factor of three in the squared [norm](../../../../norm.md) of the two-component expansion.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
