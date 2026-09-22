<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $A=RG$. An [idempotent](../../../../../idempotent.md) is an element $e$ with $e^2=e$; it is [central idempotent](../../../../../central-idempotent.md) when it commutes with every element of the [ring](../../../../../ring.md). In a commutative [ring](../../../../../ring.md) centrality is automatic. Two [idempotents](../../../../../idempotent.md) are [orthogonal idempotents](../../../../../orthogonal-idempotent.md) if $ef=fe=0$. A nonzero [primitive central idempotent](../../../../../primitive-central-idempotent.md) cannot be expressed as the sum of two nonzero orthogonal [central idempotents](../../../../../central-idempotent.md); this is primitivity in $Z(A)$, not necessarily primitivity in $A$.

A [block of a group algebra](../../../../../block-of-a-group-algebra.md) is an indecomposable two-sided direct-summand [ideal](../../../../../ideal.md) of $A$, equivalently an [ideal](../../../../../ideal.md) $Ae$ with $e$ a [primitive central idempotent](../../../../../primitive-central-idempotent.md). Here is the equivalence. If $A=B\oplus C$ as two-sided [ideals](../../../../../ideal.md), then $BC=CB=0$. Write $1=e+f$ with $e\in B,f\in C$. Multiplication by this equality shows that $e$ is the identity of $B$, that $f$ is the identity of $C$, and that $e,f$ are orthogonal [central idempotents](../../../../../central-idempotent.md). Conversely a [central idempotent](../../../../../central-idempotent.md) gives $A=Ae\oplus A(1-e)$. Splitting the [ideal](../../../../../ideal.md) further is therefore equivalent to splitting its [central idempotent](../../../../../central-idempotent.md) further.

For uniqueness, suppose $1=\sum_i e_i=\sum_j f_j$ are decompositions into [primitive central idempotents](../../../../../primitive-central-idempotent.md). For each $i$,

$$
e_i=\sum_j e_if_j
$$

is an orthogonal central-idempotent decomposition. Exactly one summand is nonzero, and that summand equals $e_i$. Applying the same reasoning to the corresponding $f_j$ gives $e_i=f_j$. Thus **the blocks, and their identities, are unique up to ordering**. Existence in the paper's coefficient [rings](../../../../../ring.md) follows from finite-dimensionality over $k$, and over $\mathcal O$ from completeness and [idempotent lifting](../../../../../idempotent-lifting.md) of the decomposition modulo its maximal [ideal](../../../../../ideal.md).

Over $k$, a [principal indecomposable module](../../../../../principal-indecomposable-module.md) is an indecomposable summand of the regular left [module](../../../../../module-mathematics.md) $A=kG$, equivalently $P=Ae$ for a [primitive idempotent](../../../../../primitive-idempotent.md) $e$ of $A$. Put $J=J(A)$, the [Jacobson radical](../../../../../jacobson-radical.md). The [head of a module](../../../../../head-of-a-module.md) $P/JP$ is nonzero and semisimple. It is simple: projectivity gives a surjection

$$
\operatorname{End}_A(P)\longrightarrow\operatorname{End}_{A/J}(P/JP),
$$

whose kernel consists of maps into $JP$ and is nilpotent, since a product of $r$ such maps sends $P$ into $J^rP$. If the [head of a module](../../../../../head-of-a-module.md) split, a nontrivial projection on it would lift by [idempotent lifting](../../../../../idempotent-lifting.md) to a nontrivial projection on $P$, contradicting indecomposability. Every maximal submodule contains $JP$, since $J$ annihilates simple [modules](../../../../../module-mathematics.md). The simplicity of the [head of a module](../../../../../head-of-a-module.md) now proves **$J(P)=JP$ is the unique maximal submodule**, and $P$ is its [head of a module](../../../../../head-of-a-module.md)'s [projective cover](../../../../../projective-cover.md).

Choose the simple [modules](../../../../../module-mathematics.md) $S_1,\ldots,S_r$, with corresponding [projective covers](../../../../../projective-cover.md) $P_1,\ldots,P_r$. Our convention for the [Cartan matrix of a group algebra](../../../../../cartan-matrix-of-a-group-algebra.md) is

