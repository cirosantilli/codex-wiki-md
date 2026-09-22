<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

For $\mathbf b\ne0$, define the [orthogonal projection](../../../../../orthogonal-projection.md) of $\mathbf a$ onto its span by

$$
\mathbf a_{\parallel}=\frac{\mathbf a\cdot\mathbf b}{|\mathbf b|^2}\mathbf b,\qquad \mathbf a_{\perp}=\mathbf a-\mathbf a_{\parallel}.
$$

The first is parallel or antiparallel to $\mathbf b$, or zero, and $\mathbf a_\perp\cdot\mathbf b=0$. This proves the decomposition. If $\mathbf a\ne0$ as well, comparison with $\mathbf a_\parallel=|\mathbf a|\cos\theta\,\widehat{\mathbf b}$ yields

$$
\boxed{\cos\theta=\frac{\mathbf a\cdot\mathbf b}{|\mathbf a||\mathbf b|}.}
$$

Indeed $|\mathbf a|^2=|\mathbf a_\parallel|^2+|\mathbf a_\perp|^2$ shows that the ratio lies in $[-1,1]$. There is a unique $\theta\in[0,\pi]$ with this cosine. The definition is symmetric in the two [vectors](../../../../../vector.md), unchanged by orthogonal coordinate changes and positive rescaling, and agrees with ordinary plane geometry in their span: projecting a unit vector onto the other gives its cosine. Parallel, perpendicular and antiparallel directions give $0,\pi/2,\pi$ respectively. The zero vector has no defined angle; if $\mathbf b=0$, the nonzero-axis projection formula itself must not be used.

The vertices of the centered [hypercube](../../../../../hypercube.md) are sign vectors $\mathbf u\in\{-1,1\}^n$. A body diagonal identifies $\mathbf u$ and $-\mathbf u$, hence there are $2^{n-1}$ such diagonals. If two sign vectors disagree in $h$ positions, their [dot product](../../../../../dot-product.md) is $n-h-h=n-2h$. For odd $n$ this integer is odd and cannot be zero. Thus **no two body diagonals are perpendicular in odd dimension**, by the [orthogonality of hypercube body diagonals](../../../../../orthogonality-of-hypercube-body-diagonals.md).

In four dimensions, mutually [orthogonal](../../../../../orthogonal-vectors.md) nonzero [vectors](../../../../../vector.md) are linearly independent, so at most four mutually perpendicular diagonals are possible. Four are achieved by the directions

$$
\boxed{(1,1,1,1),\quad(1,-1,1,-1),\quad(1,1,-1,-1),\quad(1,-1,-1,1).}
$$

Each has squared norm four and every distinct pair has zero [dot product](../../../../../dot-product.md); these are the rows of a [Hadamard matrix](../../../../../hadamard-matrix.md). Therefore **the maximum is four**.

For distinct diagonals, the [Hamming distance](../../../../../hamming-distance.md) is $h=1,2,3$; $h=0,4$ would represent the same line. Oriented vertex directions therefore give cosines $1/2,0,-1/2$. The angles are

$$
\boxed{\pi/3,\ \pi/2,\ 2\pi/3\quad\text{for oriented directions}.}
$$

For unoriented diagonals, the usual smaller angle between the lines is **$\pi/3$ or $\pi/2$**; the supplementary intersection angle $2\pi/3$ also occurs when the two rays are chosen oppositely. Stating this convention avoids counting a line and its reverse as different diagonals.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
