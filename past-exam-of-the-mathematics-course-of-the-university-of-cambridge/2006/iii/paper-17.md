# Paper 17

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper17.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper17.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work in the classical setting of [varieties](../../../algebraic-geometry.md#algebraic-variety) over an algebraically closed [field](../../../algebra.md#field) $k$. A prevariety is separated when its [diagonal morphism](../../../ringed-space.md#diagonal-morphism) $\Delta_X:X\to X\times_kX$ is a [closed immersion](../../../ringed-space.md#closed-immersion); for prevarieties the diagonal is already an immersion, so this is equivalent to its image being closed. A [complete variety](../../../ringed-space.md#complete-variety) has the following closed-projection property: for every [variety](../../../algebraic-geometry.md#algebraic-variety) $Y$, projection $X\times_kY\to Y$ maps closed subsets to closed subsets. This is [universal closedness](../../../ringed-space.md#universally-closed-morphism); since a [variety](../../../algebraic-geometry.md#algebraic-variety) is separated and of finite type, it is equivalent to the structural map being [proper](../../../ringed-space.md#proper-morphism).

First consider [projective space](../../../projective-space.md). In two sets of homogeneous coordinates its diagonal is defined by

$$
X_iY_j-X_jY_i=0\qquad(0\le i,j\le n).
$$

These equations hold exactly when the two nonzero coordinate [vectors](../../../vector-space.md#vector) are proportional. They are homogeneous in each coordinate set, so they define a closed subset of $\mathbb P^n\times\mathbb P^n$. On a common [affine chart](../../../ringed-space.md#affine-chart-of-a-variety), the diagonal map is the usual [closed immersion](../../../ringed-space.md#closed-immersion) defined by equality of the affine coordinates. Thus [projective space](../../../projective-space.md) is separated. If $X\hookrightarrow\mathbb P^n$ is a [projective embedding](../../../projective-space.md#projective-embedding), its diagonal is the intersection of that closed diagonal with $X\times X$. Consequently **every [projective variety](../../../projective-space.md#projective-variety) is separated**.

Here is an algebraic proof of completeness, rather than an appeal to projective compactness in an analytic topology. It suffices to prove [closedness of projection from projective space](../../../ringed-space.md#closedness-of-projection-from-projective-space) over an [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) $Y$, with [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $A=k[Y]$. A closed subset $Z\subseteq\mathbb P^n\times Y$ is cut out by a [homogeneous ideal](../../../commutative-algebra.md#homogeneous-ideal) $I\subseteq A[T_0,\ldots,T_n]$. Put $B=A[T_0,\ldots,T_n]/I$ and write $B_d$ for its degree-$d$ part. Each $B_d$ is a finitely generated $A$-module, because it is a quotient of the free [module](../../../module-theory.md#module-mathematics) on the degree-$d$ monomials.

Suppose the fibre over $y\in Y$ is empty. The specialized homogeneous equations then have no nonzero common zero. By the [Hilbert Nullstellensatz](../../../algebraic-geometry.md#hilbert-nullstellensatz), some power of each $T_i$ belongs to the specialized ideal. If those powers are $T_i^{r_i}$, then every monomial of degree $d=1+\sum_i(r_i-1)$ belongs to that ideal. Hence

$$
B_d\otimes_A k(y)=0.
$$

The [Nakayama lemma](../../../mathematics.md#nakayama-lemma) gives $(B_d)_{\mathfrak m_y}=0$. Since $B_d$ is finitely generated, there is $a\in A\setminus\mathfrak m_y$ with $(B_d)_a=0$: choose generators and multiply finitely many elements annihilating their [localizations](../../../commutative-algebra.md#localization-of-a-ring). On the [principal open subset](../../../ringed-space.md#principal-open-subscheme) $D(a)$, all graded pieces of degree at least $d$ vanish too, since the quotient is generated in degree one. Every fibre over $D(a)$ is therefore empty: a projective point would have a nonzero coordinate whose degree-$d$ power could not vanish. Thus the complement of the projection of $Z$ is open, proving the required closed-projection property.

An [affine open cover](../../../topology.md#affine-open-cover) of an arbitrary $Y$ establishes the same result there. Finally, a closed subset of $X\times Y$ is closed in $\mathbb P^n\times Y$ when $X$ is a [projective variety](../../../projective-space.md#projective-variety), so its image is closed by the preceding argument. Therefore

$$
\boxed{\text{Every projective variety is separated and complete.}}
$$

Over a non-algebraically-closed [field](../../../algebra.md#field), the corresponding statement concerns schemes or geometric points. Projection of rational points alone need not be closed, so it must not replace the completeness definition.

## 2

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Form the [presheaf](../../../algebraic-geometry.md#presheaf-of-sets-on-a-topological-space) whose value on $U\subseteq X$ is

$$
\mathcal G(U)\otimes_{\mathcal O_X(U)}\mathcal H(U),
$$

with restrictions induced from those of the two [sheaves of modules](../../../ringed-space.md#sheaf-of-modules) and the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme). Its [sheafification](../../../ringed-space.md#sheafification) is the [tensor product of sheaves](../../../ringed-space.md#tensor-product-of-sheaves) $\mathcal G\otimes_{\mathcal O_X}\mathcal H$. Sheafification is needed because taking a [tensor product](../../../linear-algebra.md#tensor-product) on each [open set](../../../topology.md#open-set) need not itself satisfy the gluing axiom. The resulting [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) represents bilinear [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) morphisms, and [localization](../../../commutative-algebra.md#localization-of-a-ring) gives the [stalk](../../../ringed-space.md#stalk-of-a-sheaf) formula

$$
\boxed{(\mathcal G\otimes_{\mathcal O_X}\mathcal H)_P
\cong\mathcal G_P\otimes_{\mathcal O_{X,P}}\mathcal H_P}.
$$

Indeed, [sheafification](../../../ringed-space.md#sheafification) preserves [stalks](../../../ringed-space.md#stalk-of-a-sheaf), and filtered [direct limits](../../../module-theory.md#direct-limit-of-abelian-groups) commute with the [module](../../../module-theory.md#module-mathematics) [tensor product](../../../linear-algebra.md#tensor-product).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) is defined by

$$
\boxed{(\phi_*\mathcal F)(U)=\mathcal F(\phi^{-1}U)}.
$$

Its restrictions are the restrictions of $\mathcal F$. Inverse images preserve covers and intersections, so the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) holds immediately. The [morphism of ringed spaces](../../../ringed-space.md#morphism-of-ringed-spaces) supplies

$$
\phi^\#:\mathcal O_X(U)\longrightarrow\mathcal O_Y(\phi^{-1}U).
$$

An element of $\mathcal O_X(U)$ acts on the displayed sections through this ring map and the original $\mathcal O_Y$-module action. This makes the [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) an $\mathcal O_X$-module; no additional [sheafification](../../../ringed-space.md#sheafification) is required.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

First form the [inverse image sheaf](../../../ringed-space.md#inverse-image-sheaf) $\phi^{-1}\mathcal H$ by sheafifying the presheaf

$$
V\longmapsto\varinjlim_{U\supseteq\phi(V)}\mathcal H(U),
$$

where $U$ runs through [open subsets](../../../topology.md#open-set) of $X$. It is naturally a [module](../../../module-theory.md#module-mathematics) over $\phi^{-1}\mathcal O_X$, not yet over $\mathcal O_Y$. The structure morphism $\phi^{-1}\mathcal O_X\to\mathcal O_Y$ allows extension of scalars, giving the [pullback of a sheaf of modules](../../../ringed-space.md#pullback-of-a-sheaf-of-modules):

$$
\boxed{\phi^*\mathcal H
=\mathcal O_Y\otimes_{\phi^{-1}\mathcal O_X}\phi^{-1}\mathcal H}.
$$

The [tensor product of sheaves](../../../ringed-space.md#tensor-product-of-sheaves) includes its own [sheafification](../../../ringed-space.md#sheafification). At $Q\in Y$ the construction becomes

$$
(\phi^*\mathcal H)_Q
=\mathcal O_{Y,Q}\otimes_{\mathcal O_{X,\phi(Q)}}\mathcal H_{\phi(Q)}.
$$

This adjustment of the coefficient ring distinguishes the pullback from the underlying [inverse image sheaf](../../../ringed-space.md#inverse-image-sheaf).

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [affine module sheaf](../../../ringed-space.md#affine-module-sheaf) construction makes the remaining statements explicit. For $A=k[V]$ and an $A$-module $M$, define

$$
\widetilde M(D(f))=M_f
$$

on the [basis](../../../vector-space.md#basis) of [principal open subsets](../../../ringed-space.md#principal-open-subscheme). Restrictions are the natural [localization](../../../commutative-algebra.md#localization-of-a-ring) maps. Equivalently, a section on an arbitrary [open set](../../../topology.md#open-set) is a family $s_P\in M_{\mathfrak m_P}$ which near each point is represented by a single fraction $m/f^r$, with $f$ nonvanishing throughout that neighbourhood. This locally representable family construction gives a [sheaf](../../../algebraic-geometry.md#sheaf-mathematics); the usual [localization](../../../commutative-algebra.md#localization-of-a-ring) gluing verifies its [quasi-coherence](../../../ringed-space.md#quasi-coherent-sheaf). Its [stalk](../../../ringed-space.md#stalk-of-a-sheaf) is $M_{\mathfrak m_P}$ and

$$
\boxed{\Gamma(V,\widetilde M)=M}.
$$

This last identification is precisely the standard module-localization gluing on the affine [basis](../../../vector-space.md#basis), not an assertion that arbitrary [sheaves](../../../algebraic-geometry.md#sheaf-mathematics) are determined by their global sections.

Now write $A=k[X]$, $B=k[Y]$ and $\alpha=\phi^\#:A\to B$. Let $\mathcal G=\widetilde M$, $\mathcal H=\widetilde N$ for $A$-modules $M,N$, and let $\mathcal F=\widetilde L$ for a $B$-module $L$. The affine versions of the three constructions are

$$
\boxed{\mathcal G\otimes_{\mathcal O_X}\mathcal H\cong\widetilde{M\otimes_A N},\qquad
\phi_*\mathcal F\cong\widetilde{{}_A L},\qquad
\phi^*\mathcal H\cong\widetilde{B\otimes_A N}}.
$$

Here ${}_A L$ denotes restriction of scalars along $\alpha$, whereas the last associated [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) lives on $Y$. To verify the tensor-product assertion, localize at every prime: both [stalks](../../../ringed-space.md#stalk-of-a-sheaf) are $M_{\mathfrak m}\otimes_{A_{\mathfrak m}}N_{\mathfrak m}$. For the [direct image](../../../ringed-space.md#direct-image-sheaf), $\phi^{-1}D(a)=D(\alpha(a))$, and

$$
\Gamma(D(a),\phi_*\widetilde L)=L_{\alpha(a)}=({}_A L)_a.
$$

These equalities identify the [sheaves](../../../algebraic-geometry.md#sheaf-mathematics) on a [basis](../../../vector-space.md#basis) and respect restrictions. For the [pullback of a sheaf of modules](../../../ringed-space.md#pullback-of-a-sheaf-of-modules), its [stalk](../../../ringed-space.md#stalk-of-a-sheaf) at $Q$ is $B_{\mathfrak m_Q}\otimes_A N$, exactly the [stalk](../../../ringed-space.md#stalk-of-a-sheaf) of $\widetilde{B\otimes_A N}$. The local tensor maps are compatible, so these [stalk](../../../ringed-space.md#stalk-of-a-sheaf) identifications come from an actual [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) isomorphism. Thus all three constructions are [quasi-coherent](../../../ringed-space.md#quasi-coherent-sheaf) in the stated affine setting.

Finally construct the natural [projection formula for sheaves](../../../ringed-space.md#projection-formula) map by sending a local tensor $m\otimes b$ to $b(1\otimes m)$ in the pulled-back [module](../../../module-theory.md#module-mathematics), followed by [direct image](../../../ringed-space.md#direct-image-sheaf). In the affine description, the target $\phi_*\phi^*\widetilde M$ is the [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) associated with the $A$-module ${}_A(B\otimes_A M)$, while $\widetilde M\otimes_{\mathcal O_X}\phi_*\mathcal O_Y$ corresponds to $M\otimes_A B$. The maps

$$
m\otimes b\longmapsto b\otimes m,\qquad b\otimes m\longmapsto m\otimes b
$$

are inverse $A$-linear maps. Localizing them commutes with every restriction, proving

$$
\boxed{\phi_*\phi^*\widetilde M\cong
\widetilde M\otimes_{\mathcal O_X}\phi_*\mathcal O_Y}.
$$

No flatness assumption on $A\to B$ or finiteness assumption on $M$ is needed.

## 3

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [sheaf of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups) $\mathcal F$ on a [topological space](../../../topology.md#topological-space) $X$, put

$$
C(\mathcal F)(U)=\prod_{P\in U}\mathcal F_P.
$$

These arbitrary families of [germs](../../../ringed-space.md#germ-of-a-sheaf-section) form a [sheaf](../../../algebraic-geometry.md#sheaf-mathematics), and restrictions are projections. Extending a family by zero proves that $C(\mathcal F)$ is [flasque](../../../ringed-space.md#flasque-sheaf). Sending a section to all its [germs](../../../ringed-space.md#germ-of-a-sheaf-section) gives an injective [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) map $\mathcal F\to C(\mathcal F)$, since a section with every [germ](../../../ringed-space.md#germ-of-a-sheaf-section) zero vanishes locally and hence globally.

Set $Q^{-1}=\mathcal F$, $I^j=C(Q^{j-1})$ and $Q^j=\operatorname{coker}(Q^{j-1}\to I^j)$, using the [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) [cokernel](../../../linear-algebra.md#cokernel). Compose $I^j\to Q^j\to I^{j+1}$ to obtain the [Godement resolution](../../../ringed-space.md#godement-resolution)

$$
0\longrightarrow\mathcal F\longrightarrow I^0\longrightarrow I^1\longrightarrow\cdots.
$$

It is exact by construction, with [flasque](../../../ringed-space.md#flasque-sheaf) terms. Define [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) by the [cohomology](../../../cohomology.md) of its global-section complex:

$$
H^j(X,\mathcal F)=H^j\bigl(\Gamma(X,I^\bullet)\bigr),\qquad
H^0(X,\mathcal F)=\Gamma(X,\mathcal F).
$$

The [resolution principle for sheaf cohomology](../../../ringed-space.md#resolution-principle-for-sheaf-cohomology) identifies this with the computation using any [flasque resolution](../../../ringed-space.md#flasque-resolution).

The elementary input for acyclicity is the [flasque-kernel section-lifting lemma](../../../ringed-space.md#flasque-kernel-section-lifting-lemma): in a [short exact sequence](../../../module-theory.md#short-exact-sequence) with [flasque](../../../ringed-space.md#flasque-sheaf) kernel, sections of the quotient lift over every [open subset](../../../topology.md#open-set). Consequently a quotient of two [flasque sheaves](../../../ringed-space.md#flasque-sheaf) is [flasque](../../../ringed-space.md#flasque-sheaf), because a quotient section lifts and that lift extends. If $\mathcal F$ itself is [flasque](../../../ringed-space.md#flasque-sheaf), induction through $0\to Q^{j-1}\to I^j\to Q^j\to0$ makes every $Q^j$ [flasque](../../../ringed-space.md#flasque-sheaf). The same lifting lemma makes these sequences exact on [global sections](../../../ringed-space.md#global-section). Hence the global-section complex has no positive-degree [cohomology](../../../cohomology.md), proving

$$
\boxed{H^j(X,\mathcal F)=0\quad(j>0)\text{ for flasque }\mathcal F}.
$$

This deduction uses the lifting lemma, not the desired cohomological vanishing as an assumption.

For the rational-section construction, add two representative sections after restricting to the intersection of their dense domains. Multiply by a representative rational function in the same way. Finite intersections of dense [open sets](../../../topology.md#open-set) are dense, and further restricting both representatives does not change their resulting class. The [module](../../../module-theory.md#module-mathematics) axioms hold on their common domain. Thus [rational sections](../../../ringed-space.md#rational-section-of-a-sheaf-of-modules) form a [module](../../../module-theory.md#module-mathematics) over $\operatorname{Rat}(X)$; irreducibility is not needed for this [module](../../../module-theory.md#module-mathematics) statement. When $X$ is irreducible, $\operatorname{Rat}(X)$ is the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) $K=k(X)$.

Suppose now that $\mathcal F$ is [locally free](../../../ringed-space.md#locally-free-sheaf) and $X$ irreducible. A [germ](../../../ringed-space.md#germ-of-a-sheaf-section) at $P$ is represented on a nonempty open neighbourhood, which is dense, so it defines a [rational section](../../../ringed-space.md#rational-section-of-a-sheaf-of-modules). Two representatives of the [germ](../../../ringed-space.md#germ-of-a-sheaf-section) agree on a neighbourhood of $P$ and therefore give the same class. If the class is zero, trivialize $\mathcal F$ on a neighbourhood of $P$. Its coefficient functions vanish on a dense [open subset](../../../topology.md#open-set); [regular functions](../../../ringed-space.md#regular-function) on a reduced [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) with this property vanish identically. The [germ](../../../ringed-space.md#germ-of-a-sheaf-section) is therefore zero. This proves the [stalk inclusion into rational sections of a locally free sheaf](../../../ringed-space.md#stalk-inclusion-into-rational-sections-of-a-locally-free-sheaf):

$$
\boxed{\mathcal F_P\hookrightarrow\operatorname{Rat}(\mathcal F)}.
$$

Local freeness matters: a nonzero torsion [germ](../../../ringed-space.md#germ-of-a-sheaf-section) can vanish on a dense [open set](../../../topology.md#open-set).

On an irreducible [algebraic curve](../../../algebraic-geometry.md#algebraic-curve), every proper closed subset is finite, and every [open subset](../../../topology.md#open-set) is [quasi-compact](../../../topology.md#compact-space) because the Zariski space is [Noetherian](../../../algebra.md#noetherian-ring). Let $R=\operatorname{Rat}(\mathcal F)$. The [constant sheaf](../../../algebraic-geometry.md#constant-sheaf) $\mathcal R(\mathcal F)$ has sections $R$ on every nonempty [open set](../../../topology.md#open-set): such opens are irreducible and hence connected. Define

$$
\mathcal P(\mathcal F)(U)=\bigoplus_{P\in U}R/\mathcal F_P.
$$

Restriction drops the components outside the smaller [open set](../../../topology.md#open-set). For a compatible family over an open cover of $U$, take a finite subcover by quasi-compactness. The union of the finite supports of these finitely many sections is finite. Their agreeing components therefore glue to a unique finite-support tuple on $U$. This verifies the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom), including arbitrary covers, rather than merely asserting that a presheaf direct sum is always a [sheaf](../../../algebraic-geometry.md#sheaf-mathematics).

A [rational section](../../../ringed-space.md#rational-section-of-a-sheaf-of-modules) is regular on some dense [open set](../../../topology.md#open-set), whose complement on a curve is finite. Its classes $[s]_P\in R/\mathcal F_P$ therefore have finite support, defining a [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) map $\mathcal R(\mathcal F)\to\mathcal P(\mathcal F)$. At $P$, the first [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) has [stalk](../../../ringed-space.md#stalk-of-a-sheaf) $R$. The second has [stalk](../../../ringed-space.md#stalk-of-a-sheaf) $R/\mathcal F_P$: any finite tuple can be restricted to a neighbourhood omitting all its other support points, and its $P$-component is unaffected by such restriction. The resulting sequence on [stalks](../../../ringed-space.md#stalk-of-a-sheaf) is

$$
0\to\mathcal F_P\to R\to R/\mathcal F_P\to0.
$$

Exactness of [sheaves](../../../algebraic-geometry.md#sheaf-mathematics) can be tested on [stalks](../../../ringed-space.md#stalk-of-a-sheaf), so this proves the [rational principal-parts resolution on an algebraic curve](../../../ringed-space.md#rational-principal-parts-resolution-on-an-algebraic-curve)

$$
\boxed{0\to\mathcal F\to\mathcal R(\mathcal F)\to\mathcal P(\mathcal F)\to0}.
$$

Both right-hand [sheaves](../../../algebraic-geometry.md#sheaf-mathematics) are [flasque](../../../ringed-space.md#flasque-sheaf): restrictions for the constant rational-section [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) are identities between nonempty opens, and restrictions for the rational principal-parts [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) are projections, with extension by zero. Consequently

$$
H^1(X,\mathcal F)\cong
\operatorname{coker}\left(R\to\bigoplus_{P\in X}R/\mathcal F_P\right),\qquad
H^j(X,\mathcal F)=0\quad(j\ge2).
$$

Surjectivity on [stalks](../../../ringed-space.md#stalk-of-a-sheaf) has not been confused with surjectivity on global sections.

For an explicit failure of global surjectivity take $X=\mathbb P^1$ and $\mathcal F=\mathcal O(-2)$. Use coordinate $z=X_1/X_0$ and frame $e_0=X_0^{-2}$ on the finite chart. At infinity use $w=1/z$ and $e_\infty=X_1^{-2}=z^{-2}e_0$. Prescribe the [rational principal part](../../../ringed-space.md#rational-principal-part) of $z^{-1}e_0$ at zero and zero at every other point. If a [rational section](../../../ringed-space.md#rational-section-of-a-sheaf-of-modules) $r(z)e_0$ realized this tuple, then $r-z^{-1}$ would be regular at zero and $r$ would be regular at every other finite point. Thus $r=z^{-1}+p(z)$ with $p\in k[z]$. Regularity at infinity would require

$$
z^2r(z)=w^{-1}+w^{-2}p(w^{-1})
$$

to be regular at $w=0$. Its $w^{-1}$ term cannot cancel with any term of the [polynomial](../../../polynomial.md) contribution, whose powers are at most $-2$. This is impossible. Hence **the global rational-principal-part map need not be surjective**.

For an affine curve it is always surjective, and here is a direct construction. Write $X=\operatorname{Spec}A$, $K=\operatorname{Frac}A$ and $\mathcal F=\widetilde M$. By the [affine module sheaf](../../../ringed-space.md#affine-module-sheaf) construction, $R=M\otimes_AK=:M_K$ and $\mathcal F_P=M_{\mathfrak m_P}$. Choose representatives $v_P\in M_K$ for a prescribed finite tuple, and choose one nonzero $a\in A$ with $av_P\in M$ for all of them. The zero set $T=V(a)$ is finite. The ring $A/(a)$ is [Artinian](../../../algebra.md#artinian-ring), since it is Noetherian of dimension zero, and its [Artinian decomposition into local factors](../../../algebra.md#artinian-decomposition-into-local-factors) gives

$$
M/aM\cong\bigoplus_{P\in T}(M/aM)_{\mathfrak m_P}.
$$

Prescribe the class of $av_P$ in the indicated component for each requested point in $T$, and zero in the other components. A requested point outside $T$ already has zero principal part because $a$ is a unit there. Lift the tuple to $w\in M$. Then $s=w/a\in M_K$ satisfies $s-v_P\in M_{\mathfrak m_P}$ at every requested point in $T$, and is regular at every other point of $T$. Outside $T$ it is regular because $a$ is invertible. It therefore realizes exactly the prescribed tuple. This proves [affine principal-parts interpolation for a locally free sheaf](../../../ringed-space.md#affine-principal-parts-interpolation-for-a-locally-free-sheaf) and gives

$$
\boxed{R\longrightarrow\bigoplus_{P\in X}R/\mathcal F_P
\text{ is surjective when }X\text{ is affine};\quad H^1(X,\mathcal F)=0}.
$$

No nonsingularity assumption was used; the construction applies to singular irreducible affine curves as well.

## 4

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

On the standard [affine charts](../../../ringed-space.md#affine-chart-of-a-variety) $U_i=\{X_i\ne0\}$, use the formal frame $e_i=X_i^m$ and glue rank-one free [sheaves](../../../algebraic-geometry.md#sheaf-mathematics) by

$$
e_j=(X_j/X_i)^m e_i.
$$

The transition functions are regular units on overlaps and satisfy the [cocycle](../../../algebra.md#cocycle) identity. This constructs the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) $\mathcal O(m)$ as an [invertible sheaf](../../../ringed-space.md#line-bundle) for every integer $m$, including negative $m$.

On a nonempty $U$, a section has local expressions $h_i e_i$, where $h_i\in\mathcal O(U\cap U_i)$. Pulling to the punctured affine cone gives $h_i(X/X_i)X_i^m$. Their agreement on overlaps makes them one homogeneous rational function $r$ of degree $m$, regular on $\pi^{-1}U$. To make its [polynomial](../../../polynomial.md) representation explicit, write one nonzero local coefficient as $p(y)/q(y)$ in the affine coordinates. Homogenize $p,q$ to degrees $a,b$; the resulting rational expression is

$$
r=X_i^{m-a+b}\frac{p^{\mathrm{hom}}}{q^{\mathrm{hom}}}.
$$

If the exponent of $X_i$ is negative, move its power to the denominator. Cancel common factors; the greatest common divisor of [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) can be chosen homogeneous. Thus $r=F/G$ with $F,G$ coprime [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial), $G\ne0$, and $\deg F-\deg G=m$.

Conversely, for such a homogeneous rational function regular on $\pi^{-1}U$, its coefficient $r/X_i^m$ is regular on $U\cap U_i$: restrict to the slice $X_i=1$. These coefficients obey the displayed transition rule and hence define a section. This proves the [homogeneous rational sections of a twisting sheaf](../../../ringed-space.md#homogeneous-rational-sections-of-a-twisting-sheaf) description in both directions, for arbitrary open $U$ rather than only a standard chart.

Now lift a regular degree-zero rational function $f=P/Q$ to the punctured cone. The quotient rule gives

$$
\frac{\partial f}{\partial X_i}=\frac{Q\,\partial_iP-P\,\partial_iQ}{Q^2}.
$$

This is a rational function homogeneous of degree $-1$. It is independent of the chosen representation because differentiation is a [derivation](../../../associative-algebra.md#derivation-of-an-algebra) of the rational [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety). It is regular wherever $f$ is regular: a derivation of a [polynomial](../../../polynomial.md) ring extends to each [localization](../../../commutative-algebra.md#localization-of-a-ring) by the quotient rule, and [regular functions](../../../ringed-space.md#regular-function) are locally such fractions. The preceding homogeneous-section description therefore proves

$$
\boxed{\partial_i f\in\Gamma(U,\mathcal O(-1))}.
$$

Zeros of a particular displayed denominator do not invalidate this argument; regularity is a property of the rational function, which can have another local representation.

The map $f\mapsto(\partial_0f,\ldots,\partial_nf)$ is a $k$-linear [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) derivation with values in $\mathcal O(-1)^{\oplus(n+1)}$. The [universal property of Kähler differentials](../../../ringed-space.md#universal-property-of-kahler-differentials) consequently defines

$$
D:\Omega^1_{\mathbb P^n}\longrightarrow\mathcal O(-1)^{\oplus(n+1)},\qquad
df\longmapsto(\partial_i f)_i.
$$

Multiplication by the coordinate section $X_i\in\Gamma(\mathbb P^n,\mathcal O(1))$ defines the other map

$$
\sigma:\mathcal O(-1)^{\oplus(n+1)}\longrightarrow\mathcal O,\qquad
(g_i)_i\longmapsto\sum_iX_i g_i.
$$

For a degree-$d$ homogeneous polynomial, differentiating each monomial gives $\sum_iX_i\partial_iP=dP$. Applying this to the equal-degree numerator and denominator gives $\sum_iX_i\partial_i f=0$ for degree-zero $f$, so $\sigma D=0$. This identity is valid in every characteristic.

To prove all the exactness assertions, fix $U_i$ and put $y_j=X_j/X_i$ for $j\ne i$. The [Kähler differential sheaf](../../../ringed-space.md#sheaf-of-kahler-differentials-over-a-field) is free there on $dy_j$, because a derivation of the polynomial ring is determined freely by its values on the coordinates. Trivialize each $\mathcal O(-1)$ with frame $X_i^{-1}$. In this frame,

$$
D(dy_j)=e_j-y_je_i,\qquad
\sigma((b_0,\ldots,b_n))=b_i+\sum_{j\ne i}y_jb_j,
$$

where $e_j$ now denotes the $j$th coordinate [vector](../../../vector-space.md#vector) of the direct sum. The map $\sigma$ is surjective, since its $i$th coefficient is one. Its kernel consists exactly of tuples with $b_i=-\sum_{j\ne i}y_jb_j$, so the $n$ displayed [vectors](../../../vector-space.md#vector) $e_j-y_je_i$ form a free [basis](../../../vector-space.md#basis) of that kernel. The map $D$ sends the differential [basis](../../../vector-space.md#basis) bijectively to this kernel [basis](../../../vector-space.md#basis) and is therefore injective. Exactness on these charts proves the [cotangent Euler sequence in homogeneous coordinates](../../../algebraic-geometry.md#cotangent-euler-sequence-in-homogeneous-coordinates)

$$
\boxed{0\to\Omega^1_{\mathbb P^n}\xrightarrow{D}
\mathcal O(-1)^{\oplus(n+1)}\xrightarrow{\sigma}\mathcal O\to0}.
$$

The proof uses no division by an integer and hence no characteristic-zero assumption.

For $n\ge1$, the [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space) gives

$$
h^q(\mathbb P^n,\mathcal O(m))=
\begin{cases}
\binom{m+n}{n},&q=0,\ m\ge0,\\
\binom{-m-1}{n},&q=n,\ m\le-n-1,\\
0,&\text{otherwise}.
\end{cases}
$$

In particular, $H^0(\mathcal O)=k$, $H^{q>0}(\mathcal O)=0$, and $H^q(\mathcal O(-1))=0$ for every $q$. The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) of the displayed [Euler sequence](../../../algebraic-geometry.md#euler-sequence) begins

$$
0\to H^0(\Omega^1)\to0\to k\to H^1(\Omega^1)\to0,
$$

and gives zero in the remaining degrees. Thus

$$
\boxed{\dim_k H^q(\mathbb P^n,\Omega^1_{\mathbb P^n})=
\begin{cases}1,&q=1,\\0,&q\ne1,\end{cases}\qquad(0\le q\le n,\ n\ge1)}.
$$

The nonzero group is generated by the connecting image of the section $1$ of $\mathcal O$. If $n=0$ is admitted, $\mathbb P^0$ is a point and its cotangent [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) is zero, so the sole requested group $H^0$ is zero.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
