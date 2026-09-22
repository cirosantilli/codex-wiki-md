<h1 id="6/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For a nonnegative integer-valued [random variable](../../../../../../../random-variable-split.md) $W$, the [tail-sum formula](../../../../../../../tail-sum-formula.md) states $\mathbb E[W]=\sum_{k=1}^\infty\mathbb P(W\geq k)$. It follows by writing $W=\sum_{k\geq1}\mathbf1_{\{W\geq k\}}$ and using nonnegativity to interchange sum and [expectation](../../../../../../../expected-value-split.md).

With $W=\lfloor X\rfloor$, this gives

$$
\boxed{\mathbb E[\lfloor X\rfloor]=\sum_{k=1}^\infty k^{1-t}=\zeta(t-1).}
$$

The [Riemann zeta function](../../../../../../../riemann-zeta-function.md) is finite here because $t-1>1$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
