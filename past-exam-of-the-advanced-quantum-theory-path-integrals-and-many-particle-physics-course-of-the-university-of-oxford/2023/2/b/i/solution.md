<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the specified positive-exponent [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md), the [inverse discrete Fourier transforms](../../../../../inverse-discrete-fourier-transform.md) have negative exponents:

$$
\boxed{a_n=\frac1{\sqrt L}\sum_qe^{-iqn}A_q,\qquad
b_n=\frac1{\sqrt L}\sum_qe^{-iqn}B_q.}
$$

Every sum runs over $q=2\pi j/L$, $j=0,\ldots,L-1$. Indeed, [orthogonality of roots of unity](../../../../../orthogonality-of-roots-of-unity.md) gives

$$
\frac1L\sum_qe^{iq(r-n)}=\delta_{rn},
$$

so substituting the forward [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md) into either proposed inverse recovers the original operator. Taking [Hermitian conjugates](../../../../../hermitian-conjugation.md) supplies the inverse formulas for the [creation operators](../../../../../creation-operator.md).

Multiplying the inverse [discrete Fourier transforms](../../../../../discrete-fourier-transform-split.md) gives the local [number operator](../../../../../number-operator.md) combination

$$
\boxed{\frac12(a_n^\dagger a_n+b_n^\dagger b_n)
=\frac1{2L}\sum_{q,k}e^{i(q-k)n}
\left(A_q^\dagger A_k+B_q^\dagger B_k\right).}
$$

This local expression includes off-diagonal [momentum](../../../../../momentum-split.md) terms. Only after summing over sites does [orthogonality of roots of unity](../../../../../orthogonality-of-roots-of-unity.md) give

$$
\frac12\sum_n(a_n^\dagger a_n+b_n^\dagger b_n)
=\frac12\sum_q(A_q^\dagger A_q+B_q^\dagger B_q).
$$

In a physical fixed-$s$ state the first boxed operator acts as $s$ at every site, by the [local spin constraint in the Schwinger boson representation](../../../../../local-spin-constraint-in-the-schwinger-boson-representation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
