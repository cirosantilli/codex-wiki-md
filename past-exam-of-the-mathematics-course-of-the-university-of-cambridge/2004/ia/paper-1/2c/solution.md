<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

Write $A=\sum_i a_i^2$, $B=\sum_i b_i^2$, $C=\sum_i a_ib_i$. If $B=0$, every $b_i=0$ and the claimed inequality is immediate. Otherwise the sum of squares

$$
0\leq\sum_i(a_i-tb_i)^2=A-2tC+t^2B
$$

holds for every real $t$. Choosing $t=C/B$ gives $0\leq A-C^2/B$, and hence the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in its stronger absolute-value form:

$$
\boxed{|C|\leq\sqrt{AB}.}
$$

In particular $C\leq\sqrt A\sqrt B$, as requested. For unit [vectors](../../../../../vector.md), $A=B=1$, so this same argument gives

$$
\boxed{|a\cdot b|\leq1.}
$$

The absolute value is essential for opposite-pointing [vectors](../../../../../vector.md); it follows from the squared inequality without a sign assumption on their [dot product](../../../../../dot-product.md).

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
