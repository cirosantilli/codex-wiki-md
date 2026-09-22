<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

Split the [vector](../../../../../vector.md) $x$ into its normal and tangential [orthogonal projections](../../../../../orthogonal-projection.md):

$$
x=(n\cdot x)n+\bigl(x-(n\cdot x)n\bigr).
$$

A [reflection](../../../../../reflection-mathematics.md) in the plane negates the first component and preserves the second. Thus $Hx=x-2(n\cdot x)n$, giving the [Householder reflection](../../../../../householder-transformation.md)

$$
\boxed{M=I-2nn^T,\qquad M_{ij}=\delta_{ij}-2n_in_j.}
$$

Since $n\cdot n=1$ and $n\cdot u=n\cdot v=0$,

$$
\boxed{Mn=-n,\qquad Mu=u,\qquad Mv=v.}
$$

The columns of a [matrix representation of a linear map](../../../../../matrix-representation-of-a-linear-map.md) are the coordinates of the images of the ordered basis [vectors](../../../../../vector.md). Consequently, in the [orthonormal basis](../../../../../orthonormal-basis.md) $(u,v,n)$,

$$
\boxed{N=\begin{pmatrix}1&0&0\\0&1&0\\0&0&-1\end{pmatrix}.}
$$

Equivalently, with the [orthogonal matrix](../../../../../orthogonal-matrix.md) $Q=(u\ v\ n)$, the [change of basis](../../../../../change-of-basis.md) formula is $N=Q^TMQ$.

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
