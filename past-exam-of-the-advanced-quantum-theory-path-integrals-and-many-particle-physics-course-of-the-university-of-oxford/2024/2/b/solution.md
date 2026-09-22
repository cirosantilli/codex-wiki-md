<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taking the [Hermitian adjoint](../../../../adjoint-operator.md) gives $\varphi_{\mathbf k}=c_k\psi_{\mathbf k}+s_k\psi_{-\mathbf k}^\dagger$. For nonzero [wavevectors](../../../../wavevector.md), the [canonical commutation relations](../../../../canonical-commutation-relation.md) imply

$$
\begin{aligned}
[\varphi_{\mathbf k},\varphi_{\mathbf q}^\dagger]
&=c_kc_q[\psi_{\mathbf k},\psi_{\mathbf q}^\dagger]
+s_ks_q[\psi_{-\mathbf k}^\dagger,\psi_{-\mathbf q}]\\
&=(c_kc_q-s_ks_q)\delta_{\mathbf k,\mathbf q}.
\end{aligned}
$$

When the [Kronecker delta](../../../../kronecker-delta.md) is nonzero, $k=q$, so the [hyperbolic Pythagorean identity](../../../../hyperbolic-pythagorean-identity.md) $c_k^2-s_k^2=1$ gives

$$
\boxed{[\varphi_{\mathbf k},\varphi_{\mathbf q}^\dagger]=\delta_{\mathbf k,\mathbf q}.}
$$

For the two [annihilation operators](../../../../annihilation-operator.md), the only potentially nonzero terms are

$$
\begin{aligned}
[\varphi_{\mathbf k},\varphi_{\mathbf q}]
&=c_ks_q[\psi_{\mathbf k},\psi_{-\mathbf q}^\dagger]
+s_kc_q[\psi_{-\mathbf k}^\dagger,\psi_{\mathbf q}]\\
&=(c_ks_q-s_kc_q)\delta_{\mathbf k,-\mathbf q}=0.
\end{aligned}
$$

Here $\mathbf q=-\mathbf k$ implies equal magnitudes and hence equal $c,s$, because $\theta_k$ depends only on $|\mathbf k|$. Thus

$$
\boxed{[\varphi_{\mathbf k},\varphi_{\mathbf q}]=0.}
$$

The corresponding [commutators](../../../../commutator.md) of two [creation operators](../../../../creation-operator.md) vanish by the [Hermitian adjoint](../../../../adjoint-operator.md). This verifies that the [Bogoliubov transformation](../../../../bogoliubov-transformation.md) preserves the full [bosonic](../../../../boson.md) [canonical commutation relations](../../../../canonical-commutation-relation.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
