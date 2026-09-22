<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The quadratic part of the covariant-derivative term contains $g^2v^2A_\mu A^\mu/2-gvA_\mu\partial^\mu b$. Its mixing term cancels the $+gvA_\mu\partial^\mu b$ in the stated [gauge fixing](../../../../../gauge-fixing.md) term. Thus the vector [mass](../../../../../mass.md) and diagonal quadratic action are

$$
\boxed{M_A^2=g^2v^2,\qquad M_A=|gv|,}
\qquad
\mathcal L_{A,2}=-\frac14F^2+\frac12M_A^2A^2-\frac1{2\xi}(\partial\cdot A)^2.
$$

For nonzero $p^2$ introduce the transverse and longitudinal [transverse and longitudinal momentum projectors](../../../../../transverse-and-longitudinal-momentum-projectors.md) $P_T^{\mu\nu}=g^{\mu\nu}-p^\mu p^\nu/p^2$ and $P_L^{\mu\nu}=p^\mu p^\nu/p^2$. After integration by parts, the inverse quadratic kernel is

$$
K^{\mu\nu}=-(p^2-M_A^2)P_T^{\mu\nu}
-\frac{p^2-\xi M_A^2}{\xi}P_L^{\mu\nu}.
$$

Their orthogonality makes the inversion immediate. The [gauge-boson propagator](../../../../../gauge-boson-propagator.md) is

$$
\boxed{D_A^{\mu\nu}(p)=-i\left[
\frac{P_T^{\mu\nu}}{p^2-M_A^2+i0}
+\frac{\xi P_L^{\mu\nu}}{p^2-\xi M_A^2+i0}\right].}
$$

Equivalently,

$$
D_A^{\mu\nu}(p)=\frac{-i}{p^2-M_A^2+i0}
\left[g^{\mu\nu}-(1-\xi)\frac{p^\mu p^\nu}{p^2-\xi M_A^2+i0}\right].
$$

The projector formula explains the physical massive pole and the gauge-dependent longitudinal pole. The apparent $1/p^2$ in the projectors cancels in the equivalent expression; it is not an extra massless physical state. At $\xi=1$ the numerator reduces to $g^{\mu\nu}$. At fixed [momentum](../../../../../momentum-split.md) the $\xi\to\infty$ limit gives the [unitary gauge](../../../../../unitary-gauge.md) [propagator](../../../../../propagator.md) $-i(g^{\mu\nu}-p^\mu p^\nu/M_A^2)/(p^2-M_A^2+i0)$. The relation between this limit and ultraviolet power counting is not uniform in [momentum](../../../../../momentum-split.md).[§2.7.3, Higgs-phase gauge-boson masses and the distinction between gauge descriptions and physical spectrum](../../../../../gauge-theory-by-david-tong.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
