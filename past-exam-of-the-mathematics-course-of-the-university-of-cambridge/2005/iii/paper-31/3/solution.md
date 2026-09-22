<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We give the detailed norm-index argument for a cyclic extension $L/K$ of [p-adic fields](../../../../../p-adic-field.md); thus $K$ is a finite extension of $\mathbb Q_p$. Write $G=\langle\sigma\rangle$, $|G|=n$. For an additive $G$-[module](../../../../../module-mathematics.md) $M$, put $D=\sigma-1$ and $N=1+\sigma+\cdots+\sigma^{n-1}$. The two periodic [Tate cohomology of a cyclic group](../../../../../tate-cohomology-of-a-cyclic-group.md) [groups](../../../../../group-split.md) and the [Herbrand quotient](../../../../../herbrand-quotient.md) are

$$
\widehat H^0(G,M)=\ker D/NM,\qquad
\widehat H^{-1}(G,M)=\ker N/DM,\qquad
h_G(M)=\frac{|\widehat H^0(G,M)|}{|\widehat H^{-1}(G,M)|},
$$

when these [groups](../../../../../group-split.md) are finite. For multiplicative [modules](../../../../../module-mathematics.md), $N$ is the product of conjugates and $D(z)=\sigma(z)/z$.

The periodic complex alternating $D$ and $N$ gives a six-term [exact sequence](../../../../../exact-sequence.md) for every [short exact sequence](../../../../../short-exact-sequence.md) of [modules](../../../../../module-mathematics.md). Taking the alternating product of the [finite group](../../../../../finite-group.md) orders in that [exact sequence](../../../../../exact-sequence.md) proves

