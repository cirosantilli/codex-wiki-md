<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

If $e_1,\ldots,e_n$ are [orthonormal](../../../../../orthonormal-set.md), any relation $\sum_i c_ie_i=0$ gives $c_j=0$ on taking the [dot product](../../../../../dot-product.md) with $e_j$. Thus the vectors are [linearly independent](../../../../../linear-independence.md). A linearly independent set of $n$ vectors in the $n$-dimensional [vector space](../../../../../vector-space-split.md) $\mathbb R^n$ is a [basis](../../../../../basis.md), proving the claim.

Expand both $x$ and $f$ in this [orthonormal basis](../../../../../orthonormal-basis.md), writing $f_i=e_i\cdot f$. Since $Ae_i=\lambda_ie_i$, the linear equation becomes

$$
\sum_i(\lambda_i-\mu)a_ie_i=\sum_if_ie_i.
$$

Comparing the unique [basis](../../../../../basis.md) coefficients gives, when $\mu$ is not an [eigenvalue](../../../../../eigenvalue.md),

$$
\boxed{a_i=\frac{e_i\cdot f}{\lambda_i-\mu},\qquad
x=\sum_i\frac{e_i\cdot f}{\lambda_i-\mu}e_i.}
$$

If $\mu=\lambda_1$, the equation is solvable exactly when $e_i\cdot f=0$ for every $i$ with $\lambda_i=\mu$. For those indices $a_i$ is arbitrary; for all other indices the displayed formula still applies. Thus repeated [eigenvalues](../../../../../eigenvalue.md) require orthogonality to the entire corresponding [eigenspace](../../../../../eigenspace.md), not merely to one chosen [eigenvector](../../../../../eigenvector.md). This is the finite-dimensional [Fredholm solvability condition for a self-adjoint operator](../../../../../fredholm-solvability-condition-for-a-self-adjoint-operator.md).

For the specific real [symmetric matrix](../../../../../symmetric-matrix.md), choose

$$
e_1=\frac1{\sqrt2}(1,-1,0),\quad\lambda_1=1;\qquad
e_2=\frac1{\sqrt2}(1,1,0),\quad\lambda_2=3;\qquad
e_3=(0,0,1),\quad\lambda_3=3.
$$

Their [dot products](../../../../../dot-product.md) with $f$ are $-1/\sqrt2$, $3/\sqrt2$ and $3$. At $\mu=2$ this gives

$$
\boxed{a_1=1/\sqrt2,\quad a_2=3/\sqrt2,\quad a_3=3,\qquad x=(2,1,3).}
$$

One can check $(A-2I)x=f$ directly. At $\mu=1$, the first coefficient equation would require $0\cdot a_1=-1/\sqrt2$, which is impossible. Hence **there is no solution when $\mu=1$**; the nonzero projection onto its [eigenspace](../../../../../eigenspace.md) is the obstruction.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
