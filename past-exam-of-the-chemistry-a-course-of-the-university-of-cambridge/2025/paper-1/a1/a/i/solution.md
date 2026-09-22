<h1 id="a1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $\widehat V\psi=V(x)\psi$ with real $V$, and $\widehat T=-(\hbar^2/2m)d^2/dx^2$. The [operator domain](../../../../../../operator-domain.md) matters: use sufficiently smooth [wavefunctions](../../../../../../wave-function-split.md) for which the following boundary terms vanish at both infinities. A real multiplication operator gives

$$
\langle f,\widehat Vg\rangle=\int f^*Vg\,dx=\int(Vf)^*g\,dx=\langle\widehat Vf,g\rangle.
$$

Two applications of [integration by parts](../../../../../../integration-by-parts.md) give

$$
\langle f,\widehat Tg\rangle-\langle\widehat Tf,g\rangle
=-\frac{\hbar^2}{2m}[f^*g'-f'^*g]_{-\infty}^{\infty}=0.
$$

Thus the [potential energy](../../../../../../potential-energy.md) and [kinetic energy](../../../../../../kinetic-energy.md) operators obey the stated [Hermitian operator](../../../../../../hermitian-operator.md) identity on this common domain. For $D=d/dx$, one application of [integration by parts](../../../../../../integration-by-parts.md) instead gives

$$
\langle f,Dg\rangle=[f^*g]_{-\infty}^{\infty}-\langle Df,g\rangle=-\langle Df,g\rangle.
$$

The derivative is [anti-Hermitian](../../../../../../skew-hermitian-matrix.md), rather than [Hermitian](../../../../../../hermitian-operator.md); the minus sign cannot generally be removed. Multiplication by $-i\hbar$ makes the corresponding [momentum operator](../../../../../../momentum-operator.md) Hermitian. These integrations establish the requested symmetry identities; full [self-adjointness](../../../../../../self-adjoint-operator.md) of an unbounded operator additionally requires equality of its domain with its adjoint's domain.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [A1](../../../a1.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
