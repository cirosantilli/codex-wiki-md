<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each of the four standard pairs, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\langle W,KW\rangle=A\int_0^L|W''|^2\,dx\geq0.
$$

Consequently the [eigenvalues](../../../../../../eigenvalue.md) are nonnegative. For a positive [eigenvalue](../../../../../../eigenvalue.md) $\mu_n=A k_n^4$, the [eigenvalue equation](../../../../../../eigenvalue-equation.md) is $W_n''''=k_n^4W_n$. Its four characteristic roots are $\pm k_n,\pm i k_n$, so

$$
\boxed{W_n(x)=C_1\cos(k_nx)+C_2\sin(k_nx)+C_3\cosh(k_nx)+C_4\sinh(k_nx).}
$$

Here $C_j$ are coefficients, avoiding a collision with the [filament bending modulus](../../../../../../filament-bending-modulus.md) $A$. The regular finite-interval [self-adjoint operator](../../../../../../self-adjoint-operator.md) has [compact resolvent](../../../../../../compact-resolvent.md); applying the [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) to a shifted inverse supplies a complete [orthonormal basis](../../../../../../orthonormal-basis.md) of [eigenfunctions](../../../../../../eigenfunction.md).

For [clamped boundary conditions](../../../../../../clamped-boundary-condition.md) at zero, a [clamped--clamped bending mode](../../../../../../clamped-clamped-bending-mode.md) can be written

$$
W=C(\cosh kx-\cos kx)+D(\sinh kx-\sin kx).
$$

At $L$, writing $\beta=kL$, the two remaining [boundary conditions](../../../../../../boundary-condition.md) are

$$
\begin{pmatrix}\cosh\beta-\cos\beta&\sinh\beta-\sin\beta\\
\sinh\beta+\sin\beta&\cosh\beta-\cos\beta\end{pmatrix}
\binom CD=0.
$$

The [determinant](../../../../../../determinant.md) is $2(1-\cos\beta\cosh\beta)$. Hence **the positive [wavenumbers](../../../../../../wavenumber.md) obey**

$$
\boxed{\cos\beta_n\cosh\beta_n=1,\qquad k_n=\beta_n/L.}
$$

Equivalently, intersect $\cos\beta$ with $\operatorname{sech}\beta$. Numerical root bracketing gives

$$
\beta_1\simeq4.730041,\quad\beta_2\simeq7.853205,\quad\beta_3\simeq10.995608,\quad\beta_4\simeq14.137165,\quad\beta_5\simeq17.278760.
$$

The entire sequence has the useful large-$n$ description

$$
\boxed{\beta_n=(n+\tfrac12)\pi+2(-1)^{n+1}e^{-(n+1/2)\pi}+O(e^{-2(n+1/2)\pi}),\qquad n=1,2,\ldots.}
$$

Indeed, put $\beta=(n+\tfrac12)\pi+\delta$ in $\cos\beta=\operatorname{sech}\beta$ and use $\cos\beta=(-1)^{n+1}\delta+O(\delta^3)$ and $\operatorname{sech}\beta=2e^{-\beta}+O(e^{-3\beta})$.

The apparent root $\beta=0$ in the [determinant](../../../../../../determinant.md) equation is spurious for the clamped problem: at zero [eigenvalue](../../../../../../eigenvalue.md), $W$ is a cubic polynomial, and its four clamped conditions force $W=0$. For other endpoint choices, [zero-energy filament modes](../../../../../../zero-energy-filament-mode.md) must be treated separately from the trigonometric formula. The free-free [kernel](../../../../../../kernel-of-a-linear-map.md) consists of affine functions, the torqued-torqued [kernel](../../../../../../kernel-of-a-linear-map.md) consists of constants, and the hinged-hinged [kernel](../../../../../../kernel-of-a-linear-map.md) is trivial. Including those [kernels](../../../../../../kernel-of-a-linear-map.md) is necessary for a complete [eigenfunction expansion](../../../../../../eigenfunction-expansion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
