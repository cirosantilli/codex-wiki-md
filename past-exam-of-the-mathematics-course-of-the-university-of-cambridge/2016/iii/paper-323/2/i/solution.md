<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) of the [Hermitian operator](../../../../../../hermitian-operator.md) $A$ and set $b_j=\langle\alpha_j|B|\alpha_j\rangle$. Since $B$ is a [positive contraction](../../../../../../positive-contraction.md),

$$
0\leq b_j\leq1,\qquad \sum_jb_j=r,\qquad \operatorname{Tr}(AB)=\sum_j\lambda_jb_j.
$$

For $0<r<d$, the missing weight among the first $r$ entries equals the weight in the remaining entries:

$$
t:=\sum_{j<r}(1-b_j)=\sum_{j\geq r}b_j.
$$

The ordered [eigenvalues](../../../../../../eigenvalue.md) satisfy $\lambda_j\geq\lambda_{r-1}$ for $j<r$ and $\lambda_j\leq\lambda_{r-1}$ for $j\geq r$. Therefore

$$
\sum_{j<r}\lambda_j-\operatorname{Tr}(AB)
=\sum_{j<r}\lambda_j(1-b_j)-\sum_{j\geq r}\lambda_jb_j
\geq\lambda_{r-1}t-\lambda_{r-1}t=0.
$$

This argument does not require the [eigenvalues](../../../../../../eigenvalue.md) of $A$ to be positive. For $r=0$, positivity and zero [trace](../../../../../../matrix-trace.md) give $B=0$; for $r=d$, the same argument applied to $I-B$ gives $B=I$. Thus **in every case**

$$
\boxed{\operatorname{Tr}(AB)\leq\sum_{j<r}\lambda_j.}
$$

The [orthogonal projection](../../../../../../orthogonal-projection.md) onto the leading $r$ [eigenvectors](../../../../../../eigenvector.md) attains equality. This is the [Hermitian effect variational principle](../../../../../../hermitian-effect-variational-principle.md), extending the [Ky Fan maximum principle](../../../../../../ky-fan-maximum-principle.md) to all [positive contractions](../../../../../../positive-contraction.md) with the prescribed [trace](../../../../../../matrix-trace.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
