<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We give the full local-field norm-index argument. Let $G=\langle\sigma\rangle$ be cyclic of order $n$. On an additive $G$-[module](../../../../../module-mathematics.md) set $D=\sigma-1$ and $N=1+\sigma+\cdots+\sigma^{n-1}$. The two cyclic [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) [groups](../../../../../group-split.md) are

$$
\widehat H^0(G,M)=M^G/NM,\qquad\widehat H^{-1}(G,M)=\ker N/DM.
$$

When these are finite, the [Herbrand quotient](../../../../../herbrand-quotient.md) is $h_G(M)=|\widehat H^0(G,M)|/|\widehat H^{-1}(G,M)|$. The periodic complex alternating $D$ and $N$ yields a six-term periodic exact sequence from a short exact sequence of [modules](../../../../../module-mathematics.md). Taking alternating products of orders in that exact sequence proves

$$
h_G(M)=h_G(M')h_G(M'')\qquad(0\to M'\to M\to M''\to0).
$$

For a finite [module](../../../../../module-mathematics.md), $|NM|=|M|/|\ker N|$ and $|DM|=|M|/|\ker D|$ show that the two [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) [groups](../../../../../group-split.md) have equal order. Thus the [Herbrand quotient of a finite module](../../../../../herbrand-quotient-of-a-finite-module.md) is one. For the trivial integral [module](../../../../../module-mathematics.md) $\mathbb Z$, the two groups are $\mathbb Z/n\mathbb Z$ and zero, giving $h_G(\mathbb Z)=n$.

We also need [cyclic cohomology of a regular lattice](../../../../../cyclic-cohomology-of-a-regular-lattice.md). In $R[G]$, fixed coefficient vectors are constant, and every such vector is a norm of a basis vector times its coefficient. The [kernel](../../../../../kernel-of-a-linear-map.md) of $N$ consists of vectors whose coefficient sum is zero. For such a vector $(a_i)$, solve $b_{i-1}-b_i=a_i$ successively around the cycle; the final equation holds precisely because $\sum_i a_i=0$. Thus $\ker N=DR[G]$. Both [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) [groups](../../../../../group-split.md) vanish, so $h_G(R[G])=1$, for $R=\mathbb Z$ or $\mathbb Z_p$, and likewise for finite direct sums.

Now take a cyclic extension $L/K$ of [p-adic fields](../../../../../p-adic-field.md) of degree $n$. Write $U_L^r=1+\mathfrak p_L^r$. For $r>v_L(p)/(p-1)$, the convergent [p-adic logarithm](../../../../../p-adic-logarithm.md) and [p-adic exponential](../../../../../p-adic-exponential-function.md) give mutually inverse $G$-equivariant [group isomorphisms](../../../../../group-isomorphism.md)

$$
U_L^r\cong\mathfrak p_L^r,
$$

where the right side is additive. The convergence assertion follows from the estimates $v_L(x^j/j)\ge jv_L(x)-v_L(p)v_p(j)$ and $v_L(x^j/j!)\ge jv_L(x)-v_L(p)j/(p-1)$; formal inverse identities therefore hold on this ball.

By the [normal basis theorem](../../../../../normal-basis-theorem.md), choose $\theta$ so that $\{\sigma^i\theta\}$ is a $K$-[basis](../../../../../basis.md) of $L$. The lattice $A=\sum_i\mathcal O_K\sigma^i\theta$ is a regular $\mathcal O_K[G]$-[module](../../../../../module-mathematics.md). It is a finite direct sum of regular $\mathbb Z_p[G]$-[modules](../../../../../module-mathematics.md), hence its [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) vanishes. The lattices $A$ and $\mathfrak p_L^r$ are commensurable: their intersection has finite index in both. The exact sequences with these finite quotients establish finiteness of the [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) [groups](../../../../../group-split.md) and show $h_G(\mathfrak p_L^r)=1$. Thus $h_G(U_L^r)=1$. Since $\mathcal O_L^\times/U_L^r$ is finite, $h_G(\mathcal O_L^\times)=1$ as well.

The $G$-equivariant [valuation](../../../../../valuation.md) exact sequence is

$$
1\longrightarrow\mathcal O_L^\times\longrightarrow L^\times\xrightarrow{v_L}\mathbb Z\longrightarrow0.
$$

Its last term has trivial $G$-action. The multiplication rule gives the [Herbrand quotient of the local multiplicative group](../../../../../herbrand-quotient-of-the-local-multiplicative-group.md):

$$
h_G(L^\times)=n.
$$

All the [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) [groups](../../../../../group-split.md) here are finite by the lattice argument and the exact sequence; finiteness of the norm index has not been assumed.

For completeness we prove the needed [Hilbert theorem 90](../../../../../hilbert-s-theorem-90.md). If $a\in L^\times$ has [field norm](../../../../../field-norm.md) one, put $A_0=1$ and $A_i=\prod_{j=0}^{i-1}\sigma^j(a)$. The linear map $c\mapsto b=\sum_{i=0}^{n-1}A_i\sigma^i(c)$ is not zero by [linear independence of distinct field embeddings](../../../../../linear-independence-of-distinct-field-embeddings.md). Choose $c$ with $b\ne0$. The relation $A_n=1$ gives $a\sigma(b)=b$, so $a=b/\sigma(b)$. This proves $\widehat H^{-1}(G,L^\times)=0$. The zeroth [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) [group](../../../../../group-split.md) is $K^\times/N_{L/K}L^\times$. Consequently the [cyclic local norm index](../../../../../cyclic-local-norm-index.md) is

$$
\boxed{[K^\times:N_{L/K}L^\times]=[L:K]=n.}
$$

Writing $n=ef$, the [valuation](../../../../../valuation.md) of a [field norm](../../../../../field-norm.md) is $v_K(Nx)=f v_L(x)$. The valuation quotient has order $f$, and a norm with [valuation](../../../../../valuation.md) zero comes from a unit. Therefore

$$
\boxed{[\mathcal O_K^\times:N_{L/K}\mathcal O_L^\times]=e.}
$$

In particular every unit is a norm in an [unramified extension](../../../../../unramified-extension.md). These results give the norm assertions used in the [quadratic Hilbert symbol](../../../../../quadratic-hilbert-symbol.md) computation.

We finish with the [Hasse norm theorem](../../../../../hasse-norm-theorem.md): **for a cyclic extension of number fields, an element is a global norm if and only if it is a norm at every place**. More precisely the local norm is the norm from the product $L\otimes_K K_v$; in a [Galois extension](../../../../../finite-galois-extension.md) its factors have the same norm subgroup. The forward implication is immediate. For the converse associate to $a\in K^\times$ the [cyclic algebra](../../../../../cyclic-algebra.md) $(L/K,\sigma,a)$. The [splitting criterion for a cyclic algebra](../../../../../splitting-criterion-for-a-cyclic-algebra.md), proved below, identifies its splitting with $a\in N_{L/K}L^\times$. At a place where the tensor product of fields has several factors, this [algebra](../../../../../algebra-split.md) is a matrix algebra over the [cyclic algebra](../../../../../cyclic-algebra.md) of one decomposition-field factor, with the generator restricted to its cyclic decomposition subgroup. Thus the local norm assumption makes its [Brauer class](../../../../../brauer-class.md) zero at every place. Injectivity in the [Albert-Brauer-Hasse-Noether theorem](../../../../../albert-brauer-hasse-noether-theorem.md) makes the global [Brauer class](../../../../../brauer-class.md) zero, giving the desired global norm. This is the required proof outline; cyclicity is essential to this reduction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
