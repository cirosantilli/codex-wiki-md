<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For this [two-step family with a third-order member](../../../../../../two-step-family-with-a-third-order-member.md), use the [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md). Expanding the exact-solution residual symbol gives

$$
\rho(e^z)-z\sigma(e^z)
=-\frac{1+5a}{12}z^3-\frac{3+11a}{24}z^4+O(z^5).
$$

The constant, linear and quadratic coefficients vanish for every parameter. Thus

$$
\boxed{p=2\text{ for }a\ne-1/5,\qquad p=3\text{ for }a=-1/5.}
$$

At the exceptional value the fourth-degree coefficient is $-1/30$, so there is no further increase. This means an unscaled exact-solution residual of order $h^{p+1}$, or a residual divided by the step of order $h^p$.

The first characteristic [polynomial](../../../../../../polynomial-split.md) factors as $\rho(w)=(w-1)(w-a)$. The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) requires every root to have modulus at most one and each unit-modulus root to be simple. The root $a=-1$ is allowed because it is distinct from the simple root one; $a=1$ is not, since it makes one a double root. Hence [zero-stability](../../../../../../zero-stability.md) holds exactly for

$$
\boxed{-1\leq a<1.}
$$

On this interval, $\rho(1)=0$ and $\rho'(1)=\sigma(1)=1-a\ne0$ establish [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md). The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md), for a fixed-step consistent [linear multistep method](../../../../../../linear-multistep-method.md) applied to an [ordinary differential equation](../../../../../../ordinary-differential-equation.md) with a [Lipschitz continuous](../../../../../../lipschitz-continuity.md) right-hand side with convergent starting values and well-defined small-step updates, says that [convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) is equivalent to [zero-stability](../../../../../../zero-stability.md). Therefore the same interval is exactly the [convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) range. With sufficiently accurate starting values the convergent members have the orders just computed.

At $a=1$ the [Taylor expansion](../../../../../../taylor-expansion.md) still gives a formal order-two residual, but $\rho'(1)=\sigma(1)=0$ and the double root prevents a convergent method. Canceling the common factor $w-1$ produces the [common-factor cancellation defect in a multistep recurrence](../../../../../../common-factor-cancellation-defect-in-a-multistep-recurrence.md) and changes the starting relations and cannot repair [convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) of the original recurrence. At $a=0$, cancellation of a zero root instead reveals the ordinary [trapezoidal rule](../../../../../../trapezoidal-rule.md); it is consistent with the order-two result.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
