<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $e(\omega)$ denote [exterior multiplication](../../../../../../exterior-multiplication.md), $e(\omega)\alpha=\omega\wedge\alpha$. For a $q$-form $\alpha$, evaluation of the proposed operator on [vector fields](../../../../../../vector-field.md) $Y_0,\ldots,Y_q$ gives

$$
\left(\sum_i\omega_i\wedge\nabla_{X_i}\alpha\right)(Y_0,\ldots,Y_q)
=\sum_{a=0}^q(-1)^a(\nabla_{Y_a}\alpha)(Y_0,\ldots,\widehat Y_a,\ldots,Y_q),
$$

since $\sum_i\omega_i(Y_a)X_i=Y_a$. This expression is independent of the chosen local [basis](../../../../../../basis.md).

Expand each [covariant derivative](../../../../../../covariant-derivative.md) into the derivative of $\alpha(Y_0,\ldots,\widehat Y_a,\ldots,Y_q)$ minus the terms obtained by differentiating each argument. For every pair $a<b$, those argument terms combine into

$$
(-1)^{a+b}\alpha(\nabla_{Y_a}Y_b-\nabla_{Y_b}Y_a,
Y_0,\ldots,\widehat Y_a,\ldots,\widehat Y_b,\ldots,Y_q).
$$

The [Levi-Civita connection](../../../../../../levi-civita-connection.md) is a [torsion-free connection](../../../../../../torsion-free-connection.md), so the vector in this expression is $[Y_a,Y_b]$. The result is exactly the defining evaluation formula for the [exterior derivative](../../../../../../exterior-derivative.md):

$$
(d\alpha)(Y_0,\ldots,Y_q)
=\sum_a(-1)^aY_a\bigl(\alpha(Y_0,\ldots,\widehat Y_a,\ldots,Y_q)\bigr)
+\sum_{a<b}(-1)^{a+b}\alpha([Y_a,Y_b],Y_0,\ldots,\widehat Y_a,\ldots,\widehat Y_b,\ldots,Y_q).
$$

Therefore $\boxed{d=\sum_i e(\omega_i)\nabla_{X_i}}$. No orthonormality or compactness is needed for this identity; the dual-frame property and vanishing [torsion tensor](../../../../../../torsion-tensor.md) suffice.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
