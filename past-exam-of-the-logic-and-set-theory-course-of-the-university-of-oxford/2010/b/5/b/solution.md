<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For nonzero $\alpha$, consider the exponents $\eta$ with $\omega^\eta\leq\alpha$. The set is nonempty because it contains zero, and bounded because $\omega^\eta\geq\eta$ by [transfinite induction](../../../../../transfinite-induction.md). Let $\delta$ be its supremum. If this supremum is a successor it is attained; if it is a limit, continuity of [ordinal exponentiation](../../../../../ordinal-exponentiation.md) gives $\omega^\delta\leq\alpha$. The zero case is immediate. Thus $\delta$ itself belongs to the set and is its maximum. Maximality gives

$$
\boxed{\omega^\delta\leq\alpha<\omega^{\delta+1}.}
$$

Put $\rho=\omega^\delta>0$. Since $\omega^{\delta+1}=\rho\cdot\omega=\sup_{N<\omega}\rho N$, there is a least positive [natural number](../../../../../natural-number.md) $N$ with $\alpha<\rho N$. We have $N\geq2$ because $\rho\leq\alpha$. Set $n=N-1$. Then

$$
\rho n\leq\alpha<\rho(n+1).
$$

For [ordinals](../../../../../ordinal-split.md) $\xi\leq\alpha$, the final segment of $\alpha$ after its initial segment $\xi$ has an order type $\zeta$ satisfying $\alpha=\xi+\zeta$. Apply this with $\xi=\rho n$. If $\zeta\geq\rho$, monotonicity would give $\alpha\geq\rho n+\rho=\rho(n+1)$, a contradiction. Therefore

$$
\boxed{\alpha=\omega^\delta n+\zeta,\qquad0<n<\omega,\qquad\zeta<\omega^\delta.}
$$

These intervals also make the leading exponent and coefficient unique. The remainder is unique because addition by a fixed left prefix is strictly increasing in its right operand.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
