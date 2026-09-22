<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For distinct coordinates $i,j$, let $E_{ij}(t)=I+t e_{ij}$, where $e_{ij}$ is the [matrix unit](../../../../../../matrix-unit.md). For $t\ne0$ this is a [transvection](../../../../../../transvection.md): it fixes the [hyperplane](../../../../../../hyperplane.md) with $j$th coordinate zero pointwise, has [determinant](../../../../../../determinant.md) one and inverse $E_{ij}(-t)$. We show these [elementary transvection matrices](../../../../../../elementary-transvection-matrix.md) generate $SL(n,F)$ over any [field](../../../../../../field.md).

Let $M\in SL(n,F)$. Row addition is left multiplication by an $E_{ij}(t)$. If the current diagonal pivot is zero, a nonzero entry occurs below it in the same remaining column, since the remaining square block is invertible; adding that row makes the pivot nonzero. Row additions then clear the entries below the pivot. Repeating produces an upper-triangular [matrix](../../../../../../matrix.md) with nonzero diagonal. Clearing the entries above the diagonal, starting from the last column, gives a [diagonal matrix](../../../../../../diagonal-matrix.md) $D=\operatorname{diag}(a_1,\ldots,a_n)$ with $\prod_i a_i=1$. Thus it remains to realize determinant-one [diagonal matrices](../../../../../../diagonal-matrix.md) using elementary [transvections](../../../../../../transvection.md).

In a two-coordinate block put

$$
w(a)=E_{12}(a)E_{21}(-a^{-1})E_{12}(a)
=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix}.
$$

Direct multiplication gives

$$
\boxed{w(a)w(-1)=\operatorname{diag}(a,a^{-1}).}
$$

The [diagonal matrix](../../../../../../diagonal-matrix.md) $D$ is the product, for $i=1,\ldots,n-1$, of these blocks on coordinates $i,n$, with entries $a_i,a_i^{-1}$. Their final $n$th entry is $\prod_{i<n}a_i^{-1}=a_n$. Therefore $D$, and hence $M$, is a product of elementary [transvections](../../../../../../transvection.md). All row operations used are invertible [transvections](../../../../../../transvection.md), and no division except by a nonzero pivot or $a_i$ has been made. This proves

$$
\boxed{SL(n,F)=\langle E_{ij}(t):i\ne j,\ t\in F\rangle.}
$$

The identity element $E_{ij}(0)$ can be omitted from the generating set. This is [transvections generate the special linear group](../../../../../../transvections-generate-the-special-linear-group.md); ordinary row scaling alone would not prove it, because such a scaling can leave $SL(n,F)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
