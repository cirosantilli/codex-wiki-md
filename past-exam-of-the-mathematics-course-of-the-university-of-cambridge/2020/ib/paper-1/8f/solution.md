<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

The [rank of a matrix](../../../../../matrix-rank.md) is the [dimension](../../../../../dimension-vector-space.md) of its [column space](../../../../../column-space.md), equivalently the dimension of the [image of a linear map](../../../../../image-of-a-linear-map.md) represented by the matrix. For $A\in\mathcal M_n$, the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives

$$
\operatorname{rank}A=n
\iff \ker A=\{0\}
\iff A\text{ is injective}.
$$

An injective endomorphism of a finite-dimensional [vector space](../../../../../vector-space-split.md) is [surjective](../../../../../surjective-function.md), hence [invertible](../../../../../invertible-matrix.md). By the [adjugate matrix](../../../../../adjugate-matrix.md) identity

$$
A\operatorname{adj}A=(\det A)I,
$$

$A$ is invertible when $\det A\ne0$; conversely, [multiplicativity of the determinant](../../../../../multiplicativity-of-the-determinant.md) shows that an invertible $A$ has nonzero [determinant](../../../../../determinant.md). Therefore

$$
\boxed{\operatorname{rank}A=n\iff A\text{ is nonsingular}\iff\det A\ne0}.
$$

Let $E_{ij}$ be the [matrix unit](../../../../../matrix-unit.md) with its only nonzero entry at $(i,j)$. The following $n^2$ matrices are all nonsingular:

$$
\mathcal B=\{I\}\cup\{I+E_{ij}:(i,j)\ne(n,n)\}.
$$

Indeed, $I+E_{ij}$ is an elementary shear when $i\ne j$, while $I+E_{ii}$ is diagonal with one diagonal entry equal to two. Their [linear span](../../../../../linear-span.md) contains every $E_{ij}$ except initially $E_{nn}$, because $E_{ij}=(I+E_{ij})-I$, and it then contains

$$
E_{nn}=I-\sum_{i=1}^{n-1}E_{ii}.
$$

Thus $\mathcal B$ spans the $n^2$-dimensional space $\mathcal M_n$ and, having $n^2$ members, is a [basis](../../../../../basis.md). This also covers $n=1$, when $\mathcal B=\{I\}$.

Now let $A$ be a nonsingular [zero-one matrix](../../../../../binary-matrix.md). If it had fewer than $n-1$ zero entries, at least two rows would contain no zero at all. Those two rows would both be the all-one row, contradicting [linear independence](../../../../../linear-independence.md). Hence every such matrix has at most

$$
\boxed{c_n\le n^2-n+1}
$$

ones. The bound is attained. Let $J$ be the all-one matrix and set

$$
A=J-\operatorname{diag}(1,\ldots,1,0),
$$

where there are $n-1$ initial diagonal ones. If $A\mathbf x=0$ and $S=\sum_jx_j$, the first $n-1$ row equations give $x_i=S$, while the last gives $S=0$. Hence every $x_i=0$, so $A$ is nonsingular and has exactly $n^2-n+1$ ones. Therefore

$$
\boxed{c_n=n^2-n+1}.
$$

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
