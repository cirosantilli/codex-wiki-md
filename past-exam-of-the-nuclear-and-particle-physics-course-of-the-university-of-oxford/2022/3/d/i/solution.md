<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a closed unit-branching [radioactive decay chain](../../../../../decay-chain.md), the [rate equations](../../../../../rate-equation.md) are

$$
\frac{dN_a}{dt}=-\lambda_aN_a,\qquad
\frac{dN_b}{dt}=\lambda_aN_a-\lambda_bN_b.
$$

The first gives $N_a=N_{a0}e^{-\lambda_at}$. Multiply the second by its [integrating factor](../../../../../integrating-factor.md) $e^{\lambda_bt}$:

$$
\frac{d}{dt}(N_be^{\lambda_bt})
=\lambda_aN_{a0}e^{(\lambda_b-\lambda_a)t}.
$$

Integrate from zero to $t$. For $\lambda_a\ne\lambda_b$,

$$
N_b=N_{b0}e^{-\lambda_bt}
+\frac{\lambda_aN_{a0}}{\lambda_b-\lambda_a}
(e^{-\lambda_at}-e^{-\lambda_bt}),
$$

so

$$
\boxed{\alpha=\frac{\lambda_aN_{a0}}{\lambda_b-\lambda_a},\qquad
\beta=N_{b0}-\frac{\lambda_aN_{a0}}{\lambda_b-\lambda_a}.}
$$

The coefficients can individually be negative; the physical population is nonnegative because the production integral is nonnegative. For equal [nuclear decay constants](../../../../../nuclear-decay-constant.md) $\lambda_a=\lambda_b=\lambda$, the finite limit is

$$
\boxed{N_b=(N_{b0}+\lambda N_{a0}t)e^{-\lambda t}.}
$$

A sum of two constant-coefficient copies of the same [exponential function](../../../../../exponential-function.md) cannot represent this limit; the $t$ factor is essential.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the nuclear and particle physics course of the University of Oxford](../../../../split.md)
6. [Nuclear and particle physics course of the University of Oxford](../../../../../nuclear-and-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
