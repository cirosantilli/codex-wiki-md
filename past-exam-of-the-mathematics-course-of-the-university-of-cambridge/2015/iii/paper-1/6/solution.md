<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For $a\in R$, write $m_a$ for multiplication by $a$ in $\operatorname{End}_k(R)$. The [algebraic differential operator ring](../../../../../algebraic-differential-operator-ring.md) is defined by the filtration

$$
D_k^{-1}(R)=0,\qquad
D_k^j(R)=\{\theta\in\operatorname{End}_k(R):
[\theta,m_a]\in D_k^{j-1}(R)\text{ for every }a\in R\},\qquad
D_k(R)=\bigcup_{j\geq0}D_k^j(R).
$$

The [order of an algebraic differential operator](../../../../../order-of-an-algebraic-differential-operator.md) is the least $j$ for which $\theta\in D_k^j(R)$; the zero operator may be assigned order $-\infty$. In degree zero, commuting with all multiplication maps means $\theta(a)=a\theta(1)$, so $D_k^0(R)=\{m_a:a\in R\}\cong R$. The [commutator](../../../../../commutator.md) identity $[UV,m_a]=U[V,m_a]+[U,m_a]V$ proves by induction that $D_k^rD_k^s\subseteq D_k^{r+s}$, so the union is a ring under addition and composition.

The [derivations of an algebra](../../../../../derivation-of-an-algebra.md) form

$$
\operatorname{Der}_k(R)=\{\delta:R\to R\text{ linear over }k:
\delta(ab)=a\delta(b)+b\delta(a)\}.
$$

Every such [derivation](../../../../../derivation-of-an-algebra.md) has $\delta(1)=0$ and $[\delta,m_a]=m_{\delta(a)}$, so has differential order at most one. Conversely, if $\theta\in D_k^1(R)$, set $c=\theta(1)$ and $\delta=\theta-m_c$. Then $\delta(1)=0$ and $[\delta,m_a]$ is a multiplication map. Evaluating at $1$ shows it is $m_{\delta(a)}$; evaluating at $b$ gives the [Leibniz rule](../../../../../leibniz-rule.md). **Hence the [first-order algebraic differential operator decomposition](../../../../../first-order-algebraic-differential-operator-decomposition.md) is**

$$
\boxed{D_k^1(R)=R+\operatorname{Der}_k(R).}
$$

It is a direct sum as $k$-[vector spaces](../../../../../vector-space-split.md): a multiplication map that is a [derivation](../../../../../derivation-of-an-algebra.md) vanishes at $1$, and is zero.

The complex [Weyl algebra](../../../../../weyl-algebra.md) has generators $x_1,\ldots,x_n,\partial_1,\ldots,\partial_n$ and relations

$$
\boxed{A_n=\mathbb C\langle x_i,\partial_i\rangle/
([x_i,x_j],\,[\partial_i,\partial_j],\,[\partial_i,x_j]-\delta_{ij}).}
$$

Take $n\geq1$. If a nonzero unital [module](../../../../../module-mathematics.md) $M$ had finite [dimension of a vector space](../../../../../dimension-vector-space.md) over $\mathbb C$ $m$, its representing matrices would satisfy $[\partial_1,x_1]=I_m$. Taking the [matrix trace](../../../../../matrix-trace.md) gives $0=m$, impossible in characteristic zero. **The [Weyl algebra has no nonzero finite-dimensional modules](../../../../../weyl-algebra-has-no-nonzero-finite-dimensional-modules.md).** For $n=0$ the algebra is $\mathbb C$ and this assertion has the obvious exception.

For a nonzero finitely generated [Weyl algebra](../../../../../weyl-algebra.md) [module](../../../../../module-mathematics.md), use the [Bernstein filtration](../../../../../bernstein-filtration.md)

$$
F_jA_n=\operatorname{span}_{\mathbb C}\{x^{\mathbf a}\partial^{\mathbf b}:|\mathbf a|+|\mathbf b|\leq j\}.
$$

The ordered [monomials](../../../../../monomial.md) form a [vector space basis](../../../../../basis.md), so

