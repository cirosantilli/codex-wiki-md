<h1 id="section-b/b9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a normalized state, the [expectation value](../../../../../../expectation-value.md) is

$$
\boxed{\langle Q\rangle=\langle\psi|Q|\psi\rangle=\int\psi^*(x,t)\,Q\psi(x,t)\,dx.}
$$

For a time-independent operator, differentiation gives

$$
\frac d{dt}\langle Q\rangle=\langle\dot\psi|Q|\psi\rangle+\langle\psi|Q|\dot\psi\rangle.
$$

The [Schrödinger equation](../../../../../../schrodinger-equation.md) says $|\dot\psi\rangle=-iH|\psi\rangle/\hbar$. The [self-adjointness](../../../../../../self-adjoint-operator.md) of $H$ gives $\langle\dot\psi|=i\langle\psi|H/\hbar$, so

$$
\frac d{dt}\langle Q\rangle=\frac i\hbar\langle HQ-QH\rangle=\boxed{\frac1{i\hbar}\langle[Q,H]\rangle.}
$$

In the [integral](../../../../../../integral-split.md) derivation, the same [self-adjointness](../../../../../../self-adjoint-operator.md) step is integration by parts with vanishing boundary terms. An explicitly time-dependent observable would also contribute $\langle\partial Q/\partial t\rangle$. These are the expectation-value equations underlying the [Heisenberg equation of motion](../../../../../../heisenberg-equation-of-motion.md).

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B9](../../b9.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
