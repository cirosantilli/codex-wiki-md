<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

Writing $a=cx+idp$, where $c=\sqrt{m\omega/(2\hbar)}$ and $d=1/\sqrt{2m\omega\hbar}$, the [canonical commutation relation](../../../../../canonical-commutation-relation.md) gives

$$
[a,a^\dagger]=-2icd[x,p]=2cd\hbar=\boxed{1}.
$$

Consequently $[a^\dagger a,a]=-a$ and $\boxed{[H,a]=-\hbar\omega a}$. If $a|\phi_0\rangle$ were nonzero, this [commutator](../../../../../commutator.md) would make it an [energy eigenstate](../../../../../energy-eigenstate.md) with [energy](../../../../../energy-split.md) $E_0-\hbar\omega$, contradicting the lowest-energy property. Therefore **$a|\phi_0\rangle=0$**.

The [commutator product rule](../../../../../commutator-product-rule.md) and induction give

$$
[a,(a^\dagger)^{n+1}]
=[a,(a^\dagger)^n]a^\dagger+(a^\dagger)^n[a,a^\dagger]
=(n+1)(a^\dagger)^n.
$$

Acting on the vacuum and shifting the sum then shows that the [unnormalized bosonic coherent state](../../../../../unnormalized-bosonic-coherent-state.md) $|\widetilde\psi\rangle=e^{\alpha a^\dagger}|0\rangle$ satisfies $a|\widetilde\psi\rangle=\alpha|\widetilde\psi\rangle$.

**The displayed series lacks its [wavefunction normalization](../../../../../wavefunction-normalization.md) factor.** Since $(a^\dagger)^n|0\rangle=\sqrt{n!}|n\rangle$, its squared norm is $\sum_n|\alpha|^{2n}/n!=e^{|\alpha|^2}$. The normalized [coherent state](../../../../../coherent-state.md) needed for the stated [expectation values](../../../../../expectation-value.md) is

$$
|\alpha\rangle=e^{-|\alpha|^2/2}\sum_{n=0}^{\infty}\frac{\alpha^n}{\sqrt{n!}}|n\rangle,
\qquad a|\alpha\rangle=\alpha|\alpha\rangle.
$$

Use $\langle a\rangle=\alpha$, $\langle a^\dagger\rangle=\alpha^*$, $\langle a^\dagger a\rangle=|\alpha|^2$ and $\langle aa^\dagger\rangle=|\alpha|^2+1$. For $x=x_0(a+a^\dagger)$, $x_0=\sqrt{\hbar/(2m\omega)}$,

$$
\langle x\rangle=x_0(\alpha+\alpha^*),\qquad
\langle x^2\rangle=x_0^2\left[(\alpha+\alpha^*)^2+1\right],
\qquad \boxed{\Delta x=\sqrt{\frac{\hbar}{2m\omega}}}.
$$

The displacement changes the mean position but not its ground-state uncertainty. Unnormalized bras and kets give the same physical [expectation values](../../../../../expectation-value.md) only after division by their squared norm.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
