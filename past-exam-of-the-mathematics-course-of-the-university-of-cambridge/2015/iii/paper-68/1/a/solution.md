<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are

$$
\rho(\zeta)=\zeta^2-1,\qquad \sigma(\zeta)=a\zeta^2+2(1-a)\zeta+a.
$$

The [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) conditions hold for every real $a$:

$$
\rho(1)=0,\qquad \rho'(1)=2=\sigma(1).
$$

Both [roots of a polynomial](../../../../../../root-of-a-polynomial.md) of $\rho$, namely $1$ and $-1$, are simple and have [modulus](../../../../../../modulus.md) one. The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) therefore gives [zero-stability](../../../../../../zero-stability.md) for every $a$. The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) now gives **convergence for every fixed $a\in\mathbb R$**. As usual, this means [convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) on each fixed finite interval for a sufficiently regular [ordinary differential equation](../../../../../../ordinary-differential-equation.md) with a [Lipschitz continuous](../../../../../../lipschitz-continuity.md) [vector field](../../../../../../vector-field.md) and starting values tending to the exact starting values. When $a\ne0$, the [implicit time-stepping method](../../../../../../implicit-time-stepping-method.md) update is locally uniquely solvable for sufficiently small $h$, for example by a [contraction mapping](../../../../../../contraction-mapping.md) if $|ha|L<1$. [Zero-stability](../../../../../../zero-stability.md) does not assert that a large fixed step is suitable for a [stiff differential equation](../../../../../../stiff-equation.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