$$
\boxed{(C_G)_{ij}=[P_j:S_i],}
$$

where brackets denote the multiplicity in a [composition series](../../../../../composition-series.md).

For the final two unheaded requests, retain the additional hypothesis $G=NC_G(N)$. Choose a central [subgroup](../../../../../subgroup.md) $Z=\langle z\rangle$ of $N$ of order $p$. Every element of $N$ centralizes $Z$, and so does every element of $C_G(N)$; hence $Z\le Z(G)$. Set $t=z-1$, so $t$ is central and $t^p=0$, and $A/tA\cong k(G/Z)$.

To lift a [central idempotent](../../../../../central-idempotent.md) $\bar e$ of this quotient, first lift it as an [idempotent](../../../../../idempotent.md) $e$ by [idempotent refinement theorem](../../../../../idempotent-refinement-theorem.md). Since $\bar e$ is central, $eA(1-e)\subseteq tA$. Multiplying a representation $e a(1-e)=t b$ on the left and right by $e,1-e$ gives

$$
eA(1-e)\subseteq t eA(1-e)\subseteq\cdots\subseteq t^p eA(1-e)=0.
$$

The other off-diagonal corner vanishes likewise, so $e$ is central. Two central lifts of the same [idempotent](../../../../../idempotent.md) coincide: their mismatched products $e(1-f)$ and $f(1-e)$ are [idempotents](../../../../../idempotent.md) in the nilpotent kernel and therefore zero. Primitivity is preserved because orthogonal [idempotent](../../../../../idempotent.md) decompositions lift. Thus the central $p$-quotient gives a bijection of block [idempotents](../../../../../idempotent.md).

The quotient $G/Z$ still satisfies the required hypothesis for $N/Z$, because the image of $C_G(N)$ centralizes $N/Z$. Induction on $|N|$ therefore proves **$\tau$ bijects the block [idempotents](../../../../../idempotent.md) of $kG$ and $k(G/N)$**. The centrality argument is essential: a general nilpotent [algebra](../../../../../algebra-split.md) quotient need not give a bijection of central block [idempotents](../../../../../idempotent.md).

For the [Cartan matrix of a group algebra](../../../../../cartan-matrix-of-a-group-algebra.md), every projective $A$-module is free over $kZ$: $A$ is free over $kZ$, a projective $A$-module is a summand of a finite free $A$-module, and finite projectives over the [local ring](../../../../../local-ring.md) $kZ\cong k[t]/(t^p)$ are free. If $P$ is a [principal indecomposable module](../../../../../principal-indecomposable-module.md), $\bar P=P/tP$ is a [principal indecomposable module](../../../../../principal-indecomposable-module.md) over $A/tA$: an [idempotent](../../../../../idempotent.md) splitting of its [endomorphism ring](../../../../../endomorphism-ring.md) would lift and split $P$. The $p$ quotients of its filtration

$$
P\supset tP\supset\cdots\supset t^{p-1}P\supset0
$$

are all isomorphic to $\bar P$ as $k(G/Z)$-modules, by multiplication by the corresponding power of $t$. All simple [modules](../../../../../module-mathematics.md) are annihilated by the [nilpotent ideal](../../../../../nilpotent-ideal.md) $tA$. Hence $[P:S]=p[\bar P:S]$, with the natural indexing of simple [modules](../../../../../module-mathematics.md), and $C_G=pC_{G/Z}$. Iterating over $N$ gives

$$
\boxed{C_G=|N|C_{G/N}.}
$$

This is [blocks and Cartan matrices under central p-quotients](../../../../../blocks-and-cartan-matrices-under-central-p-quotients.md). The extra hypothesis is still in force: for example $N=C_3\trianglelefteq S_3$ in characteristic three does not satisfy it, and its [Group algebra Cartan matrix](../../../../../cartan-matrix-of-a-group-algebra.md) is $\left(\begin{smallmatrix}2&1\\1&2\end{smallmatrix}\right)$ rather than $3I$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
