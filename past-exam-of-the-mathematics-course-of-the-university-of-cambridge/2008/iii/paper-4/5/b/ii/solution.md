<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $N=N_G(D)$ and $b=\operatorname{Br}_D(e)$. If $eM=M$, the [Nagao module theorem](../../../../../../../nagao-module-theorem.md) with $K=N$ puts every vertex-$D$ summand of $M\downarrow_N$ inside $bM$. In particular its [Green correspondence](../../../../../../../green-correspondence.md) summand $M'$ satisfies $bM'=M'$.

Conversely a [central idempotent](../../../../../../../central-idempotent.md) acts as zero or one on the [indecomposable module](../../../../../../../indecomposable-module.md) $M$. If $eM=0$, apply the same theorem to $1-e$. Its Brauer image is $1-b$, so $(1-b)M'=M'$, incompatible with $bM'=M'$. Thus

$$
\boxed{eM=M\quad\Longleftrightarrow\quad\operatorname{Br}_D(e)M'=M'.}
$$

For the unheaded induction request, write $\mathcal X=\{D\cap{}^gD:g\notin N\}$. We prove the sharper intersection bound, not just a drop in [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) size. We use [Green correspondence](../../../../../../../green-correspondence.md) on permutation bimodules and the usual [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) test for a permutation-module summand: its [Brauer quotient of a module](../../../../../../../brauer-quotient-of-a-module.md) at $P$ is nonzero precisely when a [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) contains a conjugate of $P$. This test follows by restricting to the $p$-group $P$, decomposing the permutation basis into its orbits, and noting that proper-orbit sums are precisely the proper-subgroup transfer terms.

Consider $kG$ as a $k[G\times D]$-module, with $(g,d)a=gad^{-1}$. It is the transitive [permutation module](../../../../../../../permutation-module.md) induced from $\Delta D$. Set $L=G\times D$ and $L_0=N\times D$; the latter contains $N_L(\Delta D)$. Its restriction decomposes as

$$
kG\downarrow_{L_0}=kN\oplus\bigoplus_{g\in N\backslash G/D,\ g\notin N}k[NgD].
$$

Each outside term has stabilizer a conjugate of a [subgroup](../../../../../../../subgroup.md) of $\Delta D$. If a diagonal [subgroup](../../../../../../../subgroup.md) $\Delta Q\le\Delta D$ embeds into one of these stabilizers, then $Q\le D\cap{}^gD$ for an outside representative. Thus its diagonal [module vertices](../../../../../../../vertex-of-an-indecomposable-module.md) are in the intersection error family.

Every indecomposable $L_0$-summand of $kN$ has [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) $\Delta D$. To justify this, its endomorphisms are right multiplications by elements of $(kN)^D$. The coefficient projection $\operatorname{Br}_D^N$ on this [algebra](../../../../../../../algebra-split.md) has nilpotent kernel: every nonsingleton $D$-orbit sum lies in the kernel of $kN\to k(N/D)$, by part 1(b), and that kernel is nilpotent by part 1(a). Hence no nonzero [idempotent](../../../../../../../idempotent.md) endomorphism can have zero Brauer image. Its image summand has nonzero [Brauer quotient of a module](../../../../../../../brauer-quotient-of-a-module.md) at $\Delta D$, and its [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md), already contained in a conjugate of $\Delta D$, must be $\Delta D$.

Apply the general [Green correspondence](../../../../../../../green-correspondence.md) from part (a) to $L,L_0$. If an indecomposable summand of $kG$ has [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) outside the intersection error family, its correspondent must be a summand of $kN$, since the outside double-coset [modules](../../../../../../../module-mathematics.md) have only error-family [module vertices](../../../../../../../vertex-of-an-indecomposable-module.md). It therefore has [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) $\Delta D$. Consequently **every summand of $kG$ not having [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) $\Delta D$ has [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) conjugate into an outside diagonal intersection**. An intersection

$$
\Delta D\cap{}^{(g,d)}\Delta D
$$

with $(g,d)\notin L_0$ projects in its first coordinate into $D\cap{}^gD$ with $g\notin N$; this is the error family required in the question.

Now form the split permutation bimodule

$$
W=(1-e)kG b.
$$

Its [Brauer quotient of a module](../../../../../../../brauer-quotient-of-a-module.md) at $\Delta D$ is zero. Indeed $kG(\Delta D)=kC_G(D)$, left multiplication by $e$ becomes multiplication by $\operatorname{Br}_D(e)=b$, and right multiplication by $b$ remains multiplication by $b$. Therefore

$$
W(\Delta D)=(1-b)kC_G(D)b=0.
$$

Here $b$ is central in $kC_G(D)$, so the last product is zero. Every indecomposable bimodule summand of $W$ consequently has [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) in the outside intersection family, by the preceding paragraph, and has trivial [module source](../../../../../../../source-of-an-indecomposable-module.md) since it is a permutation-module summand.

Since $V$ has vertex $D$, necessarily $D\le K$. Let $S$ be a [module source](../../../../../../../source-of-an-indecomposable-module.md) of $V$ at $D$. The splitting $V\mid kK\otimes_{kD}S$ remains a splitting after applying $b$, since $bV=V$. Inducing to $G$ and applying $1-e$ gives

$$
(1-e)\operatorname{Ind}_K^G V\mid W\otimes_{kD}S.
$$

A trivial-source bimodule summand with [module vertex](../../../../../../../vertex-of-an-indecomposable-module.md) conjugate into $\Delta Q$ is a summand of $\operatorname{Ind}_{\Delta Q}^{G\times D}k$. Tensoring with $S$ turns this into a [module](../../../../../../../module-mathematics.md) induced to $G$ from $Q$ (with the appropriate conjugate restriction of $S$). Thus every summand on the right is relatively projective for some $Q\le D\cap{}^gD$, $g\notin N$. Each $V_j$ lies in the left-hand side, and [Krull–Schmidt theorem](../../../../../../../krull-schmidt-theorem.md) now gives

$$
\boxed{D_j\le_G D\cap{}^gD\quad\text{for some }g\in G\setminus N_G(D).}
$$

This proves [Juhász induction refinement](../../../../../../../juhasz-induction-refinement.md). If there are no outside elements, the error family is empty and the complementary [module](../../../../../../../module-mathematics.md) is zero.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
