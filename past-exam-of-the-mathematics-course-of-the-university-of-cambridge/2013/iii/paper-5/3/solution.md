<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [Young tableau](../../../../../young-tableau.md) $t$, let $R_t$ permute the entries within its rows and $C_t$ within its columns. We use the [Young symmetrizer](../../../../../young-symmetrizer.md) convention

$$
r_t=\sum_{\sigma\in R_t}\sigma,\qquad c_t=\sum_{\tau\in C_t}\operatorname{sgn}(\tau)\tau,\qquad h_t=c_tr_t.
$$

Reversing the order gives another usual realization of the same irreducible [polynomial](../../../../../polynomial-split.md) [module](../../../../../module-mathematics.md). On the [tensor power](../../../../../tensor-power.md) $T=V^{\otimes n}$, the actions are

$$
\sigma(v_1\otimes\cdots\otimes v_n)=v_{\sigma^{-1}(1)}\otimes\cdots\otimes v_{\sigma^{-1}(n)},\qquad
g(v_1\otimes\cdots\otimes v_n)=gv_1\otimes\cdots\otimes gv_n.
$$

They commute because applying $g$ to every factor commutes with permuting the factors.

We state the permitted combinatorial input explicitly. A [Young symmetrizer](../../../../../young-symmetrizer.md) satisfies $h_t^2=H_\lambda h_t$, where $H_\lambda$ is the nonzero [hook product of a partition](../../../../../hook-product-of-a-partition.md). Thus $e_t=H_\lambda^{-1}h_t$ is a primitive [idempotent](../../../../../idempotent.md). The standard-tableau decomposition of the right regular [module](../../../../../module-mathematics.md) is $\mathbb CS_n=\bigoplus_{\lambda,t\ \mathrm{standard}}e_t\mathbb CS_n$. Tensor this right-module direct sum with the left [module](../../../../../module-mathematics.md) $T$. The map $e_t\mathbb CS_n\otimes_{\mathbb CS_n}T\to e_tT$ sending $e_ta\otimes v$ to $e_tav$ is an isomorphism, with inverse $w\mapsto e_t\otimes w$. Therefore the [Young-symmetrizer tensor decomposition](../../../../../young-symmetrizer-tensor-decomposition.md) is

$$
T=\bigoplus_{\lambda,t\ \mathrm{standard}}e_tT=\bigoplus_{\lambda,t\ \mathrm{standard}}h_tT.
$$

This is a direct sum of $GL(V)$-modules; individual summands need not be $S_n$-invariant.

We also state the allowed [Schur algebra](../../../../../schur-algebra.md) result, namely [Schur–Weyl duality](../../../../../schur-weyl-duality.md): the two actions are mutual [commutants](../../../../../centralizer.md), and

$$
T\cong\bigoplus_{\lambda\vdash n,\ \ell(\lambda)\le m}S^\lambda\otimes D_\lambda(V),
$$

where the $D_\lambda(V)$ are pairwise nonisomorphic irreducible homogeneous [polynomial representations](../../../../../polynomial-representation-of-the-general-linear-group.md) of degree $n$. We also use the standard [Schur algebra](../../../../../schur-algebra.md) equivalence between its modules and homogeneous degree-$n$ [polynomial representations](../../../../../polynomial-representation-of-the-general-linear-group.md), so these exhaust the irreducibles in that category. A primitive [idempotent](../../../../../idempotent.md) $e_t$ has one-dimensional image on $S^\lambda$ and zero image on the other simple factors, so $h_tT\cong D_\lambda(V)$. This identifies the requested irreducibles. They classify the [polynomial](../../../../../polynomial-split.md) degree-$n$ representations in this [tensor power](../../../../../tensor-power.md), not all [rational representations](../../../../../rational-representation.md) of every degree.

The [length bound for a Schur module](../../../../../length-bound-for-a-schur-module.md) is **$D_\lambda(V)\ne0$ if and only if $\ell(\lambda)\le m$**. A column of length greater than $m$ antisymmetrizes more than $m$ vectors and gives zero. Conversely, for $\ell(\lambda)\le m$, fill every tensor position in row $i$ with the $i$th [basis](../../../../../basis.md) vector of $V$. Row symmetrization multiplies it by $\prod_i\lambda_i!$, and column antisymmetrization is nonzero because the vectors within each column are distinct [basis](../../../../../basis.md) vectors.

