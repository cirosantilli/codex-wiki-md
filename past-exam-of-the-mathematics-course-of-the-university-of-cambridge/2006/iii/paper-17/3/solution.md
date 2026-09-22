<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [sheaf of abelian groups](../../../../../sheaf-of-abelian-groups.md) $\mathcal F$ on a [topological space](../../../../../topological-space.md) $X$, put

$$
C(\mathcal F)(U)=\prod_{P\in U}\mathcal F_P.
$$

These arbitrary families of [germs](../../../../../germ-of-a-sheaf-section.md) form a [sheaf](../../../../../sheaf-mathematics.md), and restrictions are projections. Extending a family by zero proves that $C(\mathcal F)$ is [flasque](../../../../../flasque-sheaf.md). Sending a section to all its [germs](../../../../../germ-of-a-sheaf-section.md) gives an injective [sheaf](../../../../../sheaf-mathematics.md) map $\mathcal F\to C(\mathcal F)$, since a section with every [germ](../../../../../germ-of-a-sheaf-section.md) zero vanishes locally and hence globally.

Set $Q^{-1}=\mathcal F$, $I^j=C(Q^{j-1})$ and $Q^j=\operatorname{coker}(Q^{j-1}\to I^j)$, using the [sheaf](../../../../../sheaf-mathematics.md) [cokernel](../../../../../cokernel.md). Compose $I^j\to Q^j\to I^{j+1}$ to obtain the [Godement resolution](../../../../../godement-resolution.md)

$$
0\longrightarrow\mathcal F\longrightarrow I^0\longrightarrow I^1\longrightarrow\cdots.
$$

It is exact by construction, with [flasque](../../../../../flasque-sheaf.md) terms. Define [sheaf cohomology](../../../../../sheaf-cohomology.md) by the [cohomology](../../../../../cohomology-split.md) of its global-section complex:

$$
H^j(X,\mathcal F)=H^j\bigl(\Gamma(X,I^\bullet)\bigr),\qquad
H^0(X,\mathcal F)=\Gamma(X,\mathcal F).
$$

The [resolution principle for sheaf cohomology](../../../../../resolution-principle-for-sheaf-cohomology.md) identifies this with the computation using any [flasque resolution](../../../../../flasque-resolution.md).

The elementary input for acyclicity is the [flasque-kernel section-lifting lemma](../../../../../flasque-kernel-section-lifting-lemma.md): in a [short exact sequence](../../../../../short-exact-sequence.md) with [flasque](../../../../../flasque-sheaf.md) kernel, sections of the quotient lift over every [open subset](../../../../../open-set.md). Consequently a quotient of two [flasque sheaves](../../../../../flasque-sheaf.md) is [flasque](../../../../../flasque-sheaf.md), because a quotient section lifts and that lift extends. If $\mathcal F$ itself is [flasque](../../../../../flasque-sheaf.md), induction through $0\to Q^{j-1}\to I^j\to Q^j\to0$ makes every $Q^j$ [flasque](../../../../../flasque-sheaf.md). The same lifting lemma makes these sequences exact on [global sections](../../../../../global-section.md). Hence the global-section complex has no positive-degree [cohomology](../../../../../cohomology-split.md), proving

$$
\boxed{H^j(X,\mathcal F)=0\quad(j>0)\text{ for flasque }\mathcal F}.
$$

This deduction uses the lifting lemma, not the desired cohomological vanishing as an assumption.

For the rational-section construction, add two representative sections after restricting to the intersection of their dense domains. Multiply by a representative rational function in the same way. Finite intersections of dense [open sets](../../../../../open-set.md) are dense, and further restricting both representatives does not change their resulting class. The [module](../../../../../module-mathematics.md) axioms hold on their common domain. Thus [rational sections](../../../../../rational-section-of-a-sheaf-of-modules.md) form a [module](../../../../../module-mathematics.md) over $\operatorname{Rat}(X)$; irreducibility is not needed for this [module](../../../../../module-mathematics.md) statement. When $X$ is irreducible, $\operatorname{Rat}(X)$ is the [function field](../../../../../function-field-of-an-algebraic-variety.md) $K=k(X)$.

