<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the supplied [weight decomposition](../../../../weight-decomposition.md) $V=\bigoplus_{\lambda\in\Psi(\mathfrak a)}V_\lambda$. There is a small distinction to justify: the definition of a [toral subalgebra](../../../../toral-subalgebra.md) uses the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md), while these [weight spaces](../../../../weight-space.md) use the [defining representation](../../../../defining-representation-of-a-matrix-lie-algebra.md). For the [symplectic Lie algebra](../../../../symplectic-lie-algebra.md), [adjoint semisimplicity in the symplectic Lie algebra](../../../../adjoint-semisimplicity-in-the-symplectic-lie-algebra.md) implies that each $a\in\mathfrak a$ is [diagonalizable](../../../../diagonalizable-matrix.md) on $V$ as well. Here is a direct verification.

Define the [symplectic adjoint](../../../../symplectic-adjoint.md) $a^*$ by $\omega(av,w)=\omega(v,a^*w)$. The [symplectic Lie algebra](../../../../symplectic-lie-algebra.md) condition is $a^*=-a$. Write the [Jordan–Chevalley decomposition](../../../../jordan-chevalley-decomposition.md) in $\operatorname{End}(V)$ as $a=S+N$, with $S$ [diagonalizable](../../../../diagonalizable-matrix.md), $N$ a [nilpotent linear map](../../../../nilpotent-linear-map.md), and $SN=NS$. Uniqueness of the [Jordan–Chevalley decomposition](../../../../jordan-chevalley-decomposition.md), applied to $a^*=-a$, gives $S^*=-S$ and $N^*=-N$. Thus $S,N\in\mathfrak{sp}(V)$. On $\operatorname{End}(V)$, $\operatorname{ad}S$ is [diagonalizable](../../../../diagonalizable-matrix.md) by using a [matrix unit](../../../../matrix-unit.md) [basis](../../../../basis.md) in an [eigenbasis](../../../../eigenbasis.md) of $S$, and $\operatorname{ad}N$ is a [nilpotent linear map](../../../../nilpotent-linear-map.md), since

$$
(\operatorname{ad}N)^m(T)=\sum_{j=0}^m(-1)^j\binom mjN^{m-j}TN^j
$$

vanishes for large $m$. These operators commute and preserve $\mathfrak{sp}(V)$, so their restrictions are the [Jordan–Chevalley decomposition](../../../../jordan-chevalley-decomposition.md) of $\operatorname{ad}a$. Because $\operatorname{ad}a$ is [diagonalizable](../../../../diagonalizable-matrix.md), its nilpotent part is zero: $\operatorname{ad}N=0$ on $\mathfrak{sp}(V)$.

To conclude that $N=0$ without an assumption on the [center of a Lie algebra](../../../../center-of-a-lie-algebra.md), observe that each map $T_v(w)=\omega(v,w)v$ lies in $\mathfrak{sp}(V)$. If $v\ne0$, its image is $kv$, because $\omega$ is a [nondegenerate bilinear form](../../../../nondegenerate-bilinear-form.md). Since $N$ commutes with $T_v$, it preserves $kv$. Hence $Nv\in kv$ for every $v$, forcing $N$ to be a scalar [linear map](../../../../linear-map.md): compare its action on two [linearly independent](../../../../linear-independence.md) vectors and their sum. A scalar [nilpotent linear map](../../../../nilpotent-linear-map.md) is zero. For $V=0$ the assertion is immediate. This proves the needed [diagonalizability](../../../../diagonalizable-matrix.md). Commuting [diagonalizable](../../../../diagonalizable-matrix.md) [linear maps](../../../../linear-map.md) admit [simultaneous diagonalization](../../../../simultaneous-diagonalization.md), giving the displayed [weight decomposition](../../../../weight-decomposition.md).

Now let $v\in V_\lambda$ and $w\in V_\mu$. For every $a\in\mathfrak a$, preservation of the [alternating bilinear form](../../../../alternating-bilinear-form.md) gives

$$
0=\omega(av,w)+\omega(v,aw)=(\lambda(a)+\mu(a))\omega(v,w).
$$

If $\lambda+\mu\ne0$ as a [linear functional](../../../../linear-functional.md), choose $a$ on which it is nonzero; then $\omega(v,w)=0$. Therefore

$$
\boxed{\omega(V_\lambda,V_\mu)=0\quad\text{unless }\mu=-\lambda.}
$$

For $v\ne0$ in $V_\lambda$, the fact that $\omega$ is a [nondegenerate bilinear form](../../../../nondegenerate-bilinear-form.md) supplies a $w\in V$ with $\omega(v,w)\ne0$. Decomposing $w$ into [weight spaces](../../../../weight-space.md), only its $V_{-\lambda}$ component can contribute. Thus $V_{-\lambda}\ne0$, and $\Psi(\mathfrak a)=-\Psi(\mathfrak a)$. The same argument on both sides shows that $\omega:V_\lambda\times V_{-\lambda}\to k$ is a [perfect pairing](../../../../perfect-pairing.md), so $\dim V_\lambda=\dim V_{-\lambda}$. On $V_0$, the restriction of $\omega$ is a [nondegenerate bilinear form](../../../../nondegenerate-bilinear-form.md) that is an [alternating bilinear form](../../../../alternating-bilinear-form.md), so $\dim V_0$ is even.

Choose one representative $\lambda_i$ from each pair of nonzero [weights of a representation](../../../../weight-of-a-representation.md), for $1\leq i\leq r$. Here

$$
r=\frac{|\Psi(\mathfrak a)\setminus\{0\}|}{2}.
$$

The [linear map](../../../../linear-map.md) $\mathfrak a\to k^r$ sending $a$ to $(\lambda_1(a),\ldots,\lambda_r(a))$ is injective: an element in its [kernel](../../../../kernel-of-a-linear-map-split.md) acts by zero on every nonzero [weight space](../../../../weight-space.md), and also on $V_0$, so it is the zero element of $\mathfrak a\subseteq\operatorname{End}(V)$. Taking [dimensions](../../../../dimension-vector-space.md) yields

$$
\boxed{\dim\mathfrak a\leq r=\frac{|\Psi(\mathfrak a)\setminus\{0\}|}{2}\leq n.}
$$

The final inequality follows because each pair contributes at least two to $\dim V=2n$. Equivalently, the nonzero [weights of a representation](../../../../weight-of-a-representation.md) span the [dual space](../../../../dual-space-split.md) $\mathfrak a^*$; they need not be [linearly independent](../../../../linear-independence.md) at this stage.

## ↑ Ancestors (12)

1. [B](../b.md)
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
