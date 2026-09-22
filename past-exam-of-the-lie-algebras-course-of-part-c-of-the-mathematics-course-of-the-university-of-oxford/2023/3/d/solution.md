<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the standard structural fact that $\mathfrak{sp}(V)$ is a [semisimple Lie algebra](../../../../semisimple-lie-algebra-split.md) over an [algebraically closed field](../../../../algebraically-closed-field.md) of [characteristic zero](../../../../characteristic-zero.md). If $\mathfrak h$ is a [Cartan subalgebra](../../../../cartan-subalgebra.md), part (a)(ii) gives $C_{\mathfrak{sp}(V)}(\mathfrak h)=\mathfrak h$, and $\mathfrak h$ is an [abelian Lie algebra](../../../../abelian-lie-algebra.md). Part (c) therefore shows that its [weight spaces](../../../../weight-space.md) occur as $n$ pairs of one-dimensional spaces, with no zero [weight space](../../../../weight-space.md).

Choose representatives $\lambda_1,\ldots,\lambda_n$ of its nonzero [weights of a representation](../../../../weight-of-a-representation.md). Pick $p_i\ne0$ in $V_{\lambda_i}$ and $q_i\ne0$ in $V_{-\lambda_i}$, scaling $q_i$ so that $\omega(p_i,q_i)=1$. Part (b) shows that all other pairings among different pairs are zero. Each individual [weight space](../../../../weight-space.md) is one-dimensional and the [bilinear form](../../../../bilinear-form-split.md) is alternating, so the ordered [basis](../../../../basis.md)

$$
\mathcal B=(p_1,\ldots,p_n,q_1,\ldots,q_n)
$$

is a [symplectic basis](../../../../symplectic-basis.md). Every $h\in\mathfrak h$ is a [diagonal matrix](../../../../diagonal-matrix.md) in this [basis](../../../../basis.md), with entries $\lambda_1(h),\ldots,\lambda_n(h),-\lambda_1(h),\ldots,-\lambda_n(h)$.

Let $D_{\mathcal B}$ be the [Lie subalgebra](../../../../lie-subalgebra.md) consisting of all [diagonal matrices](../../../../diagonal-matrix.md)

$$
D_{\mathcal B}=\{\operatorname{diag}(t_1,\ldots,t_n,-t_1,\ldots,-t_n):t_i\in k\}.
$$

Each such [matrix](../../../../matrix.md) lies in the [symplectic Lie algebra](../../../../symplectic-lie-algebra.md) and commutes with $\mathfrak h$. Hence

$$
\mathfrak h\subseteq D_{\mathcal B}\subseteq C_{\mathfrak{sp}(V)}(\mathfrak h)=\mathfrak h,
$$

and $\mathfrak h=D_{\mathcal B}$. In particular, every [Cartan subalgebra](../../../../cartan-subalgebra.md) has [dimension](../../../../dimension-vector-space.md) $n$; the $\lambda_i$ are a [basis](../../../../basis.md) of $\mathfrak h^*$.

Carry out the same construction for $\mathfrak h'$, obtaining a [symplectic basis](../../../../symplectic-basis.md) $\mathcal B'=(p'_1,\ldots,p'_n,q'_1,\ldots,q'_n)$ with $\mathfrak h'=D_{\mathcal B'}$. The unique [linear map](../../../../linear-map.md) $g$ sending $p_i$ to $p'_i$ and $q_i$ to $q'_i$ is invertible and preserves all pairings of [basis vectors](../../../../basis-vector.md). By [bilinearity](../../../../bilinearity.md), it preserves $\omega$ on all of $V$, so $g$ belongs to the [symplectic group](../../../../symplectic-group.md) $\operatorname{Sp}(V)$. The [change of basis](../../../../change-of-basis.md) gives

$$
\boxed{g\mathfrak h g^{-1}=gD_{\mathcal B}g^{-1}=D_{\mathcal B'}=\mathfrak h',\qquad g\in\operatorname{Sp}(V).}
$$

Thus [conjugacy of Cartan subalgebras of the symplectic Lie algebra](../../../../conjugacy-of-cartan-subalgebras-of-the-symplectic-lie-algebra.md) follows by explicitly matching their [symplectic bases](../../../../symplectic-basis.md). If $n=0$, the [Lie algebra](../../../../lie-algebra-split.md) is zero and the same conclusion holds with $g$ the identity on the zero [vector space](../../../../vector-space-split.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the lie algebras course of Part C of the mathematics course of the University of Oxford](../../../split.md)
5. [Lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
