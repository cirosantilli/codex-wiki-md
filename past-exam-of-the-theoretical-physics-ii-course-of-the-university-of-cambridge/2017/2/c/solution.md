<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [quantum state](../../../../quantum-state.md) is continuous through a sudden finite-force [quantum quench](../../../../quantum-quench.md), so it is still $|0\rangle$ at $t=0^+$. Define

$$
\lambda=\frac{F_0}{\sqrt{2M\hbar\omega^3}},\qquad b=a-\lambda,\qquad \theta=\omega t.
$$

The new [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is $H=\hbar\omega(b^\dagger b+1/2)-\hbar\omega\lambda^2$. The old [Fock vacuum](../../../../fock-vacuum.md) obeys $b|0\rangle=-\lambda|0\rangle$, so the [coherent state after shifting an oscillator equilibrium](../../../../coherent-state-after-shifting-an-oscillator-equilibrium.md) rotates with amplitude $-\lambda e^{-i\theta}$ relative to the new equilibrium. In the original oscillator basis, the full state is

$$
\boxed{|\psi(t)\rangle=e^{-i\theta/2+i\lambda^2(\theta-\sin\theta)}
\left|\lambda(1-e^{-i\theta})\right\rangle.}
$$

One way to obtain the phase is to write

$$
e^{-iHt/\hbar}|0\rangle
=e^{-i\theta/2+i\lambda^2\theta}D(\lambda)e^{-i\theta a^\dagger a}D(-\lambda)|0\rangle
$$

and apply the [displacement operator](../../../../displacement-operator.md) composition rule. The [coherent-state oscillator expectation values](../../../../coherent-state-oscillator-expectation-values.md) give

$$
\boxed{\langle x\rangle=\frac{F_0}{M\omega^2}(1-\cos\omega t),\qquad
\langle p\rangle=\frac{F_0}{\omega}\sin\omega t.}
$$

The [position uncertainty](../../../../position-uncertainty.md) stays $\sqrt{\hbar/(2M\omega)}$. These mean values obey the forced classical equation, while the nonzero [variance](../../../../variance-split.md) retains the quantum width.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
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
