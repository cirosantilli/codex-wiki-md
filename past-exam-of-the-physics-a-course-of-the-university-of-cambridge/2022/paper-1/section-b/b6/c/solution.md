<h1 id="section-b/b6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [number operator](../../../../../../number-operator.md) [commutators](../../../../../../commutator.md) established above imply that $\hat a_x^\dagger|n\rangle$ is proportional to $|n+1\rangle$ and $\hat a_x|n\rangle$ to $|n-1\rangle$. Their [norms](../../../../../../norm.md) determine the magnitudes of the proportionality constants:

$$
\|\hat a_x^\dagger|n\rangle\|^2
=\langle n|\hat a_x\hat a_x^\dagger|n\rangle=n+1,
\qquad
\|\hat a_x|n\rangle\|^2
=\langle n|\hat a_x^\dagger\hat a_x|n\rangle=n.
$$

Choose the [phase](../../../../../../phase-waves.md) of the normalized ground [eigenstate](../../../../../../eigenstate.md) once, then define recursively

$$
|n+1\rangle=\frac{\hat a_x^\dagger|n\rangle}{\sqrt{n+1}},
\qquad
|n\rangle=\frac{(\hat a_x^\dagger)^n}{\sqrt{n!}}|0\rangle.
$$

This removes the otherwise arbitrary relative [phases](../../../../../../phase-waves.md) of the [eigenstates](../../../../../../eigenstate.md). The [Hermitian adjoint](../../../../../../adjoint-operator.md) relation then fixes the lowering coefficient with the same positive sign, giving

$$
\boxed{\hat a_x^\dagger|n\rangle=\sqrt{n+1}|n+1\rangle,
\qquad \hat a_x|n\rangle=\sqrt n|n-1\rangle.}
$$

At $n=0$, the second expression means the [zero vector](../../../../../../zero-vector.md), $\hat a_x|0\rangle=0$; it does not introduce a physical state $|-1\rangle$.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
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
