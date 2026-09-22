<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

For the reality of the [eigenvalues](../../../../../eigenvalue.md), one may initially allow a nonzero complex [eigenvector](../../../../../eigenvector.md) $\mathbf v$ with $M\mathbf v=\lambda\mathbf v$. Since $M$ is real symmetric, it is a [Hermitian matrix](../../../../../hermitian-operator.md), and

$$
\lambda=\frac{\mathbf v^\dagger M\mathbf v}{\mathbf v^\dagger\mathbf v}
$$

is real: the numerator equals its own complex conjugate and the denominator is positive. Once $\lambda$ is real, a nonzero real or imaginary part of $\mathbf v$ supplies a real eigenvector. We work with the real unit eigenvectors of the problem.

For two such [eigenvectors](../../../../../eigenvector.md), symmetry gives

$$
\lambda_a\,\mathbf e_a\cdot\mathbf e_b
=(M\mathbf e_a)\cdot\mathbf e_b
=\mathbf e_a\cdot(M\mathbf e_b)
=\lambda_b\,\mathbf e_a\cdot\mathbf e_b.
$$

Distinct [eigenvalues](../../../../../eigenvalue.md) therefore give zero [dot product](../../../../../dot-product.md). Together with the prescribed unit lengths,

$$
\boxed{\mathbf e_a\cdot\mathbf e_b=\delta_{ab}.}
$$

These $n$ vectors form an [orthonormal basis](../../../../../orthonormal-basis.md) of $\mathbb R^n$.

Expand a real [unit vector](../../../../../unit-vector.md) as $\mathbf x=\sum_ac_a\mathbf e_a$. Then $\sum_ac_a^2=1$, and its [Rayleigh quotient](../../../../../rayleigh-quotient.md) is

$$
\mathbf x^TM\mathbf x=\sum_a\lambda_ac_a^2\le\lambda_1.
$$

Moreover,

$$
\lambda_1-\mathbf x^TM\mathbf x
=\sum_{a=2}^n(\lambda_1-\lambda_a)c_a^2.
$$

Every coefficient on the right is strictly positive, so equality forces $c_a=0$ for $a\ge2$. **Equality occurs precisely along the top eigendirection**:

$$
\boxed{\mathbf x^TM\mathbf x\le\lambda_1,\qquad
\mathbf x^TM\mathbf x=\lambda_1\iff\mathbf x=\pm\mathbf e_1.}
$$

To obtain a unit vector in $S$ using just $\mathbf e_1,\mathbf e_2$, let $u=(\mathbf e_1)_1$ and $v=(\mathbf e_2)_1$ denote their first coordinates. If $u^2+v^2>0$, take

$$
\alpha_1=\frac v{\sqrt{u^2+v^2}},\qquad
\alpha_2=-\frac u{\sqrt{u^2+v^2}}.
$$

Then $\alpha_1u+\alpha_2v=0$ and $\alpha_1^2+\alpha_2^2=1$. Hence $\alpha_1\mathbf e_1+\alpha_2\mathbf e_2$ has first coordinate zero and unit length. If $u=v=0$, simply take $\alpha_1=1,\alpha_2=0$. In either case the [Rayleigh quotient](../../../../../rayleigh-quotient.md) of the constructed vector is

$$
\lambda_1\alpha_1^2+\lambda_2\alpha_2^2\ge\lambda_2.
$$

The continuous quadratic form attains its maximum on the [compact space](../../../../../compact-space.md) $S$, so

$$
\max_{\mathbf x\in S}\mathbf x^TM\mathbf x\ge\lambda_2.
$$

For $\mathbf x=(0,\mathbf y)^T$, deletion of the first row and column gives $\mathbf x^TM\mathbf x=\mathbf y^TA\mathbf y$, while $|\mathbf x|=|\mathbf y|$. The [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) applied to $A$ identifies its largest [eigenvalue](../../../../../eigenvalue.md) with this maximum:

$$
\mu=\max_{|\mathbf y|=1}\mathbf y^TA\mathbf y
=\max_{\mathbf x\in S}\mathbf x^TM\mathbf x.
$$

Combining the upper bound for every unit vector with the constructed lower bound proves

$$
\boxed{\lambda_1\ge\mu\ge\lambda_2.}
$$

This is [largest-eigenvalue interlacing for a principal submatrix](../../../../../largest-eigenvalue-interlacing-for-a-principal-submatrix.md): restricting a quadratic form to a coordinate hyperplane cannot exceed its old maximum, but leaves some direction in the span of the top two eigenvectors.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
