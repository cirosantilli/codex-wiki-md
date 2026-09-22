<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $g=k\hbar/(2m\omega)$, which has units of [energy](../../../../../energy-split.md). In the original oscillator basis,

$$
H=\hbar\omega(a^\dagger a+b^\dagger b+1)
+g(ab+a^\dagger b^\dagger+a^\dagger b+ab^\dagger).
$$

Write $A=\widetilde a$, $B=\widetilde b$, $C_2=\cosh2\theta$ and $S_2=\sinh2\theta$. The transformed number and pair terms obey

$$
a^\dagger a+b^\dagger b+1
=C_2(A^\dagger A+B^\dagger B+1)-S_2(AB+A^\dagger B^\dagger),
$$



$$
ab+a^\dagger b^\dagger
=C_2(AB+A^\dagger B^\dagger)-S_2(A^\dagger A+B^\dagger B+1).
$$

Hence the coefficient of $AB+A^\dagger B^\dagger$ is $gC_2-\hbar\omega S_2$, which vanishes for

$$
\boxed{\tanh2\theta=\frac g{\hbar\omega}=\frac{k}{2m\omega^2},
\qquad\theta=\frac12\operatorname{artanh}\frac{k}{2m\omega^2}.}
$$

**This cancels the requested pair terms but does not diagonalize the printed [Hamiltonian](../../../../../hamiltonian.md).** Its number-conserving coupling also transforms:

$$
a^\dagger b+ab^\dagger
=C_2(A^\dagger B+AB^\dagger)
-\frac{S_2}{2}(A^2+B^2+A^{\dagger2}+B^{\dagger2}).
$$

After the pair cancellation, the last creation terms have coefficient $-gS_2/2$, nonzero for $k\ne0$. They create two quanta from the $A,B$ vacuum, so that vacuum is not an [eigenstate](../../../../../eigenstate.md) of the literal [Hamiltonian](../../../../../hamiltonian.md). This is an inconsistency in the ground-state assertion used by the next part, present in the printed PDF.

For the actual coordinate-coupled system, the [normal coordinates](../../../../../normal-coordinates.md) $q_\pm=(x\pm y)/\sqrt2$ and their conjugate momenta diagonalize $H$ into independent oscillators with

$$
\boxed{\omega_\pm=\sqrt{\omega^2\pm k/m}.}
$$

A normalizable [ground state](../../../../../ground-state.md) requires $|k|<m\omega^2$. Eliminating just the two indicated cross-pair terms is not sufficient to establish that [ground state](../../../../../ground-state.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
