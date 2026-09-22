<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [annihilation operator](../../../../annihilation-operator.md) associated with the new coordinate $X=x-x_0$ is

$$
a'=\sqrt{\frac{m\omega}{2\hbar}}(x-x_0)+\frac{i}{\sqrt{2m\hbar\omega}}p=a-\lambda.
$$

As the initial state is the old vacuum,

$$
\boxed{a'|\Psi(0)\rangle=-\lambda|\Psi(0)\rangle,\qquad
\alpha_0=-\lambda=-\sqrt{\frac{m\omega}{2\hbar}}x_0}.
$$

Equivalently, applying $a'$ to the number-state expansion in part (c) and shifting its summation index returns $-\lambda$ times the same state. It is therefore a [coherent state](../../../../coherent-state.md) of the displaced oscillator.

The new [Hamiltonian](../../../../hamiltonian.md) is $H=U_{\min}+\hbar\omega(a'^\dagger a'+1/2)$. In the [Schrödinger picture](../../../../schrodinger-picture.md) its evolution gives

$$
|\Psi(t)\rangle=e^{-i(U_{\min}/\hbar+\omega/2)t}
 e^{-|\alpha_0|^2/2}\sum_{n=0}^\infty\frac{(\alpha_0e^{-i\omega t})^n}{\sqrt{n!}}|n'\rangle.
$$

Consequently

$$
\boxed{a'|\Psi(t)\rangle=\alpha(t)|\Psi(t)\rangle,\qquad
\alpha(t)=\alpha_0e^{-i\omega t}}.
$$

The displayed prefactor is only a global phase. Equivalently, in the [Heisenberg picture](../../../../heisenberg-picture.md) $a'(t)=a'(0)e^{-i\omega t}$. The mean occupation $|\alpha(t)|^2=\lambda^2$ is constant, and $\hbar\omega(\lambda^2+1/2)$ reproduces the energy above the new minimum found in part (b). Its mean position and momentum likewise reproduce that part's oscillating wavepacket centre.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
