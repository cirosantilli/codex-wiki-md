<h1 id="11/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Combine the diagonal and cyclic products from [b](../../b.md) into $\sigma_i\sigma_j=\delta_{ij}I+i\sum_k\epsilon_{ijk}\sigma_k$. Distribute the coefficients in the two Pauli-vector factors:

$$
\begin{aligned}
\sigma(\mathbf a)\sigma(\mathbf b)
&=\sum_{i,j}a_ib_j\sigma_i\sigma_j\\
&=\left(\sum_i a_ib_i\right)I
+i\sum_k\left(\sum_{i,j}\epsilon_{ijk}a_ib_j\right)\sigma_k.
\end{aligned}
$$

The inner sums are precisely the components of $\mathbf a\times\mathbf b$, so

$$
\boxed{\sigma(\mathbf a)\sigma(\mathbf b)
=(\mathbf a\cdot\mathbf b)I+i\sigma(\mathbf a\times\mathbf b).}
$$

Interchanging the two factors shows that their [commutator](../../../../../commutator.md) is $2i\sigma(\mathbf a\times\mathbf b)$. The three [Pauli matrices](../../../../../pauli-matrices.md) are linearly independent: the entries of $\sigma(\mathbf c)$ are $c_z,c_x-ic_y,c_x+ic_y,-c_z$, which vanish together only when $\mathbf c=0$. Thus

$$
\boxed{[\sigma(\mathbf a),\sigma(\mathbf b)]=0
\iff\mathbf a\times\mathbf b=0
\iff\mathbf a,\mathbf b\text{ are linearly dependent}.}
$$

For nonzero real [vectors](../../../../../vector.md), this means parallel or antiparallel directions. The dot and cross products here are bilinear; no complex conjugates are inserted if complex coefficients are considered.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [11](../../../11.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
