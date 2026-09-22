<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

First $N(A)$ is finite: by [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md), $\|Ax\|_2\le(\sum_{ij}a_{ij}^2)^{1/2}\|x\|_2$. It is nonnegative and absolutely homogeneous. If $N(A)=0$, every $Ae_j=0$, so every column is zero and $A=0$; the converse is immediate. The triangle inequality for the [Euclidean norm](../../../../../euclidean-norm.md) gives $N(A+B)\le N(A)+N(B)$ after taking suprema. Thus **$N$ is a [norm](../../../../../norm.md)**.

For any vector $x$, rescaling gives $\|Ax\|_2\le N(A)\|x\|_2$. Applying this twice gives

$$
\boxed{N(AB)\le N(A)N(B).}
$$

Furthermore $|a_{ij}|\le\|Ae_j\|_2\le N(A)$, proving the requested strict entry bound when $N(A)<\varepsilon$.

For a [polynomial](../../../../../polynomial-split.md) in [matrix](../../../../../matrix.md) entries, expand each monomial at $A+H$. The terms involving exactly one entry of $H$ give a [linear map](../../../../../linear-map.md) $Df(A)[H]$, with [coefficients](../../../../../coefficient.md) [polynomial](../../../../../polynomial-split.md) in the entries of $A$. Every remaining term has at least two entries of $H$ and is $O(N(H)^2)$ for $N(H)\le1$, because $|h_{ij}|\le N(H)$. This proves differentiability. Its [derivative](../../../../../derivative.md) is continuous as an operator-valued function: each [coefficient](../../../../../coefficient.md) is continuous, and for $N(H)\le1$ every $h_{ij}$ is bounded by one, so the operator-[norm](../../../../../norm.md) difference is bounded by the sum of the [coefficient](../../../../../coefficient.md) differences. Coordinate [continuity](../../../../../continuous-function.md) follows from the same entry bound. Hence **every such [polynomial](../../../../../polynomial-split.md) function is continuously differentiable**.

In the Leibniz expansion of $\det(I+H)$, the identity permutation supplies $1+\sum_i h_{ii}$ plus terms of degree at least two. Any nonidentity permutation moves at least two indices, so each of its terms has at least two $H$ entries. Consequently

$$
\det(I+H)=1+\operatorname{tr}H+O(N(H)^2),\qquad
\boxed{d'(I)[H]=\operatorname{tr}H.}
$$

If $A$ is invertible, multiplicativity of the [determinant](../../../../../determinant.md) and the preceding expansion give

$$
\det(A+H)=\det A\det(I+A^{-1}H)
=\det A+\det A\operatorname{tr}(A^{-1}H)+O(N(H)^2).
$$

The adjugate identity gives $\operatorname{adj}A=\det(A)A^{-1}$. Thus $d'(A)[H]=\operatorname{tr}((\operatorname{adj}A)H)$ for invertible $A$.

For singular $A$, take invertible $A_r\to A$, using the permitted density result. Both $d'$ and the adjugate entries are continuous [polynomial](../../../../../polynomial-split.md) expressions, so taking limits for every fixed $H$ proves the [derivative of the determinant](../../../../../derivative-of-the-determinant.md) formula on all [matrices](../../../../../matrix.md):

$$
\boxed{d'(A)[H]=\operatorname{tr}((\operatorname{adj}A)H).}
$$

Here the standard adjugate is the transpose of the cofactor array, as required by $(\operatorname{adj}A)A=(\det A)I$. In components this [derivative](../../../../../derivative.md) is $\sum_{ij}\operatorname{cof}_{ij}(A)h_{ij}$, also valid at singular [matrices](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
