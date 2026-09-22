<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

Set $a=\sqrt{m\omega/(2\hbar)}x+\sqrt{\hbar/(2m\omega)}\,d/dx$ and let $a^\dagger$ have the opposite derivative sign. On the bound-state domain, $[a,a^\dagger]=1$ and $H=\hbar\omega(a^\dagger a+1/2)$. Thus every [energy eigenvalue](../../../../energy-eigenvalue-split.md) has $E/\hbar\omega-1/2=\nu\geq0$.

The [lowering operator](../../../../lowering-operator.md) maps an eigenstate of $a^\dagger a$ of [eigenvalue](../../../../eigenvalue.md) $\nu$ to one of [eigenvalue](../../../../eigenvalue.md) $\nu-1$, with squared [norm](../../../../norm.md) multiplied by $\nu$. Repeated lowering cannot pass below zero, so it must terminate at zero. Hence $\nu$ is a nonnegative integer. The equation $a\psi_0=0$ gives a Gaussian [ground state](../../../../ground-state.md), and repeated raising gives a nonzero [square-integrable](../../../../square-integrable-function.md) state for every integer $n\geq0$. Therefore

$$
\boxed{E_n=\hbar\omega(n+1/2),\qquad n=0,1,2,\ldots.}
$$

These are also the Gaussian-times-Hermite-[polynomial](../../../../polynomial-split.md) solutions obtained by the suggested series method.

Put $\alpha=m\omega/\hbar$. Normalization gives $\psi_0=(\alpha/\pi)^{1/4}e^{-\alpha x^2/2}$, so

$$
\langle|x|\rangle=2\sqrt{\frac\alpha\pi}\int_0^\infty xe^{-\alpha x^2}dx
=\boxed{\sqrt{\frac\hbar{\pi m\omega}}}.
$$

The [expectation](../../../../expected-value-split.md) of $x$ itself is zero by [parity](../../../../parity.md); that cancellation does not apply to its absolute value.

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
