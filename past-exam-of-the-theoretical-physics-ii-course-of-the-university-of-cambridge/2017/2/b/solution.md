<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A normalized oscillator [coherent state](../../../../coherent-state.md) is an [eigenstate](../../../../eigenstate.md) of the [annihilation operator](../../../../annihilation-operator.md), $a|\alpha\rangle=\alpha|\alpha\rangle$. Expanding it in [Fock states](../../../../fock-state.md) gives

$$
|\alpha\rangle=e^{-|\alpha|^2/2}\sum_{n=0}^\infty\frac{\alpha^n}{\sqrt{n!}}|n\rangle.
$$

Since $x=\sqrt{\hbar/(2M\omega)}(a+a^\dagger)$, $\langle a^2\rangle=\alpha^2$, and $\langle aa^\dagger\rangle=|\alpha|^2+1$, the [variance](../../../../variance-split.md) is $\langle x^2\rangle-\langle x\rangle^2=\hbar/(2M\omega)$. Hence

$$
\boxed{\Delta x=\sqrt{\frac{\hbar}{2M\omega}},}
$$

independently of the complex amplitude $\alpha$.

For $A=\alpha a^\dagger$ and $B=-\alpha^*a$, the [commutator](../../../../commutator.md) is the scalar $[A,B]=|\alpha|^2I$. The [Baker--Campbell--Hausdorff formula](../../../../baker-campbell-hausdorff-formula.md) therefore terminates and gives the [displacement operator](../../../../displacement-operator.md)

$$
D(\alpha)=e^{\alpha a^\dagger-\alpha^*a}
=e^{-|\alpha|^2/2}e^{\alpha a^\dagger}e^{-\alpha^*a}.
$$

Because $a|0\rangle=0$, applying it to the [Fock vacuum](../../../../fock-vacuum.md) yields exactly the [Fock state](../../../../fock-state.md) expansion above:

$$
\boxed{|\alpha\rangle=D(\alpha)|0\rangle.}
$$

For a general complex $\alpha$, its [complex conjugate](../../../../complex-conjugate.md) is required in the annihilation term. The expression with $-\alpha a$ printed in the paper is valid when $\alpha$ is real.

## ↑ Ancestors (14)

1. [B](../b.md)
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