Suppose now that $\mathcal F$ is [locally free](../../../../../locally-free-sheaf.md) and $X$ irreducible. A [germ](../../../../../germ-of-a-sheaf-section.md) at $P$ is represented on a nonempty open neighbourhood, which is dense, so it defines a [rational section](../../../../../rational-section-of-a-sheaf-of-modules.md). Two representatives of the [germ](../../../../../germ-of-a-sheaf-section.md) agree on a neighbourhood of $P$ and therefore give the same class. If the class is zero, trivialize $\mathcal F$ on a neighbourhood of $P$. Its coefficient functions vanish on a dense [open subset](../../../../../open-set.md); [regular functions](../../../../../regular-function.md) on a reduced [irreducible variety](../../../../../irreducible-variety.md) with this property vanish identically. The [germ](../../../../../germ-of-a-sheaf-section.md) is therefore zero. This proves the [stalk inclusion into rational sections of a locally free sheaf](../../../../../stalk-inclusion-into-rational-sections-of-a-locally-free-sheaf.md):

$$
\boxed{\mathcal F_P\hookrightarrow\operatorname{Rat}(\mathcal F)}.
$$

Local freeness matters: a nonzero torsion [germ](../../../../../germ-of-a-sheaf-section.md) can vanish on a dense [open set](../../../../../open-set.md).

On an irreducible [algebraic curve](../../../../../algebraic-curve.md), every proper closed subset is finite, and every [open subset](../../../../../open-set.md) is [quasi-compact](../../../../../compact-space.md) because the Zariski space is [Noetherian](../../../../../noetherian-ring.md). Let $R=\operatorname{Rat}(\mathcal F)$. The [constant sheaf](../../../../../constant-sheaf.md) $\mathcal R(\mathcal F)$ has sections $R$ on every nonempty [open set](../../../../../open-set.md): such opens are irreducible and hence connected. Define

$$
\mathcal P(\mathcal F)(U)=\bigoplus_{P\in U}R/\mathcal F_P.
$$

Restriction drops the components outside the smaller [open set](../../../../../open-set.md). For a compatible family over an open cover of $U$, take a finite subcover by quasi-compactness. The union of the finite supports of these finitely many sections is finite. Their agreeing components therefore glue to a unique finite-support tuple on $U$. This verifies the [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md), including arbitrary covers, rather than merely asserting that a presheaf direct sum is always a [sheaf](../../../../../sheaf-mathematics.md).

A [rational section](../../../../../rational-section-of-a-sheaf-of-modules.md) is regular on some dense [open set](../../../../../open-set.md), whose complement on a curve is finite. Its classes $[s]_P\in R/\mathcal F_P$ therefore have finite support, defining a [sheaf](../../../../../sheaf-mathematics.md) map $\mathcal R(\mathcal F)\to\mathcal P(\mathcal F)$. At $P$, the first [sheaf](../../../../../sheaf-mathematics.md) has [stalk](../../../../../stalk-of-a-sheaf.md) $R$. The second has [stalk](../../../../../stalk-of-a-sheaf.md) $R/\mathcal F_P$: any finite tuple can be restricted to a neighbourhood omitting all its other support points, and its $P$-component is unaffected by such restriction. The resulting sequence on [stalks](../../../../../stalk-of-a-sheaf.md) is

$$
0\to\mathcal F_P\to R\to R/\mathcal F_P\to0.
$$

Exactness of [sheaves](../../../../../sheaf-mathematics.md) can be tested on [stalks](../../../../../stalk-of-a-sheaf.md), so this proves the [rational principal-parts resolution on an algebraic curve](../../../../../rational-principal-parts-resolution-on-an-algebraic-curve.md)

