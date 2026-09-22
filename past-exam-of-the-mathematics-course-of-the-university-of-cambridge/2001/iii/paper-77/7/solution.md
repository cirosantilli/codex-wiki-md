<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

In the degree-completed symmetric-function algebra, the [Cauchy identity for symmetric functions](../../../../../cauchy-identity-for-symmetric-functions.md) is

$$
\boxed{\prod_{i,j}(1-x_iy_j)^{-1}
=\sum_{\lambda\in\operatorname{Par}}s_\lambda(x)s_\lambda(y).}
$$

It is a formal identity, so each homogeneous component is finite in the partition index; analytic convergence is not being assumed.

Expand each geometric factor and index the product by finite-support nonnegative [matrices](../../../../../matrix.md):

$$
\prod_{i,j}(1-x_iy_j)^{-1}
=\sum_A\prod_i x_i^{\sum_j a_{ij}}
\prod_j y_j^{\sum_i a_{ij}}.
$$

The [RSK correspondence](../../../../../robinson-schensted-knuth-correspondence.md) sends $A$ to a pair of [Semistandard Young tableaux](../../../../../semistandard-young-tableau.md) of equal shape. Its content identities turn the [matrix](../../../../../matrix.md) weight into the product of the recording tableau's $x$ weight and the insertion tableau's $y$ weight. Summing independently over both tableaux of each shape proves the identity.

Use the [Hall inner product of symmetric functions](../../../../../hall-inner-product-of-symmetric-functions.md), with $\langle p_\lambda,p_\mu\rangle=\delta_{\lambda\mu}z_\lambda$, as defined above. The left side is the reproducing kernel $\sum_\lambda p_\lambda(x)p_\lambda(y)/z_\lambda$. Pairing its Schur expansion in the $y$ alphabet with $s_\mu(y)$ gives

$$
s_\mu(x)=\sum_\lambda s_\lambda(x)\langle s_\lambda,s_\mu\rangle.
$$

The [Schur functions](../../../../../schur-polynomial.md) have already been proved to be a [basis](../../../../../basis.md), so uniqueness of this expansion gives

$$
\boxed{\langle s_\lambda,s_\mu\rangle=\delta_{\lambda\mu}.}
$$

This is orthonormality for the Hall product; it is not a claim about an unspecified coefficientwise [inner product](../../../../../inner-product.md).

The dual [determinant](../../../../../determinant.md) established in Question 2 gives $\omega(s_\lambda)=s_{\lambda'}$. Apply the [symmetric-function involution](../../../../../symmetric-function-involution.md) in the $y$ alphabet. Since $\omega(H_y(t))=E_y(t)$, it transforms each factor $H_y(x_i)$ into $E_y(x_i)$. The [dual Cauchy identity](../../../../../dual-cauchy-identity-for-symmetric-functions.md) is

$$
\boxed{\prod_{i,j}(1+x_iy_j)
=\sum_\lambda s_\lambda(x)s_{\lambda'}(y).}
$$

For arbitrary coefficients $f_r$ in a commutative ring, use the integral symmetric-function algebra and its free complete generators, specializing $h_r\mapsto f_r$. This works over any such coefficient ring; a literal homomorphism from the rational algebra $\Lambda$ also presupposes a $\mathbb Q$-algebra structure on the target. Specialize the first alphabet in the [Cauchy identity](../../../../../cauchy-identity-for-symmetric-functions.md) to obtain the [Schur specialization by a generating function](../../../../../schur-specialization-by-a-generating-function.md)

$$
\boxed{\prod_i F(t_i)=\sum_\lambda
\det[f_{\lambda_i-i+j}]\,s_\lambda(t)
=\sum_\lambda s_\lambda^F s_\lambda(t),}
$$

where $f_0=1$ and $f_r=0$ for $r<0$. Indeed, the left side is a product of the specialized $H(t_i)$, and the [Jacobi–Trudi identity](../../../../../jacobi-trudi-identity.md) specializes to the displayed [determinant](../../../../../determinant.md). For an arbitrary infinite $F$ the result lies in the degree completion; its coefficients in each degree are well defined.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
