<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use finite-dimensional $k$-modules or finite $R$-free lattices. We use the basic relative-projectivity facts that [Krull-Schmidt decomposition](../../../../../krull-schmidt-decomposition.md) holds with local endomorphism rings, [module vertices](../../../../../vertex-of-an-indecomposable-module.md) are conjugate [p-subgroups](../../../../../p-subgroup.md), and a [module source](../../../../../source-of-an-indecomposable-module.md) $S$ at a [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$ satisfies $S\mid M\downarrow_D$ and $M\mid S\uparrow^G$. [Module induction](../../../../../induced-representation.md) is transitive and [Mackey restriction formula](../../../../../mackey-restriction-formula.md) gives [module vertex](../../../../../vertex-of-an-indecomposable-module.md) containment for restrictions and inductions. In particular, a summand induced from $D$ has [module vertex](../../../../../vertex-of-an-indecomposable-module.md) conjugate into $D$, and [module restriction](../../../../../restriction-of-a-representation.md) to a subgroup containing a chosen [module vertex](../../../../../vertex-of-an-indecomposable-module.md) retains a summand with that [module vertex](../../../../../vertex-of-an-indecomposable-module.md). The latter follows from the [module source](../../../../../source-of-an-indecomposable-module.md) conditions and minimality: restricting further to $D$ must still contain its [module source](../../../../../source-of-an-indecomposable-module.md), whose [module vertex](../../../../../vertex-of-an-indecomposable-module.md) is $D$.

The [module vertex](../../../../../vertex-of-an-indecomposable-module.md)-$D$ form of [Green correspondence](../../../../../green-correspondence.md) states that for $N_G(D)\leq H\leq G$ there is a bijection between indecomposable $RG$-modules with [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$ and indecomposable $RH$-modules with [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$. Its maps select the unique [module vertex](../../../../../vertex-of-an-indecomposable-module.md)-$D$ summands of [module restriction](../../../../../restriction-of-a-representation.md) and induction, using $H$-conjugacy for restricted [module vertices](../../../../../vertex-of-an-indecomposable-module.md) and $G$-conjugacy for induced [module vertices](../../../../../vertex-of-an-indecomposable-module.md). They occur with multiplicity one and have the same [module sources](../../../../../source-of-an-indecomposable-module.md). Other induction summands have [module vertices](../../../../../vertex-of-an-indecomposable-module.md) conjugate to proper subgroups of $D$. The [module restriction](../../../../../restriction-of-a-representation.md) remainder is relatively projective for

$$
\mathcal Y=\{H\cap aDa^{-1}:a\in G\setminus H\}.
$$

Relative projectivity for a family means being a summand of a finite sum of inductions from its members. We prove this form; no stronger description of the induction remainder is needed for the application.

Let $U$ have [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$ over $H$. The identity [double coset](../../../../../double-coset.md) in [Mackey restriction formula](../../../../../mackey-restriction-formula.md) gives

$$
(U\uparrow^G)\downarrow_H=U\oplus T.
$$

Since $U$ is relatively $D$-projective, a further Mackey decomposition puts every other [double coset](../../../../../double-coset.md) term in the relatively-$\mathcal Y$ family. No member of $\mathcal Y$ contains an $H$-conjugate of $D$. Otherwise, conjugation within $H$ would give $D\leq H\cap (ha)D(ha)^{-1}$ with $h\in H$, $a\notin H$. Equality of orders then makes $ha\in N_G(D)\leq H$, a contradiction. Therefore the [module restriction](../../../../../restriction-of-a-representation.md) above contains exactly one summand with [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $H$-conjugate to $D$, namely $U$ once.

Decompose $U\uparrow^G$ into [indecomposable modules](../../../../../indecomposable-module.md). All their [module vertices](../../../../../vertex-of-an-indecomposable-module.md) are conjugate into $D$. Each one with a [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $G$-conjugate to $D$ can take $D$ itself as [module vertex](../../../../../vertex-of-an-indecomposable-module.md) and contributes a [module vertex](../../../../../vertex-of-an-indecomposable-module.md)-$D$ summand on [module restriction](../../../../../restriction-of-a-representation.md) to $H$. There can thus be at most one such summand and its multiplicity is one. There must be at least one, because smaller [module vertices](../../../../../vertex-of-an-indecomposable-module.md) cannot restrict to produce $U$, with [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$, in the displayed decomposition. Define $g(U)$ to be that summand. Its [module restriction](../../../../../restriction-of-a-representation.md) contains $U$ once, with remainder a summand of $T$. All other induction summands have strictly smaller [module vertices](../../../../../vertex-of-an-indecomposable-module.md). This is [Green correspondence from Mackey multiplicity](../../../../../green-correspondence-from-mackey-multiplicity.md).

Conversely take $M$ of [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$ over $G$ with [module source](../../../../../source-of-an-indecomposable-module.md) $S$. Decompose $S\uparrow^H$ into [indecomposable modules](../../../../../indecomposable-module.md). Since $M\mid S\uparrow^G=(S\uparrow^H)\uparrow^G$, the local [endomorphism ring](../../../../../endomorphism-ring.md) and [Krull-Schmidt decomposition](../../../../../krull-schmidt-decomposition.md) give $M\mid U\uparrow^G$ for one indecomposable summand $U$ of $S\uparrow^H$. Its [module vertex](../../../../../vertex-of-an-indecomposable-module.md) is $H$-conjugate to $D$: all [module vertices](../../../../../vertex-of-an-indecomposable-module.md) are conjugate into $D$, and a smaller one could not induce $M$. The preceding uniqueness makes $g(U)=M$ and identifies $U$ as the unique [module vertex](../../../../../vertex-of-an-indecomposable-module.md)-$D$ summand of $M\downarrow_H$. Define $f(M)=U$. This proves $f(g(U))=U$ and $g(f(M))=M$.

If $S$ is a [module source](../../../../../source-of-an-indecomposable-module.md) of $U$, then $S\mid U\downarrow_D\mid M\downarrow_D$ and $M\mid U\uparrow^G\mid S\uparrow^G$. These two conditions and the common [module vertex](../../../../../vertex-of-an-indecomposable-module.md) show that $S$ is also a [module source](../../../../../source-of-an-indecomposable-module.md) of $M$. Thus the correspondence preserves [module sources](../../../../../source-of-an-indecomposable-module.md), including [trivial source modules](../../../../../trivial-source-module.md), and the proof is complete under the stated coefficient conventions.

For the required expression, a [p-local module](../../../../../p-local-module.md) is a finite sum of inductions from $N_G(Q)$ for nontrivial [p-subgroups](../../../../../p-subgroup.md) $Q$. Induct on the order of a [module vertex](../../../../../vertex-of-an-indecomposable-module.md) of $M$. Vertex 1 makes $M$ projective, so choose $L_1=L_2=P_1=0$, $P_2=M$.

For [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D\ne1$, take $U=f(M)$ for $H=N_G(D)$. Its [module induction](../../../../../induced-representation.md) is p-local and

$$
U\uparrow^G=M\oplus\bigoplus_iX_i
$$

with smaller [module vertices](../../../../../vertex-of-an-indecomposable-module.md) for the $X_i$. By induction, write

$$
X_i\oplus A_i\oplus P_i\cong B_i\oplus Q_i,
$$

with $A_i,B_i$ p-local and $P_i,Q_i$ projective. Adding these identities and substituting the induction decomposition gives

$$
M\oplus\bigoplus_iB_i\oplus\bigoplus_iQ_i
\cong\left(U\uparrow^G\oplus\bigoplus_iA_i\right)\oplus\bigoplus_iP_i.
$$

Hence the explicit choices

$$
\boxed{L_1=\bigoplus_iB_i,\quad P_1=\bigoplus_iQ_i,\quad
L_2=U\uparrow^G\oplus\bigoplus_iA_i,\quad P_2=\bigoplus_iP_i}
$$

work. All sums are finite and [module vertex](../../../../../vertex-of-an-indecomposable-module.md) orders strictly decrease, so the induction terminates. If $N_G(D)=G$, induction from that [normalizer](../../../../../normalizer.md) is still allowed by the definition of p-local.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
