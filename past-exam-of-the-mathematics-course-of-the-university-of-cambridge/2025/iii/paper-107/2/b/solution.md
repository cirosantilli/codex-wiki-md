<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [p-energy](../../../../../../p-energy.md)

$$
F[u]=\frac1p\int_\Omega|Du|^p\,dx,
$$

the [first variation](../../../../../../first-variation.md) in the direction $\psi\in C_c^\infty(\Omega)$ is

$$
\left.\frac d{dt}F[u+t\psi]\right|_{t=0}
=\int_\Omega|Du|^{p-2}Du\mathbin\cdot D\psi.
$$

An [integration by parts](../../../../../../integration-by-parts.md) therefore gives the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md)

$$
\operatorname{div}(|Du|^{p-2}Du)=0,
$$

which is the [p-Laplacian equation](../../../../../../p-laplacian.md). In the notation of the question one takes $a^{ij}(x,z,\eta)=|\eta|^{p-2}\delta^{ij}$.

For $\eta\ne0$, the principal coefficient matrix is

$$
A^{ik}(\eta)=|\eta|^{p-2}\delta^{ik}
+(p-2)|\eta|^{p-4}\eta_i\eta_k.
$$

Its eigenvalue in directions orthogonal to $\eta$ is $|\eta|^{p-2}$, while its eigenvalue parallel to $\eta$ is $(p-1)|\eta|^{p-2}$. The coefficients are $C^{1,\alpha}$ away from $\eta=0$, and the [condition number](../../../../../../condition-number.md) there is at most $p-1$. On every region where $0<m\leq|Du|\leq M$, this gives uniform ellipticity with constants depending on $m$, $M$, and $p$. At $Du=0$ all principal eigenvalues vanish, so the operator is degenerate there and is not strictly elliptic on a domain containing a critical point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
