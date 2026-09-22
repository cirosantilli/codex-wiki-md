<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [transfinite induction](../../../../../transfinite-induction.md) on nonzero $\alpha$. Part (b) gives $\alpha=\omega^\delta n+\zeta$, with $n$ a positive [natural number](../../../../../natural-number.md) and $\zeta<\omega^\delta\leq\alpha$.

If $\zeta=0$, this is already a one-term [Cantor normal form](../../../../../cantor-normal-form.md). Otherwise $0<\zeta<\alpha$, so the induction hypothesis supplies a finite [Cantor normal form](../../../../../cantor-normal-form.md) for $\zeta$. Its leading exponent $\eta$ satisfies $\omega^\eta\leq\zeta<\omega^\delta$, hence $\eta<\delta$. All later exponents are smaller still. Prefixing $\omega^\delta n$ therefore gives

$$
\boxed{\alpha=\omega^{\delta_0}n_0+\cdots+\omega^{\delta_{k-1}}n_{k-1},\qquad
\delta_0>\cdots>\delta_{k-1},\quad0<n_j<\omega.}
$$

The number of terms is finite because the inductive representation of the strictly smaller remainder is finite. Equivalently, repeated extraction cannot produce an infinite strictly descending sequence of [ordinals](../../../../../ordinal-split.md). Since $\alpha\ne0$, the number of terms is positive.

## ↑ Ancestors (13)

1. [C](../c.md)
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
