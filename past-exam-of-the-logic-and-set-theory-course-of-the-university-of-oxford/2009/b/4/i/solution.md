<h1 id="b/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [ordinal](../../../../../ordinal-split.md) operations are defined by [transfinite recursion](../../../../../transfinite-recursion.md) in the right argument. Addition satisfies $\alpha+0=\alpha$, $\alpha+(\beta+1)=(\alpha+\beta)+1$, and $\alpha+\lambda=\sup_{\beta<\lambda}(\alpha+\beta)$ at a nonzero limit. Multiplication satisfies $\alpha\cdot0=0$, $\alpha\cdot(\beta+1)=\alpha\cdot\beta+\alpha$, and $\alpha\cdot\lambda=\sup_{\beta<\lambda}\alpha\cdot\beta$. Exponentiation satisfies $\alpha^0=1$, $\alpha^{\beta+1}=\alpha^\beta\cdot\alpha$, and $\alpha^\lambda=\sup_{\beta<\lambda}\alpha^\beta$ at nonzero limits. These are [ordinal](../../../../../ordinal-split.md) operations, not commutative [cardinal arithmetic](../../../../../cardinal-arithmetic.md).

For a [normal function on an ordinal](../../../../../normal-function-on-an-ordinal.md), prove domination by [transfinite induction](../../../../../transfinite-induction.md). At zero, $0\leq\Phi(0)$ automatically. If $\alpha\leq\Phi(\alpha)$, strict increase at successors gives $\alpha+1\leq\Phi(\alpha)+1\leq\Phi(\alpha+1)$. At a nonzero limit $\lambda$, continuity and the induction hypotheses give

$$
\Phi(\lambda)=\sup_{\alpha<\lambda}\Phi(\alpha)\geq\sup_{\alpha<\lambda}\alpha=\lambda.
$$

Therefore $\boxed{\alpha\leq\Phi(\alpha)\text{ for every ordinal }\alpha}$. No [axiom of choice](../../../../../axiom-of-choice.md) is needed for this [ordinal](../../../../../ordinal-split.md) induction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
