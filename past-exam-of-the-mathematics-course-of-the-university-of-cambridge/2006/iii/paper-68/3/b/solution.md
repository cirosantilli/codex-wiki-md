<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md), which follows by substituting the [bilateral shift operator](../../../../../../bilateral-shift-operator.md) $e^{h\partial_t}$ into the exact-solution residual. Direct expansion gives

$$
\rho(e^z)-z\sigma(e^z)
=-\frac{\alpha+5}{12}z^4-\frac{14\alpha+61}{90}z^5+O(z^6).
$$

All coefficients through degree three vanish. If $\alpha\ne-5$, the fourth-degree coefficient is nonzero, so the normalized [local truncation error](../../../../../../local-truncation-error.md) has exact order three. At $\alpha=-5$, the fourth-degree coefficient vanishes and the fifth-degree coefficient is $1/10$, which is nonzero. Thus

$$
\boxed{p=3\text{ if }\alpha\ne-5,\qquad p=4\text{ if }\alpha=-5.}
$$

This is the formal order of the full recurrence. The order-four member is not [zero-stable](../../../../../../zero-stability.md), so it is not convergent. All the convergent members from part (a) have order three. At the degenerate value $\alpha=1$, the full recurrence still has formal order three, while cancellation of its common factor gives [Backward Euler method](../../../../../../backward-euler-method.md) of order one; that cancellation changes the method rather than its order calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
