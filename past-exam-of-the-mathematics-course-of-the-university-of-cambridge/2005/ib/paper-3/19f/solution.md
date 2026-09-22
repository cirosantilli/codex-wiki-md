<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

Split $A=D+L+U$ with $D=\mu^{-1}I$, $L$ the negative unit subdiagonal and $U$ the positive unit superdiagonal. The [Jacobi method](../../../../../jacobi-method.md) uses $x^{(r+1)}=-D^{-1}(L+U)x^{(r)}+D^{-1}b$, so

$$
\boxed{T_J=\begin{pmatrix}0&-\mu&0&0\\\mu&0&-\mu&0\\0&\mu&0&-\mu\\0&0&\mu&0\end{pmatrix}}.
$$

The [Gauss-Seidel method](../../../../../gauss-seidel-method.md) uses $(D+L)x^{(r+1)}=b-Ux^{(r)}$, giving by forward substitution

$$
\boxed{T_{GS}=\begin{pmatrix}0&-\mu&0&0\\0&-\mu^2&-\mu&0\\0&-\mu^3&-\mu^2&-\mu\\0&-\mu^4&-\mu^3&-\mu^2\end{pmatrix}}.
$$

Both iterations converge for every initial error exactly when their [spectral radius](../../../../../spectral-radius.md) is below one, since the error evolves as powers of the iteration matrix.

For Jacobi, the leading tridiagonal determinant recurrence is $p_j(\lambda)=\lambda p_{j-1}(\lambda)+\mu^2p_{j-2}(\lambda)$, with $p_0=1,p_1=\lambda$. Thus

$$
p_4=\lambda^4+3\mu^2\lambda^2+\mu^4.
$$

Its roots are $\lambda=\pm i\mu\sqrt{(3+\sqrt5)/2}$ and $\pm i\mu\sqrt{(3-\sqrt5)/2}$. Expanding the Gauss-Seidel determinant gives

$$
\det(\lambda I-T_{GS})=\lambda^2(\lambda^2+3\mu^2\lambda+\mu^4),
$$

so its nonzero eigenvalues are $-\mu^2(3\pm\sqrt5)/2$. Therefore

$$
\rho(T_J)=\frac{1+\sqrt5}{2}|\mu|,\qquad\rho(T_{GS})=\frac{3+\sqrt5}{2}\mu^2=\rho(T_J)^2.
$$

The [skew-tridiagonal Jacobi and Gauss-Seidel iterations](../../../../../skew-tridiagonal-jacobi-and-gauss-seidel-iterations.md) consequently have the same convergence range:

$$
\boxed{0<|\mu|<\frac{\sqrt5-1}{2}}.
$$

Equality fails the every-start convergence condition, and larger magnitudes have unstable modes. The nonsymmetric matrix does not permit an unexamined positive-definite-matrix convergence argument.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
