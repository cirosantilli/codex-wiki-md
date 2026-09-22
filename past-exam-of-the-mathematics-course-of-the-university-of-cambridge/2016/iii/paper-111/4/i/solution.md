<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $c>0$, the necessary parameter range for the bounds involving $1/c$. The construction comes from the [singular value decomposition](../../../../../../singular-value-decomposition.md) of [matrix Fourier blocks](../../../../../../matrix-fourier-block.md). For each inequivalent [unitary irreducible representation](../../../../../../unitary-irreducible-representation.md) $\rho$ of [dimension](../../../../../../dimension-vector-space.md) $d_\rho$, consider the [Hilbert space](../../../../../../hilbert-space-split.md) $\mathcal H_\rho=M_{n\times d_\rho}(\mathbb C)$ with the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) $\langle A,B\rangle=\operatorname{tr}(A^*B)$ and the operator

$$
T_\rho(A)=\mathbb E_x f(x)A\rho(x)^*.
$$

Its [operator norm](../../../../../../operator-norm.md) is at most one, since $\rho(x)$ is a [unitary matrix](../../../../../../unitary-matrix.md) and $\|f(x)\|_{\mathrm{op}}\leq1$. Thus all its [singular values](../../../../../../singular-value.md) $\lambda_{\rho,j}$ lie in $[0,1]$.

Two identities control their weighted moments:

$$
S_2=\sum_\rho d_\rho\sum_j\lambda_{\rho,j}^2
=\mathbb E_x\operatorname{tr}(f(x)f(x)^*)\leq n,
$$



$$
S_4=\sum_\rho d_\rho\sum_j\lambda_{\rho,j}^4
=\mathbb E_{xy^{-1}zw^{-1}=e}\operatorname{tr}(f(x)f(y)^*f(z)f(w)^*)\geq cn.
$$

Here the [expectation](../../../../../../expected-value.md) in $S_4$ is uniform on the $|G|^3$ solutions of the constraint, and the [trace](../../../../../../matrix-trace.md) on $\mathcal H_\rho$ used to compute each moment is the ordinary operator [trace](../../../../../../matrix-trace.md). We justify the identities explicitly to fix their normalizations and the noncommutative order.

The [adjoint operator](../../../../../../adjoint-operator.md) is $T_\rho^*(A)=\mathbb E_yf(y)^*A\rho(y)$, so

$$
T_\rho T_\rho^*(A)
=\mathbb E_{x,y}f(x)f(y)^*A\rho(yx^{-1}).
$$

For rectangular matrices, the operator $A\mapsto LAR$ has [trace](../../../../../../matrix-trace.md) $\operatorname{tr}(L)\operatorname{tr}(R)$, as is seen on the matrix-unit [basis](../../../../../../basis.md). Squaring the previous operator therefore gives

$$
\begin{aligned}
\operatorname{Tr}_{\mathcal H_\rho}(T_\rho T_\rho^*)&=\mathbb E_{x,y}\operatorname{tr}(f(x)f(y)^*)\chi_\rho(yx^{-1}),\\
\operatorname{Tr}_{\mathcal H_\rho}((T_\rho T_\rho^*)^2)&=\mathbb E_{x,y,z,w}\operatorname{tr}(f(x)f(y)^*f(z)f(w)^*)\chi_\rho(wz^{-1}yx^{-1}).
\end{aligned}
$$

The required [representation theory](../../../../../../representation-theory-split.md) consists of [unitarization of a finite-group representation](../../../../../../unitarization-of-a-finite-group-representation.md), the [Schur orthogonality relations](../../../../../../schur-orthogonality-relations.md), and the [regular representation](../../../../../../regular-representation.md) decomposition. The last gives the [character expansion of the identity delta](../../../../../../character-expansion-of-the-identity-delta.md)

$$
\sum_\rho d_\rho\chi_\rho(g)=|G|1_{\{g=e\}}.
$$

Summing the two operator [traces](../../../../../../matrix-trace.md) with weights $d_\rho$ selects $x=y$ in the first, and $w=xy^{-1}z$ in the second. Multiplication by $|G|$ converts each independent-variable [expectation](../../../../../../expected-value.md) to its conditional [expectation](../../../../../../expected-value.md). This proves $S_2,S_4$. In particular $S_4$ is real and nonnegative, despite the apparently complex summands in its original formula. Since $S_4\leq S_2\leq n$, the nonvacuous hypothesis has $0<c\leq1$.

Select every [singular value](../../../../../../singular-value.md) satisfying $\lambda_{\rho,j}\geq\sqrt{c/2}$. Index the selected pairs by $p=1,\ldots,r$, set $\rho_p=\rho$, $n_p=d_\rho$, and choose unit [right singular vectors](../../../../../../right-singular-vector.md) $A_p$ and unit [left singular vectors](../../../../../../left-singular-vector.md) $B_p$ with $T_{\rho_p}A_p=\lambda_pB_p$. Define

$$
\boxed{U(p)=\sqrt{n_p}A_p,\qquad V(p)=\sqrt{n_p}B_p.}
$$

Both are $n\times n_p$ matrices, proving (i). Repeated [group representations](../../../../../../group-representation.md) in this list are literally the same chosen representative, rather than different equivalent realizations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
