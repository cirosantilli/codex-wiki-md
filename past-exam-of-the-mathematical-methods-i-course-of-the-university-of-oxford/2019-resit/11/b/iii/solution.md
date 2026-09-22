<h1 id="11/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Expand the two [linear combinations](../../../../../linear-combination.md) and use the [Pauli matrix multiplication identity](../../../../../pauli-multiplication-identity.md):

$$
\begin{aligned}
\sigma(\mathbf a)\sigma(\mathbf b)
&=\sum_{ij}a_i b_j\left(\delta_{ij}I+i\sum_k\epsilon_{ijk}\sigma_k\right)\\
&=(\mathbf a\cdot\mathbf b)I+i\sigma(\mathbf a\times\mathbf b).
\end{aligned}
$$

Interchanging the [vectors](../../../../../vector.md) reverses the [cross product](../../../../../cross-product.md), so their [commutator](../../../../../commutator.md) is $2i\sigma(\mathbf a\times\mathbf b)$. The three [Pauli matrices](../../../../../pauli-matrices.md) are [linearly independent](../../../../../linear-independence.md); alternatively, [trace](../../../../../matrix-trace.md) against $\sigma_k$ to recover each coefficient. Thus

$$
\boxed{[\sigma(\mathbf a),\sigma(\mathbf b)]=0\quad\Longleftrightarrow\quad\mathbf a\times\mathbf b=0.}
$$

For nonzero real [vectors](../../../../../vector.md), this means they are parallel or antiparallel, equivalently [linearly dependent](../../../../../linear-dependence.md). The algebra also extends to complex [vectors](../../../../../vector.md) using bilinear dot and cross products, with the same linear-dependence criterion; the [dot product](../../../../../dot-product.md) there has no complex conjugation.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [11](../../../11.md)
4. [2019 resit](../../../../2019-resit-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