A [rational representation of an algebraic group](../../../../../rational-representation.md) is a regular morphism into the general linear group of its representation space. For $GL_m$, its matrix entries belong to $\mathbb C[g_{ij},\det(g)^{-1}]$; rational here permits [determinant](../../../../../determinant.md) denominators but not arbitrary poles on $GL_m$. A one-dimensional rational [character](../../../../../character-of-a-representation.md) of $\mathbb C^\times$ is a [Laurent polynomial](../../../../../laurent-polynomial.md) $p(z)$ with $p(zw)=p(z)p(w)$ and $p(1)=1$. Comparing Laurent coefficients shows that just one monomial occurs and its coefficient is $1$, hence $p(z)=z^r$ for $r\in\mathbb Z$.

Restrict a one-dimensional rational [character](../../../../../character-of-a-representation.md) of $GL_m$ to its diagonal torus. The same argument in several variables gives $\prod_i x_i^{r_i}$. Conjugation by permutation matrices makes all $r_i$ equal. On every [diagonalizable](../../../../../diagonalizable-matrix.md) invertible matrix it consequently agrees with $(\det g)^r$. The allowed Zariski-density statement, and equality of [regular functions](../../../../../regular-function.md) on a dense subset, give

$$
\boxed{\chi(g)=(\det g)^r,\qquad r\in\mathbb Z.}
$$

These are the [one-dimensional rational characters of the general linear group](../../../../../one-dimensional-rational-characters-of-the-general-linear-group.md).

For [complete reducibility of rational GL and SL representations](../../../../../complete-reducibility-of-rational-gl-and-sl-representations.md), use the compact-group averaging argument. Average any positive definite Hermitian [inner product](../../../../../inner-product.md) over $SU(m)$ using normalized [Haar measure](../../../../../haar-measure.md). The [orthogonal complement](../../../../../orthogonal-complement.md) of an invariant subspace is then $SU(m)$-invariant. Differentiating makes it invariant under $\mathfrak{su}(m)$ and therefore under its complex span $\mathfrak{sl}_m(\mathbb C)$. The elementary unipotent matrices $\exp(tE_{ij})$ generate $SL_m(\mathbb C)$, so the complement is $SL_m$-invariant. This proves complete reducibility. Averaging over $U(m)$ similarly gives complete reducibility for rational $GL_m$ representations.

Here is an explicit [rational extension from SL to GL](../../../../../rational-extension-from-sl-to-gl.md). Decompose the representation space by the finite scalar center of $SL_m$ into subspaces $W_k$ on which $\zeta I$ acts as $\zeta^k$, with $0\le k<m$ and $\zeta^m=1$. These subspaces are invariant. For $g\in GL_m$, choose $a$ with $a^m=\det g$, set $s=a^{-1}g\in SL_m$, and define

$$
\rho'(g)|_{W_k}=a^k\rho(s)|_{W_k}.
$$

Changing $a$ to $\zeta a$ changes $s$ to $\zeta^{-1}s$, so the two factors cancel. It is a homomorphism, since scalar roots multiply up to the same harmless factor, and it restricts to $\rho$ on $SL_m$.

It is rational as well. Every matrix coefficient of $\rho|_{W_k}$ has a [polynomial](../../../../../polynomial-split.md) representative on $SL_m$. Averaging that representative over the finite scalar center selects its homogeneous parts $P_d$ with $d\equiv k\pmod m$. Substitution in the extension gives $\sum_d(\det g)^{(k-d)/m}P_d(g)$, a [regular function](../../../../../regular-function.md) on $GL_m$. Each $SL_m$-invariant subspace decomposes into its $W_k$ parts, and the extension acts on each part by a scalar times an $SL_m$ action. Thus these subspaces are also invariant under the chosen extension. Consequently **$\rho$ is irreducible if and only if this $\rho'$ is irreducible**. For $m=1$, $SL_1$ is trivial and the trivial extension supplies the same conclusion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
