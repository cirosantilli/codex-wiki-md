<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $L$ is an [invertible matrix](../../../../../invertible-matrix.md), $Av=0$ is equivalent to $Uv=0$. The last nontrivial row gives $v_3=v_4$; the second gives $v_2=v_4$; and the first gives $2v_1=v_2+v_4$, so $v_1=v_4$. A [basis](../../../../../basis.md) of the [null space](../../../../../kernel-of-a-linear-map-split.md) is therefore

$$
\boxed{\mathcal B_{\ker A}=\{(1,1,1,1)^T\}.}
$$

Its single [basis vector](../../../../../basis-vector.md) has [Euclidean norm](../../../../../euclidean-norm.md) $2$, so the unit [null space](../../../../../kernel-of-a-linear-map-split.md) [basis vector](../../../../../basis-vector.md) is $(1,1,1,1)^T/2$.

The [pivot elements](../../../../../pivot-element.md) of $U$ lie in columns $1,2,3$. Take these columns from the **original** [matrix](../../../../../matrix.md) $A$ to obtain a [basis](../../../../../basis.md) of its [column space](../../../../../column-space.md):

$$
\boxed{\mathcal B_{\operatorname{Col} A}=
\left\{\begin{pmatrix}-2\\2\\0\\0\end{pmatrix},
\begin{pmatrix}1\\-2\\1\\0\end{pmatrix},
\begin{pmatrix}0\\0\\-2\\2\end{pmatrix}\right\}.}
$$

The fourth column is minus the sum of these three columns, and the leading three-by-three [matrix minor](../../../../../minor-linear-algebra.md) has nonzero [determinant](../../../../../determinant.md) $-4$, confirming [linear independence](../../../../../linear-independence.md).

[Elementary row operations](../../../../../elementary-row-operation.md) preserve the [row space](../../../../../row-space.md). Thus the nonzero rows of $U$ give a [basis](../../../../../basis.md) of the [row space](../../../../../row-space.md) of $A$:

$$
\boxed{\mathcal B_{\operatorname{Row} A}=
\{(-2,1,0,1),\ (0,-1,0,1),\ (0,0,-2,2)\}.}
$$

These [basis vectors](../../../../../basis-vector.md) need not have unit [Euclidean norm](../../../../../euclidean-norm.md) or be [orthogonal](../../../../../orthogonal-vectors.md). Their [Euclidean norms](../../../../../euclidean-norm.md) are $\sqrt6,\sqrt2,2\sqrt2$, respectively; the three column [basis vectors](../../../../../basis-vector.md) have [Euclidean norms](../../../../../euclidean-norm.md) $2\sqrt2,\sqrt6,2\sqrt2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
