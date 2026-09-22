<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the regular real [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), with $p,w>0$, ordered [eigenvalues](../../../../../eigenvalue.md) $\lambda_0<\lambda_1<\cdots$, and real orthonormal [eigenfunctions](../../../../../eigenfunction.md) in the [weighted inner product](../../../../../weighted-inner-product.md)

$$
\langle u,v\rangle_w=\int_0^1uv\,w\,dx.
$$

The [Rayleigh quotient](../../../../../rayleigh-quotient.md) for an admissible trial [function](../../../../../function-split.md) is

$$
R[\widetilde y]=\frac{\int_0^1\widetilde y\mathcal L\widetilde y\,dx}{\int_0^1w\widetilde y^2\,dx}=\frac{\int_0^1[p(\widetilde y')^2+q\widetilde y^2]\,dx}{\int_0^1w\widetilde y^2\,dx}.
$$

The second expression follows by [integration by parts](../../../../../integration-by-parts.md). It is the quantity used in the [Rayleigh-Ritz method](../../../../../rayleigh-ritz-method.md).

For $\widetilde y=y_0+\sum_{n\geq1}a_ny_n$, orthonormality eliminates every cross-term in the denominator:

$$
\int_0^1w\widetilde y^2\,dx=1+\sum_{n\geq1}a_n^2.
$$

Applying $\mathcal L$ to the [eigenfunction expansion](../../../../../eigenfunction-expansion.md) and using the same [orthogonality](../../../../../orthogonal-vectors.md) in the numerator gives

$$
\int_0^1\widetilde y\mathcal L\widetilde y\,dx=\lambda_0+\sum_{n\geq1}a_n^2\lambda_n.
$$

Hence, whenever the trial [function](../../../../../function-split.md) has finite energy,

$$
\boxed{\widetilde\lambda_0=R[\widetilde y]=\frac{\lambda_0+\sum_{n\geq1}a_n^2\lambda_n}{1+\sum_{n\geq1}a_n^2}.}
$$

Put $S=\sum a_n^2$ and $\Delta=\sum a_n^2(\lambda_n-\lambda_0)$. The exact error and its expansion are

$$
\boxed{\widetilde\lambda_0-\lambda_0=\frac\Delta{1+S}=\Delta+O(S\Delta).}
$$

In particular, under a common small scaling $a_n=\varepsilon b_n$ with fixed finite sums $\sum b_n^2$ and $\sum b_n^2(\lambda_n-\lambda_0)$,

$$
\boxed{\widetilde\lambda_0=\lambda_0+\sum_{n\geq1}a_n^2(\lambda_n-\lambda_0)+O(\varepsilon^4).}
$$

The fourth-order remainder includes mixed products $a_n^2a_j^2$, not just individual fourth powers.

**Error comparison and sign.** Since $\|y_0\|_w=1$, the relative [weighted norm](../../../../../weighted-norm.md) error of the supplied trial [function](../../../../../function-split.md) is

$$
\frac{\|\widetilde y-y_0\|_w}{\|y_0\|_w}=\sqrt{S}=O(\varepsilon).
$$

For $\lambda_0\ne0$, the relative [eigenvalue](../../../../../eigenvalue.md) error is $\Delta/(|\lambda_0|(1+S))=O(\varepsilon^2)$. Thus the [Rayleigh quotient](../../../../../rayleigh-quotient.md) has a second-order error for a first-order error in the trial [eigenfunction](../../../../../eigenfunction.md), provided the energy-weighted coefficient sum is controlled. Small weighted norm error alone does not control arbitrarily high-frequency contamination, because $\lambda_n$ can grow without bound. If $\lambda_0=0$, an absolute error must replace the undefined relative one.

Finally every summand of $\Delta$ is nonnegative. Thus

$$
\boxed{\widetilde\lambda_0\geq\lambda_0,}
$$

with strict inequality whenever some $a_n\ne0$. This is the upper-bound property of the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) for the lowest [eigenvalue](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