$$
\dim_{\mathbb C}F_jA_n=\binom{j+2n}{2n},\qquad
\operatorname{gr}_F A_n\cong\mathbb C[X_1,\ldots,X_n,\Xi_1,\ldots,\Xi_n].
$$

To justify the ordered basis, the relations move all $\partial_i$ to the right and give spanning. Independence follows in the action on $\mathbb C[x_1,\ldots,x_n]$: apply a putative zero operator $\sum_{\mathbf b}p_{\mathbf b}(x)\partial^{\mathbf b}$ coefficientwise to the formal exponential $e^{t\cdot x}$, obtaining $\sum_{\mathbf b}p_{\mathbf b}(x)t^{\mathbf b}=0$. Thus every coefficient vanishes.

Choose a finite-dimensional nonzero generating subspace $M_0\subseteq M$ and set $M_j=F_jA_n M_0$. The [associated graded module](../../../../../associated-graded-module.md) is finitely generated over the polynomial [associated graded ring](../../../../../associated-graded-ring.md), so the [Hilbert-Serre theorem](../../../../../hilbert-serre-theorem.md) implies $\dim_{\mathbb C}M_j$ is eventually a polynomial. Define

$$
\boxed{d(M)=\deg\bigl(\text{the eventual polynomial }\dim_{\mathbb C}M_j\bigr)
=\operatorname{GKdim}_{A_n}M.}
$$

This [Bernstein growth dimension of a Weyl algebra module](../../../../../bernstein-growth-dimension-of-a-weyl-algebra-module.md) equals the [Gelfand–Kirillov dimension of a module](../../../../../gelfand-kirillov-dimension-of-a-module.md), not its ordinary vector-space dimension. If a different finite generating subspace is used, each lies in some fixed filtration step of the other. The corresponding $M_j$ are sandwiched between shifted filtrations, so the degree is unchanged.

We prove [Bernstein inequality for Weyl algebra modules](../../../../../bernstein-inequality-for-weyl-algebra-modules.md) using an injectivity estimate. The [faithful finite-step action of a Weyl algebra](../../../../../faithful-finite-step-action-of-a-weyl-algebra.md) claim is that the map

$$
F_jA_n\longrightarrow\operatorname{Hom}_{\mathbb C}(M_j,M_{2j}),\qquad
a\longmapsto(v\mapsto av)
$$

is injective for every $j$. Induct on $j$. For $j=0$, a [scalar](../../../../../scalar.md) annihilating $M_0\ne0$ is zero. Suppose $a\in F_jA_n$ annihilates $M_j$. For any generator $z=x_i$ or $\partial_i$, the [commutator](../../../../../commutator.md) $[a,z]$ belongs to $F_{j-1}A_n$ and annihilates $M_{j-1}$: both $a(zv)$ and $z(av)$ vanish. The induction hypothesis gives $[a,z]=0$ for every generator. In the ordered basis,

$$
[a,x_i]=\sum_{\mathbf a,\mathbf b}b_i c_{\mathbf a,\mathbf b}
x^{\mathbf a}\partial^{\mathbf b-\mathbf e_i},\qquad
[a,\partial_i]=-\sum_{\mathbf a,\mathbf b}a_i c_{\mathbf a,\mathbf b}
x^{\mathbf a-\mathbf e_i}\partial^{\mathbf b}.
$$

In characteristic zero these identities force $a$ to be a [scalar](../../../../../scalar.md). Since it annihilates $M_0$, it is zero. This proves injectivity.

Consequently

$$
\binom{j+2n}{2n}\leq(\dim_{\mathbb C}M_j)(\dim_{\mathbb C}M_{2j}).
$$

The left side grows as a positive constant times $j^{2n}$; the right side has growth degree $2d(M)$. **Comparing powers proves**

$$
\boxed{d(M)\geq n.}
$$

The polynomial [module](../../../../../module-mathematics.md) $\mathbb C[x_1,\ldots,x_n]$, with the usual multiplication and differentiation actions, has $d(M)=n$, showing the bound is sharp.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
