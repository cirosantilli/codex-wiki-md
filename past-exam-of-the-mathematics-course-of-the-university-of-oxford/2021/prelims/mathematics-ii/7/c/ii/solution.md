<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $a<b$, choose the uniform [partition of an interval](../../../../../../../partition-of-an-interval.md) into $n$ pieces and its midpoint tags

$$
\xi_i=a+\left(i-\frac12\right)\frac{b-a}{n},\qquad1\leq i\leq n.
$$

Their [arithmetic mean](../../../../../../../arithmetic-mean.md) is exactly $(a+b)/2$. Apply the given [Jensen inequality](../../../../../../../jensen-s-inequality.md) with equal weights $\lambda_i=1/n$:

$$
\frac1n\sum_{i=1}^n f(\xi_i)\leq f\left(\frac1n\sum_{i=1}^n\xi_i\right)=f\left(\frac{a+b}2\right).
$$

Multiplying by $b-a$ gives a midpoint [Riemann sum](../../../../../../../riemann-sum.md) on the left. Its [mesh of a partition](../../../../../../../mesh-of-a-partition.md) is $(b-a)/n\to0$, so the [Riemann sum convergence theorem](../../../../../../../riemann-sum-convergence-theorem.md) gives

$$
\boxed{\int_a^b f(x)\,dx\leq(b-a)f\left(\frac{a+b}2\right).}
$$

For $a=b$ the equality is immediate. Together with part [i](../i.md), this is the [Hermite-Hadamard inequality](../../../../../../../hermite-hadamard-inequality.md) with the directions appropriate to a [concave function](../../../../../../../concave-function.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
