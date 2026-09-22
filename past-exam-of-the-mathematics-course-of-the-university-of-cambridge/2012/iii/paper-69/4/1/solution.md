<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are

$$
\rho(\zeta)=\zeta^2-\alpha\zeta-(1-\alpha),\qquad
\sigma(\zeta)=(1-\alpha/4)\zeta^2+(1-3\alpha/4).
$$

Expanding the [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md) gives

$$
\rho(e^w)-w\sigma(e^w)
=\frac{\alpha-2}{3}w^3+\frac{7\alpha-16}{24}w^4+O(w^5).
$$

Thus the formal local consistency order is **two for $\alpha\ne2$**, and **three at $\alpha=2$**, since the fourth-degree coefficient there is $-1/12$. This exceptional formal order is degenerate: $\rho'(1)=\sigma(1)=0$, so it is not a convergent third-order time integrator.

For [zero-stability](../../../../../../zero-stability.md), factor $\rho(\zeta)=(\zeta-1)(\zeta-(\alpha-1))$. The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) requires every root to have modulus at most one and every unit-modulus root to be simple. For real $\alpha$ it holds exactly for

$$
\boxed{0\leq\alpha<2.}
$$

At zero the second root is $-1$, simple and admissible; at two the root one is double and inadmissible. Outside the closed interval the second root has modulus greater than one. The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) says that a consistent linear multistep method is convergent exactly when it is zero-stable, for a locally Lipschitz initial-value problem with consistent starting values and solvable implicit steps. Hence the displayed interval is also exactly the convergence range, and every convergent member has order two.

The [common-factor cancellation defect in a multistep recurrence](../../../../../../common-factor-cancellation-defect-in-a-multistep-recurrence.md) explains why the $\alpha=2$ exception cannot be repaired just by canceling $\zeta-1$. For $y'=0$, its recurrence allows linear growth from a vanishing but insufficiently small starting perturbation: $y_0=0$, $y_1=\sqrt h$ gives $y_n=n\sqrt h$, diverging at a fixed positive time. Canceling the factor silently imposes an additional starting relation and changes the method.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [4](../../4.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