$$
\boxed{0\to\mathcal F\to\mathcal R(\mathcal F)\to\mathcal P(\mathcal F)\to0}.
$$

Both right-hand [sheaves](../../../../../sheaf-mathematics.md) are [flasque](../../../../../flasque-sheaf.md): restrictions for the constant rational-section [sheaf](../../../../../sheaf-mathematics.md) are identities between nonempty opens, and restrictions for the rational principal-parts [sheaf](../../../../../sheaf-mathematics.md) are projections, with extension by zero. Consequently

$$
H^1(X,\mathcal F)\cong
\operatorname{coker}\left(R\to\bigoplus_{P\in X}R/\mathcal F_P\right),\qquad
H^j(X,\mathcal F)=0\quad(j\ge2).
$$

Surjectivity on [stalks](../../../../../stalk-of-a-sheaf.md) has not been confused with surjectivity on global sections.

For an explicit failure of global surjectivity take $X=\mathbb P^1$ and $\mathcal F=\mathcal O(-2)$. Use coordinate $z=X_1/X_0$ and frame $e_0=X_0^{-2}$ on the finite chart. At infinity use $w=1/z$ and $e_\infty=X_1^{-2}=z^{-2}e_0$. Prescribe the [rational principal part](../../../../../rational-principal-part.md) of $z^{-1}e_0$ at zero and zero at every other point. If a [rational section](../../../../../rational-section-of-a-sheaf-of-modules.md) $r(z)e_0$ realized this tuple, then $r-z^{-1}$ would be regular at zero and $r$ would be regular at every other finite point. Thus $r=z^{-1}+p(z)$ with $p\in k[z]$. Regularity at infinity would require

$$
z^2r(z)=w^{-1}+w^{-2}p(w^{-1})
$$

to be regular at $w=0$. Its $w^{-1}$ term cannot cancel with any term of the [polynomial](../../../../../polynomial-split.md) contribution, whose powers are at most $-2$. This is impossible. Hence **the global rational-principal-part map need not be surjective**.

For an affine curve it is always surjective, and here is a direct construction. Write $X=\operatorname{Spec}A$, $K=\operatorname{Frac}A$ and $\mathcal F=\widetilde M$. By the [affine module sheaf](../../../../../affine-module-sheaf.md) construction, $R=M\otimes_AK=:M_K$ and $\mathcal F_P=M_{\mathfrak m_P}$. Choose representatives $v_P\in M_K$ for a prescribed finite tuple, and choose one nonzero $a\in A$ with $av_P\in M$ for all of them. The zero set $T=V(a)$ is finite. The ring $A/(a)$ is [Artinian](../../../../../artinian-ring.md), since it is Noetherian of dimension zero, and its [Artinian decomposition into local factors](../../../../../artinian-decomposition-into-local-factors.md) gives

$$
M/aM\cong\bigoplus_{P\in T}(M/aM)_{\mathfrak m_P}.
$$

Prescribe the class of $av_P$ in the indicated component for each requested point in $T$, and zero in the other components. A requested point outside $T$ already has zero principal part because $a$ is a unit there. Lift the tuple to $w\in M$. Then $s=w/a\in M_K$ satisfies $s-v_P\in M_{\mathfrak m_P}$ at every requested point in $T$, and is regular at every other point of $T$. Outside $T$ it is regular because $a$ is invertible. It therefore realizes exactly the prescribed tuple. This proves [affine principal-parts interpolation for a locally free sheaf](../../../../../affine-principal-parts-interpolation-for-a-locally-free-sheaf.md) and gives

$$
\boxed{R\longrightarrow\bigoplus_{P\in X}R/\mathcal F_P
\text{ is surjective when }X\text{ is affine};\quad H^1(X,\mathcal F)=0}.
$$

No nonsingularity assumption was used; the construction applies to singular irreducible affine curves as well.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
