<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The [spectral norm](../../../../../../matrix-2-norm.md) is the induced Euclidean [operator norm](../../../../../../operator-norm.md)**:

$$
\boxed{\|A\|=\sup_{\|v\|_2=1}\|Av\|_2
=\sqrt{\lambda_{\max}(A^\dagger A)}.}
$$

It is the largest [singular value](../../../../../../singular-value.md). From the definition, multiplying on either side by a [unitary operator](../../../../../../unitary-operator.md) leaves the norm unchanged: right multiplication permutes the unit sphere of possible inputs, and left multiplication preserves output lengths. In particular every [unitary operator](../../../../../../unitary-operator.md) has norm one.

For [unitary product telescoping](../../../../../../unitary-product-telescoping.md), replace the factors one at a time. With empty products interpreted as the identity,

$$
U_m\cdots U_1-V_m\cdots V_1
=\sum_{j=1}^m U_m\cdots U_{j+1}(U_j-V_j)V_{j-1}\cdots V_1.
$$

All cross terms cancel. By the triangle inequality and unitary invariance of the [spectral norm](../../../../../../matrix-2-norm.md),

$$
\boxed{\|U_m\cdots U_1-V_m\cdots V_1\|
\leq\sum_{j=1}^m\|U_j-V_j\|<m\epsilon.}
$$

This bound is independent of the dimension and does not assume that any of the factors commute.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
