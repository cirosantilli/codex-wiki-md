# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper4.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $A=RG$. An [idempotent](../../../commutative-algebra.md#idempotent) is an element $e$ with $e^2=e$; it is [central idempotent](../../../associative-algebra.md#central-idempotent) when it commutes with every element of the [ring](../../../commutative-algebra.md#ring). In a commutative [ring](../../../commutative-algebra.md#ring) centrality is automatic. Two [idempotents](../../../commutative-algebra.md#idempotent) are [orthogonal idempotents](../../../commutative-algebra.md#orthogonal-idempotent) if $ef=fe=0$. A nonzero [primitive central idempotent](../../../associative-algebra.md#primitive-central-idempotent) cannot be expressed as the sum of two nonzero orthogonal [central idempotents](../../../associative-algebra.md#central-idempotent); this is primitivity in $Z(A)$, not necessarily primitivity in $A$.

A [block of a group algebra](../../../representation-theory.md#block-of-a-group-algebra) is an indecomposable two-sided direct-summand [ideal](../../../commutative-algebra.md#ideal) of $A$, equivalently an [ideal](../../../commutative-algebra.md#ideal) $Ae$ with $e$ a [primitive central idempotent](../../../associative-algebra.md#primitive-central-idempotent). Here is the equivalence. If $A=B\oplus C$ as two-sided [ideals](../../../commutative-algebra.md#ideal), then $BC=CB=0$. Write $1=e+f$ with $e\in B,f\in C$. Multiplication by this equality shows that $e$ is the identity of $B$, that $f$ is the identity of $C$, and that $e,f$ are orthogonal [central idempotents](../../../associative-algebra.md#central-idempotent). Conversely a [central idempotent](../../../associative-algebra.md#central-idempotent) gives $A=Ae\oplus A(1-e)$. Splitting the [ideal](../../../commutative-algebra.md#ideal) further is therefore equivalent to splitting its [central idempotent](../../../associative-algebra.md#central-idempotent) further.

For uniqueness, suppose $1=\sum_i e_i=\sum_j f_j$ are decompositions into [primitive central idempotents](../../../associative-algebra.md#primitive-central-idempotent). For each $i$,

$$
e_i=\sum_j e_if_j
$$

is an orthogonal central-idempotent decomposition. Exactly one summand is nonzero, and that summand equals $e_i$. Applying the same reasoning to the corresponding $f_j$ gives $e_i=f_j$. Thus **the blocks, and their identities, are unique up to ordering**. Existence in the paper's coefficient [rings](../../../commutative-algebra.md#ring) follows from finite-dimensionality over $k$, and over $\mathcal O$ from completeness and [idempotent lifting](../../../commutative-algebra.md#idempotent-lifting) of the decomposition modulo its maximal [ideal](../../../commutative-algebra.md#ideal).

Over $k$, a [principal indecomposable module](../../../module-theory.md#principal-indecomposable-module) is an indecomposable summand of the regular left [module](../../../module-theory.md#module-mathematics) $A=kG$, equivalently $P=Ae$ for a [primitive idempotent](../../../commutative-algebra.md#primitive-idempotent) $e$ of $A$. Put $J=J(A)$, the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical). The [head of a module](../../../module-theory.md#head-of-a-module) $P/JP$ is nonzero and semisimple. It is simple: projectivity gives a surjection

$$
\operatorname{End}_A(P)\longrightarrow\operatorname{End}_{A/J}(P/JP),
$$

whose kernel consists of maps into $JP$ and is nilpotent, since a product of $r$ such maps sends $P$ into $J^rP$. If the [head of a module](../../../module-theory.md#head-of-a-module) split, a nontrivial projection on it would lift by [idempotent lifting](../../../commutative-algebra.md#idempotent-lifting) to a nontrivial projection on $P$, contradicting indecomposability. Every maximal submodule contains $JP$, since $J$ annihilates simple [modules](../../../module-theory.md#module-mathematics). The simplicity of the [head of a module](../../../module-theory.md#head-of-a-module) now proves **$J(P)=JP$ is the unique maximal submodule**, and $P$ is its [head of a module](../../../module-theory.md#head-of-a-module)'s [projective cover](../../../module-theory.md#projective-cover).

Choose the simple [modules](../../../module-theory.md#module-mathematics) $S_1,\ldots,S_r$, with corresponding [projective covers](../../../module-theory.md#projective-cover) $P_1,\ldots,P_r$. Our convention for the [Cartan matrix of a group algebra](../../../representation-theory.md#cartan-matrix-of-a-group-algebra) is

$$
\boxed{(C_G)_{ij}=[P_j:S_i],}
$$

where brackets denote the multiplicity in a [composition series](../../../finite-group-theory.md#composition-series).

For the final two unheaded requests, retain the additional hypothesis $G=NC_G(N)$. Choose a central [subgroup](../../../group.md#subgroup) $Z=\langle z\rangle$ of $N$ of order $p$. Every element of $N$ centralizes $Z$, and so does every element of $C_G(N)$; hence $Z\le Z(G)$. Set $t=z-1$, so $t$ is central and $t^p=0$, and $A/tA\cong k(G/Z)$.

To lift a [central idempotent](../../../associative-algebra.md#central-idempotent) $\bar e$ of this quotient, first lift it as an [idempotent](../../../commutative-algebra.md#idempotent) $e$ by [idempotent refinement theorem](../../../commutative-algebra.md#idempotent-refinement-theorem). Since $\bar e$ is central, $eA(1-e)\subseteq tA$. Multiplying a representation $e a(1-e)=t b$ on the left and right by $e,1-e$ gives

$$
eA(1-e)\subseteq t eA(1-e)\subseteq\cdots\subseteq t^p eA(1-e)=0.
$$

The other off-diagonal corner vanishes likewise, so $e$ is central. Two central lifts of the same [idempotent](../../../commutative-algebra.md#idempotent) coincide: their mismatched products $e(1-f)$ and $f(1-e)$ are [idempotents](../../../commutative-algebra.md#idempotent) in the nilpotent kernel and therefore zero. Primitivity is preserved because orthogonal [idempotent](../../../commutative-algebra.md#idempotent) decompositions lift. Thus the central $p$-quotient gives a bijection of block [idempotents](../../../commutative-algebra.md#idempotent).

The quotient $G/Z$ still satisfies the required hypothesis for $N/Z$, because the image of $C_G(N)$ centralizes $N/Z$. Induction on $|N|$ therefore proves **$\tau$ bijects the block [idempotents](../../../commutative-algebra.md#idempotent) of $kG$ and $k(G/N)$**. The centrality argument is essential: a general nilpotent [algebra](../../../algebra.md) quotient need not give a bijection of central block [idempotents](../../../commutative-algebra.md#idempotent).

For the [Cartan matrix of a group algebra](../../../representation-theory.md#cartan-matrix-of-a-group-algebra), every projective $A$-module is free over $kZ$: $A$ is free over $kZ$, a projective $A$-module is a summand of a finite free $A$-module, and finite projectives over the [local ring](../../../commutative-algebra.md#local-ring) $kZ\cong k[t]/(t^p)$ are free. If $P$ is a [principal indecomposable module](../../../module-theory.md#principal-indecomposable-module), $\bar P=P/tP$ is a [principal indecomposable module](../../../module-theory.md#principal-indecomposable-module) over $A/tA$: an [idempotent](../../../commutative-algebra.md#idempotent) splitting of its [endomorphism ring](../../../module-theory.md#endomorphism-ring) would lift and split $P$. The $p$ quotients of its filtration

$$
P\supset tP\supset\cdots\supset t^{p-1}P\supset0
$$

are all isomorphic to $\bar P$ as $k(G/Z)$-modules, by multiplication by the corresponding power of $t$. All simple [modules](../../../module-theory.md#module-mathematics) are annihilated by the [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal) $tA$. Hence $[P:S]=p[\bar P:S]$, with the natural indexing of simple [modules](../../../module-theory.md#module-mathematics), and $C_G=pC_{G/Z}$. Iterating over $N$ gives

$$
\boxed{C_G=|N|C_{G/N}.}
$$

This is [blocks and Cartan matrices under central p-quotients](../../../representation-theory.md#blocks-and-cartan-matrices-under-central-p-quotients). The extra hypothesis is still in force: for example $N=C_3\trianglelefteq S_3$ in characteristic three does not satisfy it, and its [Group algebra Cartan matrix](../../../representation-theory.md#cartan-matrix-of-a-group-algebra) is $\left(\begin{smallmatrix}2&1\\1&2\end{smallmatrix}\right)$ rather than $3I$.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $I$ be the [augmentation ideal](../../../commutative-algebra.md#augmentation-ideal) of $kN$, generated by the elements $n-1$. First prove its nilpotence. A nontrivial finite $p$-group has a central element $z$ of order $p$. Put $t=z-1$. In characteristic $p$, $t^p=z^p-1=0$, and

$$
kN/tkN\cong k(N/\langle z\rangle).
$$

Induction on $|N|$ says that the image of $I$ in this smaller [group algebra](../../../associative-algebra.md#group-algebra) is nilpotent. Thus $I^m\subseteq tkN$ for some $m$, and $I^{mp}\subseteq t^pkN=0$. The trivial [group](../../../group.md) starts the induction. This proves [nilpotence of a p-group augmentation ideal](../../../commutative-algebra.md#nilpotence-of-a-p-group-augmentation-ideal).

The quotient homomorphism kills exactly the differences of elements in each $N$-coset, so

$$
\ker\tau=I kG=kG I.
$$

Normality of $N$ makes $I$ stable under conjugation by $G$. Moving [group](../../../group.md) elements past factors from $I$ therefore gives $(I kG)^r=I^r kG$. Consequently

$$
\boxed{\ker\tau\text{ is a nilpotent ideal of }kG.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Partition the [conjugacy class](../../../group-theory.md#conjugacy-class) into its orbits under conjugation by $N$. Since none of its elements centralizes $N$, each orbit has size $[N:C_N(x)]>1$, a power of $p$. All elements of such an orbit have the same image in $G/N$, because conjugation by an element of $N$ does not alter an $N$-coset. Its orbit sum therefore has image

$$
[N:C_N(x)]\,\tau(x)=0
$$

in characteristic $p$. Summing over the orbits proves **$[\mathcal C]\in\ker\tau$**. This does not require $G=NC_G(N)$; that additional assumption is used in the block and Cartan conclusions proved in the root Solution.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the usual [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem) setting, in which indecomposable summands have local [endomorphism rings](../../../module-theory.md#endomorphism-ring); the paper's [rings](../../../commutative-algebra.md#ring) $\mathcal O,k$ satisfy it for the [subgroups](../../../group.md#subgroup) involved. The [relative projective module](../../../representation-theory.md#relative-projective-module) condition for $H$ means that $M$ is a [direct summand](../../../vector-space.md#direct-summand) of a [module](../../../module-theory.md#module-mathematics) induced from $H$, equivalently, $M$ is a summand of $\operatorname{Ind}_H^G\operatorname{Res}_H^G M$. A [vertex of an indecomposable module](../../../representation-theory.md#vertex-of-an-indecomposable-module) is an inclusion-minimal such [subgroup](../../../group.md#subgroup). A [source of an indecomposable module](../../../representation-theory.md#source-of-an-indecomposable-module) at its [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$ is an indecomposable $RD$-summand $S$ of $M\downarrow_D$ such that $M\mid S\uparrow^G$.

Existence of a [module source](../../../representation-theory.md#source-of-an-indecomposable-module) follows by decomposing $M\downarrow_D$ and using [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem) on the induced decomposition: the indecomposable summand $M$ must occur in the induction of one indecomposable summand $S$. Such $S$ has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$ as a $D$-module, since relative projectivity of $S$ for a proper [subgroup](../../../group.md#subgroup) would make $M$ relatively projective for that [subgroup](../../../group.md#subgroup).

In the paper's modular coefficient [rings](../../../commutative-algebra.md#ring), an [indecomposable module](../../../module-theory.md#indecomposable-module) is a [trivial source module](../../../representation-theory.md#trivial-source-module) when its [module source](../../../representation-theory.md#source-of-an-indecomposable-module) is the rank-one trivial [module](../../../module-theory.md#module-mathematics) $R$ of its [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module). It is then a summand of $R[G/D]$, a [permutation module](../../../representation-theory.md#permutation-module). Conversely suppose $M$ is an indecomposable summand of a [permutation module](../../../representation-theory.md#permutation-module). Restriction to a [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$ is a sum of [modules](../../../module-theory.md#module-mathematics) $R[D/E]$, one for each $D$-orbit of the permutation basis. For a $p$-group $D$, each transitive [permutation module](../../../representation-theory.md#permutation-module) is indecomposable: over $k$ it has simple [head of a module](../../../module-theory.md#head-of-a-module) over the [local ring](../../../commutative-algebra.md#local-ring) $kD$, and over $\mathcal O$ a nontrivial splitting would give a nontrivial splitting after reduction. A [module source](../../../representation-theory.md#source-of-an-indecomposable-module) $S$ must be one of these summands by [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem). Its [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) is $D$, whereas $R[D/E]$ is relatively $E$-projective. Thus $E=D$, and $S\cong R$. Therefore **trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) is equivalent to being an indecomposable permutation-module summand**.

The rank-one formulation uses the paper's coefficient [rings](../../../commutative-algebra.md#ring). If the earlier general coefficient-ring wording were applied to a disconnected [ring](../../../commutative-algebra.md#ring), it would need qualification: for $R=k\times k$ and $G=1$, $(k,0)$ is an indecomposable summand of the [permutation module](../../../representation-theory.md#permutation-module) $R$, but is not the rank-one trivial [module](../../../module-theory.md#module-mathematics) $R$. One can instead allow indecomposable summands of the trivial coefficient [module](../../../module-theory.md#module-mathematics) as [module sources](../../../representation-theory.md#source-of-an-indecomposable-module) in that generality.

For the homomorphism request, take $M_i=\mathcal O[G/H_i]$. [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity) and [Mackey decomposition](../../../representation-theory.md#mackey-restriction-formula) give

$$
\begin{aligned}
\operatorname{Hom}_{\mathcal OG}(M_1,M_2)
&\cong (\mathcal O[G/H_2])^{H_1}\\
&\cong\bigoplus_{g\in H_1\backslash G/H_2}\mathcal O.
\end{aligned}
$$

The summand for $g$ is generated by the sum of the cosets in the $H_1$-orbit of $gH_2$. The identical orbit-sum construction over $k$ gives one copy of $k$ per [double coset](../../../group-theory.md#double-coset). These are free bases in both characteristics, since invariance means coefficients are constant on orbits, with no division by orbit size. Hence

$$
\boxed{\operatorname{Hom}_{\mathcal OG}(M_1,M_2)\twoheadrightarrow
\operatorname{Hom}_{kG}(\bar M_1,\bar M_2).}
$$

The same argument applies to [direct sums](../../../vector-space.md#direct-sum) of coset [permutation modules](../../../representation-theory.md#permutation-module).

If $M$ is a trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) $kG$-module, choose a permutation lattice $X$ with $M\mid\bar X$. Its projection is an [idempotent](../../../commutative-algebra.md#idempotent) $f\in\operatorname{End}_{kG}(\bar X)$. The endomorphism reduction is surjective by the preceding calculation. Its kernel is $\mathfrak p\operatorname{End}_{\mathcal OG}(X)$, and the endomorphism [algebra](../../../algebra.md) is complete over $\mathcal O$. By [idempotent refinement theorem](../../../commutative-algebra.md#idempotent-refinement-theorem), $f$ lifts to an [idempotent](../../../commutative-algebra.md#idempotent) $\hat f$. The lattice $\hat fX$ is a permutation-module summand, hence a trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) lattice, and reduces to $M$.

To prove uniqueness within the class of trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) lattices, let $L,L'$ be two such lifts. They are summands of permutation lattices. Lift a modular isomorphism and its inverse between them by the same homomorphism-surjectivity argument, inserting the summand projections on either side. The lifted composites are identity modulo $\mathfrak p$ and therefore invertible over $\mathcal O$, by [Nakayama lemma](../../../mathematics.md#nakayama-lemma) or the determinant criterion. The lifted maps are consequently inverse up to an invertible composite and give $L\cong L'$. Thus **each trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) [module](../../../module-theory.md#module-mathematics) has a unique trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) lift up to isomorphism**. This is [permutation homomorphisms lift through modular reduction](../../../representation-theory.md#permutation-homomorphisms-lift-through-modular-reduction); uniqueness is not claimed among arbitrary lattice lifts.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $D,E$ be [module vertices](../../../representation-theory.md#vertex-of-an-indecomposable-module) of $M$, and choose a [module](../../../module-theory.md#module-mathematics) $T$ such that $M\mid\operatorname{Ind}_E^G T$. Relative $D$-projectivity then gives

$$
M\mid\operatorname{Ind}_D^G\operatorname{Res}_D^G\operatorname{Ind}_E^G T.
$$

Apply [Mackey decomposition](../../../representation-theory.md#mackey-restriction-formula) to the inner restriction and use induction transitivity. The resulting [module](../../../module-theory.md#module-mathematics) is a [direct sum](../../../vector-space.md#direct-sum) of [modules](../../../module-theory.md#module-mathematics) induced to $G$ from [subgroups](../../../group.md#subgroup) $D\cap{}^gE$, for representatives $g\in D\backslash G/E$. By [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem), the [indecomposable module](../../../module-theory.md#indecomposable-module) $M$ is a summand of one of these [induced representations](../../../representation-theory.md#induced-representation). It is therefore relatively projective for one intersection contained in $D$. Minimality of $D$ forces $D=D\cap{}^gE$, so $D\le{}^gE$.

Interchanging $D,E$ gives $E\le{}^hD$ for some $h$. The two inclusions force equal orders, and hence

$$
\boxed{D={}^gE.}
$$

Thus all [vertices of an indecomposable module](../../../representation-theory.md#vertex-of-an-indecomposable-module) are conjugate in $G$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $S,T$ be [module sources](../../../representation-theory.md#source-of-an-indecomposable-module) at $D$. Since $S\mid M\downarrow_D$ and $M\mid T\uparrow^G$, [Mackey decomposition](../../../representation-theory.md#mackey-restriction-formula) gives

$$
S\mid\operatorname{Res}_D^G\operatorname{Ind}_D^G T
\cong\bigoplus_{g\in D\backslash G/D}
\operatorname{Ind}_{D\cap{}^gD}^D
\operatorname{Res}_{D\cap{}^gD}^{{}^gD}({}^gT).
$$

The [module source](../../../representation-theory.md#source-of-an-indecomposable-module) $S$ has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$. By [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem) it is a summand of one term, and minimality of its [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) forces $D\cap{}^gD=D$. As both [subgroups](../../../group.md#subgroup) have order $|D|$, $g\in N_G(D)$. The corresponding term is simply ${}^gT$, which is indecomposable. Thus

$$
\boxed{S\cong{}^gT\quad\text{for some }g\in N_G(D).}
$$

This proves conjugacy of [sources of an indecomposable module](../../../representation-theory.md#source-of-an-indecomposable-module) at the specified [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Choose a Sylow $p$-subgroup $P$ of a [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$. Its index $[D:P]$ divides the $p'$-part of $|G|$, so it is a unit in $R$ under the hypothesis. For every $RD$-module $U$, the induction counit from $P$ splits by averaging: equivalently, the [relative trace](../../../representation-theory.md#relative-trace) satisfies

$$
\operatorname{Tr}_P^D\left(\frac{\operatorname{id}_U}{[D:P]}\right)=\operatorname{id}_U.
$$

The [D. Higman criterion](../../../representation-theory.md#d-higman-criterion) therefore makes every $RD$-module relatively $P$-projective. Since $M$ is relatively $D$-projective, transitivity of induction makes it relatively $P$-projective. Minimality of the [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) now forces $D=P$. Thus **every [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) is a $p$-subgroup**.

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $q=p^n$ and choose a generator $h$ of $H$. In characteristic $p$, $(h-1)^q=h^q-1=0$, so

$$
kH\cong k[t]/(t^q),\qquad t=h-1.
$$

A [module](../../../module-theory.md#module-mathematics) is a vector space with a [nilpotent operator](../../../linear-operator-theory.md#nilpotent-linear-map) $t$ whose nilpotence index is at most $q$. The nilpotent [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form), valid over every [field](../../../algebra.md#field), splits it into Jordan blocks. One block of size $i$ is

$$
\boxed{V_i=k[t]/(t^i),\qquad1\le i\le q.}
$$

It is indecomposable: its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is $k[t]/(t^i)$, a [local ring](../../../commutative-algebra.md#local-ring) with no nontrivial [idempotents](../../../commutative-algebra.md#idempotent). Distinct $i$ have distinct dimensions. Conversely a [direct sum](../../../vector-space.md#direct-sum) of at least two Jordan blocks is decomposable. Thus there are exactly $q$ indecomposable isomorphism classes.

A homomorphism $V_i\to V_j$ is determined by the image of $1$, which can be any element of $V_j$ annihilated by $t^i$. If $i\ge j$ this is all of $V_j$, of dimension $j$; if $i<j$ it is the span of $t^{j-i},\ldots,t^{j-1}$, of dimension $i$. Hence

$$
\boxed{\dim_k\operatorname{Hom}_{kH}(V_i,V_j)=\min(i,j).}
$$

This realizes the [indecomposable modules for a cyclic p-group](../../../representation-theory.md#indecomposable-modules-for-a-cyclic-p-group).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For generators $g,h$ of $P$, write $x=g-1$, $y=h-1$. Then

$$
kP\cong k[x,y]/(x^p,y^p).
$$

For each $\lambda\in k$, define a two-dimensional [module](../../../module-theory.md#module-mathematics) $M_\lambda$ on basis $v,w$ by $xv=w$, $xw=0$, $yv=\lambda w$, $yw=0$. Every product of two of these operators is zero, so the defining relations hold even when $p=2$.

The action of $x$ is one nonzero nilpotent Jordan block. A decomposition of $M_\lambda$ would decompose its restriction to $k[x]/(x^p)$, which is already indecomposable. Thus $M_\lambda$ is indecomposable. An isomorphism $F:M_\lambda\to M_\mu$ commutes with $x$ and $y$, and consequently

$$
\lambda Fx=Fy=yF=\mu xF=\mu Fx.
$$

Since $F$ is invertible and $x\ne0$, $\lambda=\mu$. The infinite [field](../../../algebra.md#field) supplies infinitely many parameters, proving **$kP$ has infinite representation type**. This is the [parameter family for an elementary abelian p-group](../../../representation-theory.md#parameter-family-for-an-elementary-abelian-p-group).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $B=kGe$ have defect [group](../../../group.md) $D$. Use two vertex-and-source facts, with their relevant content made explicit. Every [indecomposable module](../../../module-theory.md#indecomposable-module) in $B$ has a [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) conjugate into $D$. Also $B$, as a $k[G\times G]$-module with $(g,h)a=gah^{-1}$, is an indecomposable permutation-module summand with [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $\Delta D=\{(d,d):d\in D\}$ and trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module). The second fact is the bimodule characterization of a [defect group of a block](../../../representation-theory.md#defect-group-of-a-block); the first follows by applying its relative-$\Delta D$ induction splitting to $B\otimes_{kG}M=M$.

If $D$ is cyclic, every [module source](../../../representation-theory.md#source-of-an-indecomposable-module) for every [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $Q\le D$ occurs among the finitely many [indecomposable modules for a cyclic p-group](../../../representation-theory.md#indecomposable-modules-for-a-cyclic-p-group). Each [module](../../../module-theory.md#module-mathematics) in the block is a summand of an induction of one of these finitely many [module sources](../../../representation-theory.md#source-of-an-indecomposable-module). There are finitely many [subgroups](../../../group.md#subgroup) $Q$ and each [induced representation](../../../representation-theory.md#induced-representation) has finitely many indecomposable summands by [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem). Thus **cyclic defect implies finite representation type of the block**.

For the converse, the restriction $B\downarrow_{D\times D}$ has the regular $kD$-bimodule as a [direct summand](../../../vector-space.md#direct-summand). To see this from [module vertices](../../../representation-theory.md#vertex-of-an-indecomposable-module) and [module sources](../../../representation-theory.md#source-of-an-indecomposable-module), its [Brauer quotient of a module](../../../representation-theory.md#brauer-quotient-of-a-module) at $\Delta D$ is nonzero. Its summands are [permutation modules](../../../representation-theory.md#permutation-module) for the $p$-group $D\times D$ and have [module vertices](../../../representation-theory.md#vertex-of-an-indecomposable-module) of order at most $|D|$. A summand detected at $\Delta D$ therefore has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $\Delta D$ and trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module), hence is

$$
\operatorname{Ind}_{\Delta D}^{D\times D}k\cong kD.
$$

Here a transitive [permutation module](../../../representation-theory.md#permutation-module) for a $p$-group is indecomposable: it has one-dimensional [head of a module](../../../module-theory.md#head-of-a-module) over the local [group algebra](../../../associative-algebra.md#group-algebra) and cannot split into two nonzero [modules](../../../module-theory.md#module-mathematics). This also explains the Brauer-quotient detection used in the argument.

For any $kD$-module $U$, tensor that split bimodule inclusion with $U$. It gives

$$
U\mid\operatorname{Res}_D^G(B\otimes_{kD}U),
$$

where $\mid$ denotes being a [direct summand](../../../vector-space.md#direct-summand). If $B$ has only finitely many [indecomposable modules](../../../module-theory.md#indecomposable-module) $M_1,\ldots,M_s$, each $B\otimes_{kD}U$ is a sum of these. Therefore every indecomposable $U$ must occur among the summands of the finite list $M_i\downarrow_D$. Thus $kD$ has finite representation type.

A noncyclic $p$-group has a quotient $C_p\times C_p$: its [Frattini quotient](../../../finite-group-theory.md#frattini-quotient) has rank at least two, since a one-generator [Frattini quotient](../../../finite-group-theory.md#frattini-quotient) forces the [group](../../../group.md) itself to be cyclic. Inflation along this quotient embeds all the [indecomposable modules](../../../module-theory.md#indecomposable-module) of that elementary abelian [group](../../../group.md), preserving isomorphisms and indecomposability. Part (b) rules out finite type when $k$ is infinite.

The conclusion remains valid if the splitting [field](../../../algebra.md#field) $k$ is finite. For completeness, replace the scalar parameter in part (b) by an $m\times m$ companion matrix $T_f$ of an irreducible polynomial $f$. On $k^m\oplus k^m$ use

$$
x=\begin{pmatrix}0&0\\I&0\end{pmatrix},\qquad
y=\begin{pmatrix}0&0\\T_f&0\end{pmatrix}.
$$

An endomorphism commuting with these has form $\left(\begin{smallmatrix}A&0\\C&A\end{smallmatrix}\right)$ with $AT_f=T_fA$. Its [endomorphism ring](../../../module-theory.md#endomorphism-ring) has a square-zero [ideal](../../../commutative-algebra.md#ideal) of the $C$-matrices and quotient $k[T_f]\cong k[t]/(f)$, a [field](../../../algebra.md#field), so it is local and the [module](../../../module-theory.md#module-mathematics) is indecomposable. Finite [fields](../../../algebra.md#field) have irreducible polynomials of arbitrarily large degrees, giving infinitely many dimensions. This also excludes noncyclic $D$ in that case. Altogether,

$$
\boxed{B\text{ has finite representation type}\quad\Longleftrightarrow\quad D\text{ is cyclic}.}
$$

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the conjugation action, fixed elements have coefficients constant on $G$-conjugacy classes. Therefore **$(\mathcal OG)^G=Z(\mathcal OG)$**. More generally an $\mathcal O$-basis of $(\mathcal OG)^H$ consists of sums of the $H$-conjugation orbits on $G$.

For $a\in(\mathcal OG)^H$ define the [relative trace](../../../representation-theory.md#relative-trace), or transfer, by

$$
\operatorname{Tr}_H^G(a)=\sum_{g\in G/H}gag^{-1}.
$$

The expression is independent of the coset representatives and is $G$-fixed. If $z\in Z(\mathcal OG)$, then $z\operatorname{Tr}_H^G(a)=\operatorname{Tr}_H^G(za)$; hence its image is a [transfer ideal of conjugation-fixed elements](../../../representation-theory.md#transfer-ideal-of-conjugation-fixed-elements) in the [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra).

Let $P$ be a Sylow $p$-subgroup of $H$. Trace transitivity gives $\operatorname{Tr}_P^G=\operatorname{Tr}_H^G\operatorname{Tr}_P^H$, proving inclusion of the $P$-image in the $H$-image. Conversely $[H:P]$ is a unit of $\mathcal O$, and for an $H$-fixed element $a$,

$$
\operatorname{Tr}_P^H(a)=[H:P]a.
$$

Thus $\operatorname{Tr}_H^G(a)=\operatorname{Tr}_P^G(a/[H:P])$, proving the reverse inclusion and

$$
\boxed{(\mathcal OG)_H^G=(\mathcal OG)_P^G.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the basis of $D$-conjugation orbit sums in $kG$. A singleton orbit is exactly an element of $C_G(D)$, so these basis vectors span the subring $kC_G(D)$. For a nonsingleton orbit with representative $x$, its stabilizer is the proper [subgroup](../../../group.md#subgroup) $E=C_D(x)<D$, and its orbit sum is $\operatorname{Tr}_E^D(x)$. Thus every nonsingleton basis vector belongs to the sum of proper-subgroup transfer images.

Conversely the coefficient at a $D$-fixed basis element $x\in C_G(D)$ in $\operatorname{Tr}_E^D(a)$ is $[D:E]a_x=0$ in characteristic $p$ whenever $E<D$. Hence the two spans intersect trivially, giving

$$
\boxed{(kG)^D=kC_G(D)\oplus I_D^{\mathrm{prop}},\qquad
I_D^{\mathrm{prop}}=\sum_{E<D}\operatorname{Tr}_E^D((kG)^E).}
$$

For $u\in(kG)^D$, multiplication by a transfer element satisfies $u\operatorname{Tr}_E^D(a)=\operatorname{Tr}_E^D(ua)$ and $\operatorname{Tr}_E^D(a)u=\operatorname{Tr}_E^D(au)$. Therefore the second summand is a two-sided [ideal](../../../commutative-algebra.md#ideal), as required; it need not be nilpotent in this general setting.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Projection onto the subring in part (b), along the two-sided [ideal](../../../commutative-algebra.md#ideal), is the [Brauer homomorphism](../../../representation-theory.md#brauer-morphism):

$$
\boxed{\operatorname{Br}_D:(kG)^D\to kC_G(D),\qquad
\sum_x a_xx\longmapsto\sum_{x\in C_G(D)}a_xx.}
$$

It is a unital [algebra](../../../algebra.md) homomorphism because it is the quotient by that [ideal](../../../commutative-algebra.md#ideal) followed by the displayed subring identification.

Put $N=N_G(D)$. The projection is $N$-equivariant, since $N$ preserves the [centralizer](../../../group-theory.md#centralizer). Its restricted kernel is

$$
\boxed{\ker(\operatorname{Br}_D|_{(kG)^N})
=(kG)^N\cap\sum_{E<D}\operatorname{Tr}_E^D((kG)^E).}
$$

Equivalently it is spanned by the sums of the $N$-conjugation orbits on $G$ disjoint from $C_G(D)$. Normality of $D$ in $N$ ensures that an $N$-orbit either lies wholly inside that [centralizer](../../../group-theory.md#centralizer) or wholly outside it.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Write $N=N_G(D)$, $C=C_G(D)$, and use the commutative transfer [ideals](../../../commutative-algebra.md#ideal)

$$
I_D=\operatorname{Tr}_D^G((kG)^D)\subseteq Z(kG),\qquad
J_D=\operatorname{Tr}_D^N(kC)\subseteq(kC)^N.
$$

The target fixed [algebra](../../../algebra.md) is commutative, because $C\le N$ makes every $N$-fixed element of $kC$ central in $kC$.

The [Brauer morphism and relative trace](../../../representation-theory.md#brauer-morphism-and-relative-trace) identity is

$$
\operatorname{Br}_D(\operatorname{Tr}_D^G a)=\operatorname{Tr}_D^N(\operatorname{Br}_D a).
$$

Indeed let $D$ act on $G/D$ by left multiplication in the trace sum. Its fixed cosets are exactly $gD$ with $g\in N$; every other orbit has size divisible by $p$. After Brauer projection the contributions on each such nonfixed orbit are equal, so they cancel. Fixed cosets give precisely the right-hand side. Since the Brauer projection of $(kG)^D$ is all of $kC$, this proves a surjection **$I_D\twoheadrightarrow J_D$**.

We use the [trace criterion for defect groups](../../../representation-theory.md#trace-criterion-for-defect-groups): a block [idempotent](../../../commutative-algebra.md#idempotent) $e$ belongs to $I_D$ exactly when its defect [group](../../../group.md) is conjugate into $D$; among these, $\operatorname{Br}_D(e)\ne0$ exactly when its defect [group](../../../group.md) is $D$ up to conjugacy. The criterion can be read from the class-sum basis: if $E=C_D(x)$ then

$$
\operatorname{Tr}_D^G(\operatorname{Tr}_E^D x)
=\operatorname{Tr}_E^G x=[C_G(x):E]\,[x^G].
$$

This coefficient is nonzero exactly when $E$ is a Sylow $p$-subgroup of $C_G(x)$. Thus $I_D$ is spanned by classes whose class defect is conjugate into $D$, and the kernel of its Brauer projection is the sum of the corresponding proper-subgroup transfer [ideals](../../../commutative-algebra.md#ideal). The block version follows by refinement of the [central idempotents](../../../associative-algebra.md#central-idempotent) in these [ideals](../../../commutative-algebra.md#ideal).

For clarity, the refinement fact needed here is [primitive idempotents under a surjection of commutative Artinian ideals](../../../commutative-algebra.md#primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals): a surjection between [ideals](../../../commutative-algebra.md#ideal) of commutative Artinian [algebras](../../../algebra.md) bijects the [primitive idempotents](../../../commutative-algebra.md#primitive-idempotent) in the [module source](../../../representation-theory.md#source-of-an-indecomposable-module) whose images are nonzero with the [primitive idempotents](../../../commutative-algebra.md#primitive-idempotent) in the target. Decompose the [algebras](../../../algebra.md) into local factors. An [ideal](../../../commutative-algebra.md#ideal) in a local Artinian factor either contains the identity and is the whole factor, or lies in its nilpotent maximal [ideal](../../../commutative-algebra.md#ideal) and has no nonzero [idempotents](../../../commutative-algebra.md#idempotent). A surviving local factor has a local quotient, so its identity remains primitive. This proves the stated refinement fact without imposing nilpotence on the entire kernel.

The [primitive idempotents](../../../commutative-algebra.md#primitive-idempotent) in $I_D$ are the block [idempotents](../../../commutative-algebra.md#idempotent) with defect conjugate into $D$, and the surviving ones have defect $D$. Applying refinement to the surjection above gives

$$
\boxed{e\longmapsto\operatorname{Br}_D(e):
\{\text{blocks of }G\text{ with defect }D\}\ \longleftrightarrow\
\{\text{primitive idempotents of }J_D\}.}
$$

This is the [Brauer morphism on a defect transfer ideal](../../../representation-theory.md#brauer-morphism-on-a-defect-transfer-ideal); the target is the transfer [ideal](../../../commutative-algebra.md#ideal) $J_D$, not the entire fixed [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

If $N_G(D)\le H\le G$, then $N_H(D)=N_G(D)=N$ and $C_H(D)=C_G(D)=C$. Applying part (d) to $G$ and to $H$ therefore gives the same target [ideal](../../../commutative-algebra.md#ideal)

$$
J_D=\operatorname{Tr}_D^N(kC).
$$

Compose the two bijections. A block [idempotent](../../../commutative-algebra.md#idempotent) $e$ of $G$ with defect $D$ corresponds to the unique block [idempotent](../../../commutative-algebra.md#idempotent) $f$ of $H$ with defect $D$ satisfying

$$
\boxed{\operatorname{Br}_D^G(e)=\operatorname{Br}_D^H(f).}
$$

This proves the requested form of [Brauer first main theorem](../../../representation-theory.md#brauer-first-main-theorem), including uniqueness and the equality of the Brauer images.

## 5

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $D$ be a $p$-subgroup and let $N_G(D)\le H\le G$. Put

$$
\mathcal X=\{D\cap{}^gD:g\in G\setminus H\},\qquad
\mathcal Y=\{H\cap{}^gD:g\in G\setminus H\}.
$$

A [module](../../../module-theory.md#module-mathematics) relatively projective for a family means a summand of a sum of [modules](../../../module-theory.md#module-mathematics) induced from its members, allowing [subgroups](../../../group.md#subgroup) and conjugates. The [Green correspondence](../../../representation-theory.md#green-correspondence) gives inverse bijections $f,g$ between the indecomposable $RG$-modules and $RH$-modules with [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$, up to isomorphism, such that

$$
\operatorname{Res}_H^G M\cong f(M)\oplus M_{\mathcal Y},\qquad
\operatorname{Ind}_H^G U\cong g(U)\oplus U_{\mathcal X}.
$$

The error terms are respectively relatively $\mathcal Y$-projective and $\mathcal X$-projective. In particular the displayed correspondents are the unique summands of [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$, occur with multiplicity one, and have the same [module source](../../../representation-theory.md#source-of-an-indecomposable-module) as the original [module](../../../module-theory.md#module-mathematics), up to [normalizer](../../../group-theory.md#normalizer) conjugacy.

We will also use the general form of [Green correspondence](../../../representation-theory.md#green-correspondence): replace [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $D$ by any [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $Q\le D$ not conjugate into a member of $\mathcal X$. Restriction and induction again have unique summands with that [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module), and the same error-family description. This is important in the final induction argument: merely knowing that an error term has a proper [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) would not give the required intersection bound.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Put $b=\operatorname{Br}_D(e)$. By equivariance of the [Brauer homomorphism](../../../representation-theory.md#brauer-morphism), $b$ is a [central idempotent](../../../associative-algebra.md#central-idempotent) of $kK$, since $C_G(D)\le K\le N_G(D)$. The [Nagao module theorem](../../../representation-theory.md#nagao-module-theorem) asserts that, if $eM=M$, then

$$
\boxed{M\downarrow_K=bM\oplus(1-b)M,}
$$

and every indecomposable summand of $(1-b)M$ is relatively projective for a $p$-subgroup of $K$ not containing $D$. Because $D$ is normal in $K$, its [module vertices](../../../representation-theory.md#vertex-of-an-indecomposable-module) cannot contain $D$ even after $K$-conjugation.

Here is a direct proof. As an element of $(kG)^K$, $e-b$ is a linear combination of $K$-conjugation orbit sums supported outside $C_G(D)$. An orbit represented by $x$ has sum

$$
\operatorname{Tr}_{C_K(x)}^K(x).
$$

Its stabilizer $C_K(x)$ does not contain $D$. On $T=(1-b)M$, the element $e-b$ acts as the identity. Map the orbit-sum expression into $\operatorname{End}_k(M)$ by left multiplication, and compose on both sides with the $K$-linear projection onto $T$. It follows that

$$
\operatorname{id}_T\in\sum_{x\notin C_G(D)}
\operatorname{Tr}_{C_K(x)}^K\operatorname{End}_{kC_K(x)}(T).
$$

Replace each [centralizer](../../../group-theory.md#centralizer) by a Sylow $p$-subgroup of it using trace transitivity and its invertible prime-to-$p$ index. Project this identity further onto an indecomposable summand $U$ of $T$. Its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is local by [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem). A sum of nonunits cannot be the identity in a [local ring](../../../commutative-algebra.md#local-ring), so one of the trace terms is a unit $u$ in $\operatorname{End}_{kK}(U)$. Multiplying the endomorphism inside that trace by $u^{-1}$ gives $\operatorname{id}_U$ as a single relative trace. The [D. Higman criterion](../../../representation-theory.md#d-higman-criterion) makes $U$ relatively projective for that [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $Q\le C_K(x)$, and $D\nleq Q$. This proves the assertion rather than just invoking the theorem's name.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Take $N=N_G(D)$ and $b=\operatorname{Br}_D(e)$. If $eM=M$, the [Nagao module theorem](../../../representation-theory.md#nagao-module-theorem) with $K=N$ puts every vertex-$D$ summand of $M\downarrow_N$ inside $bM$. In particular its [Green correspondence](../../../representation-theory.md#green-correspondence) summand $M'$ satisfies $bM'=M'$.

Conversely a [central idempotent](../../../associative-algebra.md#central-idempotent) acts as zero or one on the [indecomposable module](../../../module-theory.md#indecomposable-module) $M$. If $eM=0$, apply the same theorem to $1-e$. Its Brauer image is $1-b$, so $(1-b)M'=M'$, incompatible with $bM'=M'$. Thus

$$
\boxed{eM=M\quad\Longleftrightarrow\quad\operatorname{Br}_D(e)M'=M'.}
$$

For the unheaded induction request, write $\mathcal X=\{D\cap{}^gD:g\notin N\}$. We prove the sharper intersection bound, not just a drop in [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) size. We use [Green correspondence](../../../representation-theory.md#green-correspondence) on permutation bimodules and the usual [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) test for a permutation-module summand: its [Brauer quotient of a module](../../../representation-theory.md#brauer-quotient-of-a-module) at $P$ is nonzero precisely when a [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) contains a conjugate of $P$. This test follows by restricting to the $p$-group $P$, decomposing the permutation basis into its orbits, and noting that proper-orbit sums are precisely the proper-subgroup transfer terms.

Consider $kG$ as a $k[G\times D]$-module, with $(g,d)a=gad^{-1}$. It is the transitive [permutation module](../../../representation-theory.md#permutation-module) induced from $\Delta D$. Set $L=G\times D$ and $L_0=N\times D$; the latter contains $N_L(\Delta D)$. Its restriction decomposes as

$$
kG\downarrow_{L_0}=kN\oplus\bigoplus_{g\in N\backslash G/D,\ g\notin N}k[NgD].
$$

Each outside term has stabilizer a conjugate of a [subgroup](../../../group.md#subgroup) of $\Delta D$. If a diagonal [subgroup](../../../group.md#subgroup) $\Delta Q\le\Delta D$ embeds into one of these stabilizers, then $Q\le D\cap{}^gD$ for an outside representative. Thus its diagonal [module vertices](../../../representation-theory.md#vertex-of-an-indecomposable-module) are in the intersection error family.

Every indecomposable $L_0$-summand of $kN$ has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $\Delta D$. To justify this, its endomorphisms are right multiplications by elements of $(kN)^D$. The coefficient projection $\operatorname{Br}_D^N$ on this [algebra](../../../algebra.md) has nilpotent kernel: every nonsingleton $D$-orbit sum lies in the kernel of $kN\to k(N/D)$, by part 1(b), and that kernel is nilpotent by part 1(a). Hence no nonzero [idempotent](../../../commutative-algebra.md#idempotent) endomorphism can have zero Brauer image. Its image summand has nonzero [Brauer quotient of a module](../../../representation-theory.md#brauer-quotient-of-a-module) at $\Delta D$, and its [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module), already contained in a conjugate of $\Delta D$, must be $\Delta D$.

Apply the general [Green correspondence](../../../representation-theory.md#green-correspondence) from part (a) to $L,L_0$. If an indecomposable summand of $kG$ has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) outside the intersection error family, its correspondent must be a summand of $kN$, since the outside double-coset [modules](../../../module-theory.md#module-mathematics) have only error-family [module vertices](../../../representation-theory.md#vertex-of-an-indecomposable-module). It therefore has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $\Delta D$. Consequently **every summand of $kG$ not having [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) $\Delta D$ has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) conjugate into an outside diagonal intersection**. An intersection

$$
\Delta D\cap{}^{(g,d)}\Delta D
$$

with $(g,d)\notin L_0$ projects in its first coordinate into $D\cap{}^gD$ with $g\notin N$; this is the error family required in the question.

Now form the split permutation bimodule

$$
W=(1-e)kG b.
$$

Its [Brauer quotient of a module](../../../representation-theory.md#brauer-quotient-of-a-module) at $\Delta D$ is zero. Indeed $kG(\Delta D)=kC_G(D)$, left multiplication by $e$ becomes multiplication by $\operatorname{Br}_D(e)=b$, and right multiplication by $b$ remains multiplication by $b$. Therefore

$$
W(\Delta D)=(1-b)kC_G(D)b=0.
$$

Here $b$ is central in $kC_G(D)$, so the last product is zero. Every indecomposable bimodule summand of $W$ consequently has [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) in the outside intersection family, by the preceding paragraph, and has trivial [module source](../../../representation-theory.md#source-of-an-indecomposable-module) since it is a permutation-module summand.

Since $V$ has vertex $D$, necessarily $D\le K$. Let $S$ be a [module source](../../../representation-theory.md#source-of-an-indecomposable-module) of $V$ at $D$. The splitting $V\mid kK\otimes_{kD}S$ remains a splitting after applying $b$, since $bV=V$. Inducing to $G$ and applying $1-e$ gives

$$
(1-e)\operatorname{Ind}_K^G V\mid W\otimes_{kD}S.
$$

A trivial-source bimodule summand with [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) conjugate into $\Delta Q$ is a summand of $\operatorname{Ind}_{\Delta Q}^{G\times D}k$. Tensoring with $S$ turns this into a [module](../../../module-theory.md#module-mathematics) induced to $G$ from $Q$ (with the appropriate conjugate restriction of $S$). Thus every summand on the right is relatively projective for some $Q\le D\cap{}^gD$, $g\notin N$. Each $V_j$ lies in the left-hand side, and [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem) now gives

$$
\boxed{D_j\le_G D\cap{}^gD\quad\text{for some }g\in G\setminus N_G(D).}
$$

This proves [Juhász induction refinement](../../../representation-theory.md#juhasz-induction-refinement). If there are no outside elements, the error family is empty and the complementary [module](../../../module-theory.md#module-mathematics) is zero.

## 6

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A finite-dimensional [group algebra](../../../associative-algebra.md#group-algebra) has [finite representation type of a group algebra](../../../representation-theory.md#finite-representation-type-of-a-group-algebra) when there are only finitely many isomorphism classes of finite-dimensional [indecomposable modules](../../../module-theory.md#indecomposable-module). The definition concerns all dimensions, not merely finitely many [modules](../../../module-theory.md#module-mathematics) in each fixed dimension.

Let $e_B$ be the block [idempotent](../../../commutative-algebra.md#idempotent) and choose a maximal [Brauer pair](../../../representation-theory.md#brauer-pair) $(D,b_D)$: $b_D$ is a block [idempotent](../../../commutative-algebra.md#idempotent) of $kC_G(D)$ with $b_D\operatorname{Br}_D(e_B)\ne0$. The [inertial index of a block](../../../representation-theory.md#inertial-index-of-a-block) is

$$
\boxed{e(B)=|N_G(D,b_D):DC_G(D)|,}
$$

where $N_G(D,b_D)$ is the stabilizer of the chosen pair. Changing the pair by conjugation does not alter this number. For cyclic $D$, it is a prime-to-$p$ divisor of $p-1$. Here $n\ge1$, as required for the order-$p$ [subgroup](../../../group.md#subgroup) $Q$ to exist.

Put $H=N_G(Q)$. Since $Q$ is characteristic in $D$, $N_G(D)\le H$, so [Green correspondence](../../../representation-theory.md#green-correspondence) applies. In fact the nonprojective [modules](../../../module-theory.md#module-mathematics) in $B$ have a particularly simple correspondence. If $g\notin H$, a nontrivial intersection $D\cap{}^gD$ would contain the unique order-$p$ [subgroup](../../../group.md#subgroup) of both cyclic [groups](../../../group.md), giving $Q={}^gQ$ and hence $g\in H$, a contradiction. Thus every such intersection is trivial. The error [modules](../../../module-theory.md#module-mathematics) in induction are projective. In restriction, an intersection $H\cap{}^gD$ cannot contain a conjugate of a nontrivial [subgroup](../../../group.md#subgroup) of $D$ by an element of $H$: such a conjugate contains $Q$, and that would again force ${}^gQ=Q$. The general [Green correspondence](../../../representation-theory.md#green-correspondence) therefore pairs all [indecomposable modules](../../../module-theory.md#indecomposable-module) with nontrivial [module vertex](../../../representation-theory.md#vertex-of-an-indecomposable-module) contained in a conjugate of $D$. In particular it pairs the nonprojective [modules](../../../module-theory.md#module-mathematics) of $B$ with the nonprojective [modules](../../../module-theory.md#module-mathematics) of its Brauer correspondent $b$ in $H$; the block-compatible form of the correspondence selects $b$. Explicitly,

$$
M\downarrow_H=f(M)\oplus M_{\mathcal Y},\qquad
f(M)\uparrow^G=M\oplus P,
$$

where $P$ is projective and the restriction error family is $\mathcal Y=\{H\cap{}^gD:g\notin H\}$. One should not replace this restriction error term by projectives without an additional argument about $H$.

For the final structure calculation we use the general cyclic-defect structure theorem, which is permitted here as a general fact: the basic [algebra](../../../algebra.md) of a split [block with cyclic defect group](../../../representation-theory.md#block-with-cyclic-defect-group) is a [Brauer tree algebra](../../../representation-theory.md#brauer-tree-algebra). Its tree has $e(B)$ edges, one simple [module](../../../module-theory.md#module-mathematics) per edge, and exceptional multiplicity

$$
m=\frac{|D|-1}{e(B)}.
$$

For a one-edge tree the basic [algebra](../../../algebra.md) presentation is $k[t]/(t^{m+1})$. This is the local presentation of the tree [algebra](../../../algebra.md), not an assertion that an arbitrary block with one simple [module](../../../module-theory.md#module-mathematics) is automatically uniserial.

With $e(B)=1$ the tree has one edge and $m=p^n-1$. Thus the basic [algebra](../../../algebra.md) of $B$ is

$$
A_0=k[t]/(t^{p^n}).
$$

It has exactly one simple [module](../../../module-theory.md#module-mathematics), $k=A_0/(t)$. Its [ideals](../../../commutative-algebra.md#ideal) are precisely $(t^i)$: for any nonzero element, factor out its lowest power of $t$, after which the remaining factor is a unit. The regular projective therefore has the unique submodule chain

$$
A_0\supset tA_0\supset\cdots\supset t^{p^n-1}A_0\supset0,
$$

with each consecutive factor one-dimensional and simple. A [Morita equivalence](../../../noncommutative-algebra.md#morita-equivalence) from $A_0$ to $B$ preserves simple [modules](../../../module-theory.md#module-mathematics), [projective covers](../../../module-theory.md#projective-cover), submodule lattices and composition length. Hence

$$
\boxed{B\text{ has one simple module }S,\qquad P(S)\text{ is uniserial of length }p^n.}
$$

In the split setting one may also write $B\cong M_{\dim_k S}(A_0)$. The [projective cover](../../../module-theory.md#projective-cover) has $p^n$ [composition factors](../../../module-theory.md#composition-factor) all isomorphic to $S$, so its vector-space dimension is $p^n\dim_kS$, not generally $p^n$.

There is also an elementary reason why the uniserial conclusion follows once the one-simple-module conclusion and finite type are known. If the basic local [algebra](../../../algebra.md) had $\dim J/J^2\ge2$, quotienting its radical square and all but two generators would give $k[x,y]/(x,y)^2$. The two-dimensional parameter family from Question 3(b) would then give infinitely many indecomposables. Thus $J/J^2$ is one-dimensional. [Nakayama lemma](../../../mathematics.md#nakayama-lemma) makes $J$ generated by one element $t$, so its powers yield a chain and the basic [algebra](../../../algebra.md) is $k[t]/(t^r)$. The cyclic-defect calculation above identifies $r=p^n$. This explains why finite representation type rules out branching in this [projective cover](../../../module-theory.md#projective-cover).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
