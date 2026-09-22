<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $i\ne j$, put $x_{ij}(a)=I+aE_{ij}$. When $a\ne0$ this is a [transvection](../../../../../../transvection.md): it fixes the [hyperplane](../../../../../../hyperplane.md) $v_j=0$ pointwise and has rank-one difference from the identity. Its inverse is $x_{ij}(-a)$ and its [determinant](../../../../../../determinant.md) is one.

Left multiplication performs a row addition. For an invertible [matrix](../../../../../../matrix.md), bring a nonzero entry into a pivot position by a signed interchange, then clear its column by row additions. A signed interchange on two coordinates is itself a product of row additions, because

$$
w(a)=x_{12}(a)x_{21}(-a^{-1})x_{12}(a)
=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix}\qquad(a\ne0).
$$

Repeating the pivot construction and then clearing above the pivots reduces any determinant-one [matrix](../../../../../../matrix.md) to a diagonal [matrix](../../../../../../matrix.md) of [determinant](../../../../../../determinant.md) one. Finally

$$
w(a)w(-1)=\operatorname{diag}(a,a^{-1}).
$$

A determinant-one diagonal [matrix](../../../../../../matrix.md) is a product of such two-coordinate matrices, using the last coordinate to compensate each of the first $n-1$ diagonal entries. Each displayed [matrix](../../../../../../matrix.md) is a product of [elementary transvection matrices](../../../../../../elementary-transvection-matrix.md). Hence reversing the elimination proves

$$
\boxed{SL_n(F)=\langle x_{ij}(a):i\ne j,\ a\in F\rangle.}
$$

This argument works over every [field](../../../../../../field.md), including [characteristic](../../../../../../characteristic-of-a-field.md) two.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