$$
h_G(M)=h_G(M')h_G(M'')\quad\text{if }0\to M'\to M\to M''\to0.
$$

For a finite [module](../../../../../module-mathematics.md), the counting fibers gives $|NM|=|M|/|\ker N|$ and $|DM|=|M|/|\ker D|$, so the two Tate [groups](../../../../../group-split.md) have equal order. This proves the [Herbrand quotient of a finite module](../../../../../herbrand-quotient-of-a-finite-module.md) is one. It follows that replacing a [module](../../../../../module-mathematics.md) by a finite-index submodule does not change its quotient, whenever the [cohomology groups](../../../../../cohomology-group.md) are finite.

Two basic calculations drive the norm computation. For the trivial [module](../../../../../module-mathematics.md) $\mathbb Z$, $D=0$ and $N$ is multiplication by $n$, so $h_G(\mathbb Z)=n$. For a regular lattice $R[G]$, with $R=\mathbb Z_p$, invariants are constant coefficient vectors and every such vector is a norm: put its constant coefficient in just one coordinate before applying $N$. The [group kernel](../../../../../kernel-of-a-group-homomorphism.md) of $N$ consists of the coefficient vectors of sum zero. Successively taking [partial sums](../../../../../partial-sum.md) solves the cyclic difference equation $Dx=y$ for every such vector $y$. Thus both Tate [groups](../../../../../group-split.md) vanish and $h_G(R[G])=1$. This is [cyclic cohomology of a regular lattice](../../../../../cyclic-cohomology-of-a-regular-lattice.md).

Let $U_L=\mathcal O_L^\times$ and $U_L^r=1+\mathfrak P_L^r$. For sufficiently large $r$, the [p-adic logarithm](../../../../../p-adic-logarithm.md) and [p-adic exponential](../../../../../p-adic-exponential-function.md) are inverse $G$-equivariant [isomorphisms](../../../../../isomorphism.md)

$$
\log:U_L^r\xrightarrow{\sim}\mathfrak P_L^r.
$$

To make the range explicit, $r>v_L(p)/(p-1)$ suffices: the higher terms in the logarithm and exponential have greater [valuation](../../../../../valuation.md) than their leading terms, their series converge there, and the identities $\log(\exp x)=x$ and $\exp(\log(1+x))=1+x$ remain valid. Thus a deep multiplicative [unit group](../../../../../unit-group.md) becomes an additive $\mathbb Z_p$-lattice in $L$.

By the [normal basis theorem](../../../../../normal-basis-theorem.md), $L\cong K[G]$ as a $K[G]$-module. As a $\mathbb Q_p[G]$-module it is therefore $\mathbb Q_p[G]^{[K:\mathbb Q_p]}$. Transport the regular lattice $M_0=\mathbb Z_p[G]^{[K:\mathbb Q_p]}$ into $L$. Both $M_0$ and $\mathfrak P_L^r$ are full $G$-stable $\mathbb Z_p$-lattices, so their intersection has finite index in each. The [exact sequences](../../../../../exact-sequence.md) with finite quotients show that the Tate [groups](../../../../../group-split.md) of $\mathfrak P_L^r$ are finite and that

$$
h_G(U_L^r)=h_G(\mathfrak P_L^r)=h_G(M_0)=1.
$$

Since $U_L/U_L^r$ is finite, the exact-sequence formula for the [Herbrand quotient](../../../../../herbrand-quotient.md) gives $h_G(U_L)=1$. Finally, the [valuation](../../../../../valuation.md) sequence

$$
1\longrightarrow U_L\longrightarrow L^\times\xrightarrow{v_L}\mathbb Z\longrightarrow0
$$

has trivial $G$-action on $\mathbb Z$. Hence the [Herbrand quotient of the local multiplicative group](../../../../../herbrand-quotient-of-the-local-multiplicative-group.md) is

$$
h_G(L^\times)=h_G(U_L)h_G(\mathbb Z)=n.
$$

For [completeness](../../../../../completeness.md), the denominator vanishes by [Hilbert theorem 90](../../../../../hilbert-s-theorem-90.md). If $N_{L/K}a=1$, put $c_0=1$ and $c_j=a\sigma(a)\cdots\sigma^{j-1}(a)$. Independence of distinct [field automorphisms](../../../../../field-automorphism.md) lets us choose $t\in L$ with $b=\sum_{j=0}^{n-1}c_j\sigma^j(t)\ne0$. Since $c_n=1$, shifting the sum gives $\sigma(b)=b/a$. Thus $a=b/\sigma(b)$, a multiplicative coboundary. Therefore $\widehat H^{-1}(G,L^\times)=1$. The invariant [subgroup](../../../../../subgroup.md) of $L^\times$ is $K^\times$, so

$$
\boxed{[K^\times:N_{L/K}L^\times]=[L:K]=n.}
$$

This proves the [cyclic local norm index](../../../../../cyclic-local-norm-index.md) without assuming local reciprocity. If the extension has [ramification index](../../../../../ramification-index.md) $e$ and [residue degree](../../../../../residue-degree.md) $f$, the [valuation](../../../../../valuation.md) formula $v_K(Nz)=f\,v_L(z)$ shows that the [valuation](../../../../../valuation.md) contribution to the index is $f$. A norm is a unit only when $z$ is a unit, so the remaining contribution is

$$
[U_K:N_{L/K}U_L]=e.
$$

In particular, unit norms are surjective in an unramified cyclic extension. The norm [subgroup](../../../../../subgroup.md) is open: on deep units its logarithm is $\operatorname{Tr}_{L/K}(\mathfrak P_L^r)$, a nonzero full lattice in $K$, and therefore contains a sufficiently deep principal-unit [group](../../../../../group-split.md). This connects the index calculation to the open finite-index norm [subgroups](../../../../../subgroup.md) classified by [local class field theory](../../../../../local-class-field-theory.md).

To finish, the [Hasse norm theorem](../../../../../hasse-norm-theorem.md) for a cyclic extension of [number fields](../../../../../number-field.md) states that a nonzero element is a global norm if and only if it is a norm at every finite and infinite completion. Here is its Brauer-theoretic proof outline. Associate to $a\in K^\times$ the [cyclic algebra](../../../../../cyclic-algebra.md) $A=(L/K,\sigma,a)$, with relations $z\ell=\sigma(\ell)z$ and $z^n=a$. The [splitting criterion for a cyclic algebra](../../../../../splitting-criterion-for-a-cyclic-algebra.md) says that it splits exactly when $a=Nc$: if $a=Nc$, multiplication by $L$ and the operator $c\sigma$ realize it as $\operatorname{End}_K(L)$; conversely, in a split [matrix representation](../../../../../matrix-representation.md), the underlying $n$-dimensional space is one-dimensional over $L$, so $z$ must act as $c\sigma$ and $z^n=Nc$.

Apply this criterion at every completion, using the restricted cyclic character and any one completion of $L$ above that place. If $a$ is a local norm everywhere, every localized Brauer class is zero. [Injectivity](../../../../../injective-function.md) in the [Albert-Brauer-Hasse-Noether theorem](../../../../../albert-brauer-hasse-noether-theorem.md) forces $[A]=0$ in $\operatorname{Br}(K)$; the global splitting criterion gives $a=Nc$. Conversely, a global norm is a local norm after completion, since the norm on $L\otimes_K K_v$ is the product of the component norms, whose images coincide in the Galois case. **The cyclic hypothesis is essential**; the stated local-global principle does not hold for arbitrary extensions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
