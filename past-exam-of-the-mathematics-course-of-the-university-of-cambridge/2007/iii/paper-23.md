# Paper 23

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper23.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper23.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the quotient convention for [projective space](../../../projective-space.md). To a [scheme](../../../ringed-space.md#scheme) $T$, associate the set of pairs

$$
(q,\mathcal L),\qquad q:\mathcal O_T^{\oplus(n+1)}\twoheadrightarrow\mathcal L,
$$

where $\mathcal L$ is a [line bundle](../../../ringed-space.md#line-bundle), modulo [isomorphisms](../../../algebra.md#isomorphism) $\mathcal L\to\mathcal L'$ carrying $q$ to $q'$. Pullback defines the contravariant [functor](../../../category.md#functor). On $T=\operatorname{Spec}A$, this means rank-one [projective module](../../../module-theory.md#projective-module) quotients of $A^{n+1}$; the quotient need not be free. Thus merely listing generating tuples modulo multiplication by a unit would omit points over rings with nontrivial [Picard group](../../../ringed-space.md#picard-group).

This [functor](../../../category.md#functor) is represented by $\mathbb P^n_{\mathbb Z}$. For each $i$, the locus where $q(e_i)$ generates $\mathcal L$ is open. These loci cover $T$, since a surjection onto a rank-one free stalk must have some coefficient a unit in its [local ring](../../../commutative-algebra.md#local-ring). On this locus, trivialize by $q(e_i)$ and write

$$
t_j=\frac{q(e_j)}{q(e_i)},\qquad j\ne i.
$$

These functions specify a map to the standard chart $U_i=\operatorname{Spec}\mathbb Z[t_j:j\ne i]$. Their transition rules are exactly those of [projective space](../../../projective-space.md), so the chart maps glue. Conversely the universal quotient on [projective space](../../../projective-space.md) pulls back to the given pair, and the construction is natural and unique. This proves that [projective space represents invertible quotients](../../../projective-space.md#projective-space-represents-invertible-quotients).

Write its universal exact sequence as

$$
0\longrightarrow\mathcal K\longrightarrow V\otimes\mathcal O\xrightarrow q\mathcal O(1)\longrightarrow0,\qquad V=\mathbb Z^{n+1}.
$$

A first-order change of the quotient, with target trivialized locally, is a map $\delta q:V\otimes\mathcal O\to\mathcal O(1)$. Changing the target trivialization by $1+\varepsilon h$ changes $\delta q$ by $hq$. Restriction to $\mathcal K$ removes this ambiguity, and every local map $\mathcal K\to\mathcal O(1)$ extends because the displayed sequence splits locally. Consequently the [tangent sheaf of a scheme](../../../ringed-space.md#tangent-sheaf-of-a-scheme) is

$$
\mathcal T_{\mathbb P^n/\mathbb Z}\cong\mathcal H om(\mathcal K,\mathcal O(1)).
$$

This identification can also be seen on $U_i$: the first-order change of $t_j$ is $\delta q(e_j)-t_j\delta q(e_i)$ after setting $q(e_i)=1$. Thus these maps are precisely the coordinate tangent directions.

Apply $\mathcal H om(-,\mathcal O(1))$ to the universal sequence. Since its terms are [locally free](../../../ringed-space.md#locally-free-sheaf) and it splits locally, this gives the [Euler sequence](../../../algebraic-geometry.md#euler-sequence)

$$
\boxed{0\longrightarrow\mathcal O\xrightarrow{(X_0,\ldots,X_n)}\mathcal O(1)^{\oplus(n+1)}\longrightarrow\mathcal T_{\mathbb P^n/\mathbb Z}\longrightarrow0.}
$$

It remains exact after any base change. Taking its [dual of a sheaf](../../../ringed-space.md#dual-of-a-sheaf) over a [field](../../../algebra.md#field) $k$ gives

$$
0\longrightarrow\Omega^1_{\mathbb P^n_k/k}\longrightarrow\mathcal O(-1)^{\oplus(n+1)}\longrightarrow\mathcal O\longrightarrow0.
$$

For $n=1$, the first term has rank one; taking determinants yields

$$
\boxed{\Omega^1_{\mathbb P^1_k/k}\cong\mathcal O(-2).}
$$

Explicitly, for $u=t^{-1}$ on the overlap of the two affine charts, $du=-t^{-2}dt$, the same transition as $\mathcal O(-2)$ after changing one local frame's sign.

## 2

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Cover the [projective line](../../../finite-group-theory.md#projective-line) by $U_0=\operatorname{Spec}k[t]$ and $U_1=\operatorname{Spec}k[t^{-1}]$. On their overlap the coordinate is invertible. Choose frames $e_0,e_1$ of the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) $\mathcal O(n)$ with $e_1=t^ne_0$. The [vanishing of quasi-coherent cohomology on an affine scheme](../../../ringed-space.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme) applies to both charts and their intersection, so the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex)

$$
0\longrightarrow k[t]\oplus k[t^{-1}]\xrightarrow{\delta}k[t,t^{-1}]\longrightarrow0,\qquad\delta(a,b)=t^nb-a,
$$

computes the [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology). Its kernel identifies with $k[t]\cap t^nk[t^{-1}]$, and its cokernel is

$$
\frac{k[t,t^{-1}]}{k[t]+t^nk[t^{-1}]}.
$$

For $n\geq0$, the intersection has basis $1,t,\ldots,t^n$; for $n<0$ it is zero. In the quotient, powers $t^j$ with $j\geq0$ or $j\leq n$ disappear. The surviving basis for $n\leq-2$ is $t^{n+1},\ldots,t^{-1}$; for $n\geq-1$ none survives. Hence

$$
\boxed{h^0(\mathcal O(n))=\max(n+1,0),\qquad h^1(\mathcal O(n))=\max(-n-1,0),\qquad H^i(\mathcal O(n))=0\ (i\geq2).}
$$

This is the [Čech cohomology of twists on the projective line](../../../ringed-space.md#cech-cohomology-of-twists-on-the-projective-line).

By the preceding question, $\omega=\Omega^1_{\mathbb P^1/k}=\mathcal O(-2)$. In the $dt$ frame its degree-one [Čech cohomology](../../../ringed-space.md#cech-cohomology) is one-dimensional, represented by $t^{-1}dt$. Define

$$
\operatorname{tr}:H^1(\omega)\longrightarrow k,\qquad [h(t)dt]\longmapsto[t^{-1}]h(t).
$$

This is well defined: differentials regular on $U_0$ have nonnegative powers, and those regular on $U_1$ have powers at most $-2$ when expressed using $dt$. Evaluation and the [cup product](../../../cohomology.md#cup-product) give natural pairings

$$
H^i(E)\times H^{1-i}(E^\vee\otimes\omega)\longrightarrow H^1(\omega)\xrightarrow{\operatorname{tr}}k,\qquad i=0,1.
$$

For $E=\mathcal O(n)$ with $n\geq0$, the basis element $t^a$ in $H^0(E)$ pairs with $t^{-a-1}dt$ in $H^1(E^\vee\otimes\omega)$ and with no other element of this dual Laurent basis. The pairing matrix is a permutation matrix, hence invertible. For $n\leq-2$ the same computation exchanges degrees zero and one. For $n=-1$ both sides vanish. Thus the pairings are perfect for every [line bundle](../../../ringed-space.md#line-bundle) on $\mathbb P^1$.

Here we used the classification of [line bundles](../../../ringed-space.md#line-bundle) on the [projective line](../../../finite-group-theory.md#projective-line): they are $\mathcal O(a)$ for integers $a$. One direct justification is that every [line bundle](../../../ringed-space.md#line-bundle) has a nonzero rational section and hence is associated with a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve). The finite closed point defined by an irreducible polynomial $p(t)$ is linearly equivalent to $(\deg p)\infty$, using the [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) of $p(t)$. Thus every divisor is equivalent to its degree times $\infty$, proving the classification over arbitrary $k$.

To extend the pairing to every [locally free coherent sheaf](../../../ringed-space.md#locally-free-sheaf) $E$, induct on rank, without assuming the splitting theorem of the next question. A one-dimensional subspace of the generic fibre, saturated in $E$, gives an exact sequence

$$
0\longrightarrow L\longrightarrow E\longrightarrow Q\longrightarrow0
$$

with $L$ a [line bundle](../../../ringed-space.md#line-bundle) and $Q$ a lower-rank [vector bundle](../../../fiber-bundle.md#vector-bundle). This [saturated line subbundle on a smooth curve](../../../ringed-space.md#saturated-line-subbundle-on-a-smooth-curve) exists because its stalk and its torsion-free quotient are free over the [discrete valuation rings](../../../commutative-algebra.md#discrete-valuation-ring) of the curve. The dual sequence, tensored with $\omega$, is exact as well, since the original sequence splits locally.

The two [long exact sequences in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology), after dualizing one, are compatible with the evaluation pairings. In [Čech cohomology](../../../ringed-space.md#cech-cohomology), this compatibility follows by lifting a section locally: the differences of its lifts represent its connecting class, and contracting those differences with a dual cocycle gives the transpose connecting map, with the usual sign. Thus the connecting maps are adjoint; changing one vertical map's sign gives a commuting diagram. Its rows are

$$
\begin{aligned}
0&\to H^0(L)\to H^0(E)\to H^0(Q)\to H^1(L)\to H^1(E)\to H^1(Q)\to0,\\
0&\to H^1(L^\vee\omega)^*\to H^1(E^\vee\omega)^*\to H^1(Q^\vee\omega)^*\to H^0(L^\vee\omega)^*\to H^0(E^\vee\omega)^*\to H^0(Q^\vee\omega)^*\to0.
\end{aligned}
$$

The maps for $L$ and $Q$ are isomorphisms by the line-bundle calculation and induction. Exactness then makes the maps for $E$ isomorphisms, by the [Five lemma](../../../category-theory.md#five-lemma) (or by comparing the relevant kernels and cokernels). All groups are finite-dimensional because the curve is projective and the sheaves coherent. Therefore [residue duality on the projective line](../../../ringed-space.md#residue-duality-on-the-projective-line) proves

$$
\boxed{H^i(\mathbb P^1,E)\cong H^{1-i}(\mathbb P^1,E^\vee(-2))^*,\qquad i=0,1.}
$$

These isomorphisms are natural in $E$. Higher [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) vanishes by the same two-chart complex.

## 3

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We prove the [Birkhoff–Grothendieck theorem](../../../fiber-bundle.md#birkhoff-grothendieck-theorem) by induction on the rank of the [vector bundle](../../../fiber-bundle.md#vector-bundle) $E$. Rank zero is immediate; rank one is the classification $\operatorname{Pic}(\mathbb P^1_k)\cong\mathbb Z$ established above.

First there is a largest integer $a$ with $H^0(E(-a))\ne0$. To see existence and boundedness directly, trivialize $E$ on the two standard affine charts: the associated finite projective modules over the [principal ideal domains](../../../commutative-algebra.md#principal-ideal-domain) $k[t]$ and $k[t^{-1}]$ are free. Let $A(t)\in GL_r(k[t,t^{-1}])$ be its transition matrix, so a section of $E(-a)$ is a pair satisfying

$$
p(t)=t^{-a}A(t)q(t^{-1}),\qquad p\in k[t]^r,\quad q\in k[t^{-1}]^r.
$$

If $a$ exceeds the largest exponent in any entry of $A$, the right side has only strictly negative powers; the left side has nonnegative powers. Hence both vanish. For $a$ sufficiently negative, take a nonzero constant vector $p$ and put $q=t^aA(t)^{-1}p$; all its exponents are nonpositive, so it supplies a nonzero section. Thus a largest $a$ exists.

Such a section gives a nonzero map $\mathcal O(a)\to E$. It is injective, since it is nonzero generically and the source is torsion-free. Saturate its image. The resulting [line subbundle](../../../fiber-bundle.md#line-subbundle) is $\mathcal O(a+d)$ for the degree $d\geq0$ of the [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) of zeros of the original map. If $d>0$, its inclusion in $E$ would give a nonzero section of $E(-a-d)$, contradicting maximality. Therefore $d=0$ and

$$
0\longrightarrow\mathcal O(a)\longrightarrow E\longrightarrow Q\longrightarrow0
$$

has a [locally free](../../../ringed-space.md#locally-free-sheaf) quotient. By induction, $Q\cong\bigoplus_j\mathcal O(b_j)$.

Twist this exact sequence by $\mathcal O(-a-1)$. The outer groups $H^0(\mathcal O(-1))$ and $H^1(\mathcal O(-1))$ are zero by the [Čech cohomology of twists on the projective line](../../../ringed-space.md#cech-cohomology-of-twists-on-the-projective-line). The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) therefore gives

$$
H^0(E(-a-1))\cong H^0(Q(-a-1)).
$$

The first is zero by the choice of $a$, so each $H^0(\mathcal O(b_j-a-1))$ vanishes. Thus $b_j\leq a$ for every $j$. The extension class lies in

$$
\operatorname{Ext}^1(Q,\mathcal O(a))\cong\bigoplus_jH^1(\mathcal O(a-b_j))=0,
$$

since $a-b_j\geq0$. The identification of this [Ext functor](../../../algebra.md#ext-functor) with cohomology can be seen without additional duality: local splittings of a vector-bundle extension differ by a [Čech cocycle](../../../ringed-space.md#cech-cocycle-condition) in $\mathcal H om(Q,\mathcal O(a))$, and a [coboundary](../../../algebra.md#coboundary) changes them to compatible splittings. Vanishing therefore gives a global splitting. Consequently

$$
\boxed{E\cong\mathcal O(a)\oplus\bigoplus_j\mathcal O(b_j),}
$$

completing the induction over any [field](../../../algebra.md#field) $k$.

The degrees can be arranged in nonincreasing order and their multiset is unique. Indeed, for any such decomposition,

$$
h^0(E(m))-h^0(E(m-1))=\#\{i:a_i\geq-m\},
$$

so the dimensions of the twisted [global sections](../../../ringed-space.md#global-section) recover the number of summands of every degree.

## 4

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $\Omega^1_C=\Omega^1_{C/k}$. A [dualizing sheaf on a smooth projective curve](../../../ringed-space.md#dualizing-sheaf-on-a-smooth-projective-curve), for the [vector bundles](../../../fiber-bundle.md#vector-bundle) in this question, consists of a [line bundle](../../../ringed-space.md#line-bundle) $D_C$ and a trace $H^1(C,D_C)\to k$ making evaluation induce natural perfect pairings

$$
H^i(C,E)\times H^{1-i}(C,E^\vee\otimes D_C)\longrightarrow k,\qquad i=0,1.
$$

In particular it represents the functor $E\mapsto H^1(C,E)^*$ through $\operatorname{Hom}_C(E,D_C)$. We construct it by reducing to the proved [residue duality on the projective line](../../../ringed-space.md#residue-duality-on-the-projective-line).

Choose a separating nonconstant rational function $t$ on $C$. Such a choice exists over any [field](../../../algebra.md#field) $k$: the function field of a [smooth algebraic curve](../../../algebraic-geometry.md#smooth-algebraic-curve) is separably generated of transcendence degree one, and a choice with $dt\ne0$ makes its finite extension of $k(t)$ separable. The map $(t:1)$ extends across poles using $(1:t^{-1})$ in the [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) at each point. It gives a finite generically separable morphism

$$
f:C\longrightarrow\mathbb P^1_k.
$$

Indeed it is nonconstant, hence has finite fibres, and is proper; a proper quasi-finite morphism is finite. This finite map is flat: locally its direct-image module is finite and torsion-free over a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring), and hence free. The same argument works componentwise if needed.

For an affine chart $\operatorname{Spec}B\subset\mathbb P^1$ with inverse image $\operatorname{Spec}A$, form the $A$-[module](../../../module-theory.md#module-mathematics)

$$
W=\operatorname{Hom}_B(A,B),\qquad(a\lambda)(a')=\lambda(aa').
$$

These modules glue to the relative trace-dual sheaf $W_f$ on $C$. There are two algebraic identities used here. First, finite-map adjunction gives

$$
\operatorname{Hom}_A(M,\operatorname{Hom}_B(A,N))\cong\operatorname{Hom}_B(M,N).
$$

The forward map evaluates at $1$; the inverse sends $g$ to $m\mapsto(a\mapsto g(am))$. Second, the different–differential identity for a finite generically separable map between smooth curves gives

$$
W_f\otimes f^*\Omega^1_{\mathbb P^1/k}\cong\Omega^1_{C/k}.
$$

To explain its algebraic content, the field trace identifies $\operatorname{Hom}_B(A,B)$ with the inverse [different ideal](../../../arithmetic.md#different-ideal), while the different is the vanishing ideal of $f^*\Omega^1_{\mathbb P^1/k}\to\Omega^1_{C/k}$. These identities include wild ramification; one must not replace the different by just ramification index minus one. This is the identity allowed to be quoted in the question; the finite-map description is recorded in [Stacks Project, finite morphisms](https://stacks.math.columbia.edu/tag/0FKW), and its differential form in [Stacks Project, Section 53.12](https://stacks.math.columbia.edu/tag/0C1B).

Set $D_C=W_f\otimes f^*\Omega^1_{\mathbb P^1/k}$. The second identity shows it is a [line bundle](../../../ringed-space.md#line-bundle) and already identifies it with $\Omega^1_C$. For a [vector bundle](../../../fiber-bundle.md#vector-bundle) $E$, the first identity gives the sheaf isomorphism

$$
f_*(E^\vee\otimes D_C)\cong\mathcal H om_{\mathbb P^1}(f_*E,\Omega^1_{\mathbb P^1/k})=(f_*E)^\vee\otimes\Omega^1_{\mathbb P^1/k}.
$$

The sheaf $f_*E$ is [locally free](../../../ringed-space.md#locally-free-sheaf): on an affine chart, the projective $A$-module defining $E$ is a summand of $A^r$, and $A$ is finite free over $B$. Since $f$ is finite, affine-cover [Čech cohomology](../../../ringed-space.md#cech-cohomology) identifies $H^j(C,F)$ with $H^j(\mathbb P^1,f_*F)$ for each of these sheaves. Apply the already established duality on $\mathbb P^1$ to $f_*E$. It gives

$$
\boxed{H^i(C,E)\cong H^{1-i}(C,E^\vee\otimes D_C)^*,\qquad D_C\cong\Omega^1_{C/k},\quad i=0,1.}
$$

The trace is obtained by evaluating the trace-dual module at $1$ and then using the trace $H^1(\mathbb P^1,\Omega^1_{\mathbb P^1/k})\to k$. The adjunction formulas show the displayed isomorphisms are induced by evaluation against this trace and are natural in $E$. They thus establish the requested dualizing property, not merely the existence of an invertible differential sheaf. Uniqueness follows from the [Yoneda lemma](../../../category.md#yoneda-lemma) applied to the representing functor on [vector bundles](../../../fiber-bundle.md#vector-bundle).

## 5

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the finite map $f:C\to\mathbb P^1$ from the preceding solution. The inverse images of the two standard affine charts and of their intersection are affine, because $f$ is finite. The [vanishing of quasi-coherent cohomology on an affine scheme](../../../ringed-space.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme) therefore lets their two-term [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex) compute $H^i(C,E)$. It has terms only in degrees zero and one, proving

$$
\boxed{H^i(C,E)=0\qquad(i\geq2).}
$$

This actually applies to every [quasi-coherent sheaf](../../../ringed-space.md#quasi-coherent-sheaf) on $C$.

For a [smooth projective curve](../../../projective-space.md#smooth-projective-curve) with $H^0(C,\mathcal O_C)=k$, define its [genus of a smooth projective curve](../../../projective-space.md#genus-of-a-smooth-projective-curve) by

$$
\boxed{g=\dim_kH^1(C,\mathcal O_C).}
$$

The preceding [Serre duality](../../../ringed-space.md#serre-duality) also gives $g=\dim_kH^0(C,\Omega^1_C)$. The condition on constants holds in particular for a geometrically connected smooth projective curve. It makes $g$ equal to the [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) $1-\chi(\mathcal O_C)$. We state the theorem with this usual convention and then give the formula valid without that condition.

For a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $D$ and a [canonical divisor](../../../algebraic-geometry.md#canonical-divisor) $K$ with $\mathcal O(K)\cong\Omega^1_C$, the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) is

$$
\boxed{\ell(D)-\ell(K-D)=\deg_kD+1-g,\qquad\ell(D)=h^0(C,\mathcal O(D)).}
$$

The degree over an arbitrary [field](../../../algebra.md#field) is weighted by residue degrees: $\deg_kD=\sum_pn_p[k(p):k]$ when $D=\sum_pn_pp$. Equivalently, for a [line bundle](../../../ringed-space.md#line-bundle) $L$,

$$
h^0(L)-h^0(\Omega^1_C\otimes L^{-1})=\deg_kL+1-g.
$$

We now prove it via [Riemann-Roch via elementary modifications](../../../algebraic-geometry.md#riemann-roch-via-elementary-modifications).

For any closed point $p$ and any [line bundle](../../../ringed-space.md#line-bundle) $L$, the exact sequence

$$
0\longrightarrow L(-p)\longrightarrow L\longrightarrow L|_p\longrightarrow0
$$

has a [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) as its quotient, with $k$-dimension $[k(p):k]$. This follows locally from a uniformizer of the [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) at $p$: a local line-bundle generator modulo that uniformizer spans one copy of $k(p)$. The quotient has zero higher cohomology, as it is the direct image from a finite affine scheme. The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) and the proved higher vanishing give

$$
\chi(L)-\chi(L(-p))=[k(p):k],\qquad\chi(L)=h^0(L)-h^1(L).
$$

Every [line bundle](../../../ringed-space.md#line-bundle) has a nonzero [rational section of a line bundle](../../../ringed-space.md#rational-section-of-a-line-bundle), whose local orders give a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $D$ with $L\cong\mathcal O(D)$. Iterating the displayed identity, adding or subtracting closed points with their multiplicities, gives

$$
\chi(\mathcal O(D))=\deg_kD+\chi(\mathcal O_C).
$$

For the constants convention above, $\chi(\mathcal O_C)=1-g$. The [dualizing sheaf on a smooth projective curve](../../../ringed-space.md#dualizing-sheaf-on-a-smooth-projective-curve) gives $h^1(\mathcal O(D))=h^0(\mathcal O(K-D))$, which converts this Euler-characteristic identity into the stated [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem). This proves the formula over arbitrary $k$, without assuming the closed points are $k$-rational.

For [vector bundles](../../../fiber-bundle.md#vector-bundle), the corresponding formula is

$$
\boxed{\chi(E)=\deg_k(\det E)+\operatorname{rank}(E)(1-g).}
$$

To see it, saturate a rational rank-one subspace to a [line subbundle](../../../fiber-bundle.md#line-subbundle) and induct on rank. Both [Euler characteristic of a coherent sheaf](../../../ringed-space.md#euler-characteristic-of-a-coherent-sheaf) and the degree of the determinant are additive in the resulting short exact sequence. The line-bundle formula just proved starts the induction.

Taking $L=\Omega^1_C$ and using duality gives $h^0(\Omega^1_C)=g$, $h^1(\Omega^1_C)=1$, and hence $\deg_k\Omega^1_C=2g-2$. In particular a [line bundle](../../../ringed-space.md#line-bundle) of degree greater than $2g-2$ has zero first cohomology: its dual twisted by $\Omega^1_C$ has negative degree, and a negative-degree line bundle has no nonzero section, since any section would have an [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) of zeros.

If the term “curve over $k$” is used without requiring $H^0(\mathcal O_C)=k$, the unconditional formula we proved is

$$
\boxed{\chi(L)=\deg_kL+\chi(\mathcal O_C).}
$$

Writing $g=h^1(\mathcal O_C)$ then replaces $1-g$ by $h^0(\mathcal O_C)-g$. For example, $\mathbb P^1_{k'}$ viewed as a $k$-curve for a finite separable extension $k'/k$ has $h^0(\mathcal O_C)=[k':k]$, so a literal constant term $1$ would be incorrect. Alternatively the [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) $p_a=1-\chi(\mathcal O_C)$ gives the formula with constant $1-p_a$. The constants hypothesis for the usual genus is recorded in [Stacks Project, genus of a curve](https://stacks.math.columbia.edu/tag/0BY6).

## 6

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Here $k$ is algebraically closed and $C$ is a connected [smooth projective curve](../../../projective-space.md#smooth-projective-curve). For a [scheme](../../../ringed-space.md#scheme) $T$ over $k$, let $\pi:C_T=C\times_kT\to T$. The degree-$d$ [Picard functor of a curve](../../../ringed-space.md#picard-functor-of-a-curve) assigns

$$
\boxed{\operatorname{Pic}^d_C(T)=\{L\in\operatorname{Pic}(C_T):\deg(L|_{C_{\bar t}})=d\text{ for every geometric point }\bar t\}\big/\pi^*\operatorname{Pic}(T).}
$$

One can equivalently take the associated faithfully flat sheaf. It is essential to divide out by [line bundles](../../../ringed-space.md#line-bundle) from the base: a parameter space should remember the family on $C$, not an independent base line bundle.

Choose $p_0\in C(k)$. A class can be normalized as $L\otimes\pi^*(L|_{p_0\times T})^{-1}$, with its canonical trivialization along $p_0\times T$. Since $\pi_*\mathcal O_{C_T}=\mathcal O_T$, an automorphism of a [line bundle](../../../ringed-space.md#line-bundle) is multiplication by a base unit, and preserving this normalization forces that unit to be $1$. Descent of line bundles is effective, so normalized bundles satisfy the faithfully flat sheaf condition with no automorphism ambiguity. Thus this normalized description works on families, including nonreduced bases, rather than only on $k$-points.

We construct a representing scheme by [Picard charts from nonspecial divisors](../../../ringed-space.md#picard-charts-from-nonspecial-divisors). Fix $N\geq2g$ and put $r=N-g$. The [symmetric product of a curve](../../../algebraic-geometry.md#symmetric-product-of-a-curve) $C^{(g)}$ represents [relative effective Cartier divisors on a curve](../../../cartier-divisor.md#relative-effective-cartier-divisor-on-a-curve) of degree $g$ and has a universal divisor $\Delta$. This uses the scheme symmetric product, not the naive set of unordered $T$-points. Locally on a smooth curve, a divisor of length $m$ is described by a monic polynomial in a smooth coordinate; its coefficients are elementary symmetric functions, so this construction includes coincident points in any characteristic. These local descriptions give the usual effective-divisor interpretation of the symmetric product.

Let $W\subset C^{(g)}$ be the open set where $H^1(C,\mathcal O(E))=0$. It is open by [semicontinuity theorem for coherent cohomology](../../../ringed-space.md#semicontinuity-theorem-for-coherent-cohomology). The [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives $h^0(\mathcal O(E))=1$ there, so $E$ is the unique effective divisor in its line-bundle class. For every fixed effective divisor $B$ of degree $r$, take a copy $W_B$ of $W$, with family

$$
L_B=\mathcal O(B+\Delta)
$$

of degree $N$. Normalize it along $p_0$ as above.

This chart represents the open subfunctor defined by

$$
H^1(C,L_t(-B))=0.
$$

Indeed, for a family satisfying that condition, [cohomology and base change for line bundles on a curve](../../../ringed-space.md#cohomology-and-base-change-for-line-bundles-on-a-curve) makes $V=\pi_*L(-B)$ a [line bundle](../../../ringed-space.md#line-bundle) on $T$, with formation commuting with base change. The rank is one by [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem). The evaluation map

$$
\pi^*V\longrightarrow L(-B)
$$

is a nonzero section on each fibre, up to the base twist. Its zero scheme is a [relative effective Cartier divisor on a curve](../../../cartier-divisor.md#relative-effective-cartier-divisor-on-a-curve) $E$ of degree $g$. To check the family assertion, source and target are flat over $T$ and the fibre maps are injections of line bundles on an integral curve, so their cokernel is flat over $T$. Their zeros are Cartier, and the zero scheme is proper with finite fibres of length $g$, hence finite flat of degree $g$. It therefore defines a unique map $T\to W_B$. Conversely this construction recovers the family $\mathcal O(B+E)$ modulo a base line bundle.

The base-change step controls infinitesimal families as well. Locally, a finite free complex computes the two cohomology groups. Vanishing of its degree-one cokernel on fibres makes the last differential surjective by the [Nakayama lemma](../../../mathematics.md#nakayama-lemma). Splitting that differential leaves a locally free degree-zero kernel of rank one and commutes with base change. This is the standard finite-complex form of the permitted cohomology semicontinuity and base-change results.

These chart subfunctors cover all degree-$N$ families. For a geometric-fibre [line bundle](../../../ringed-space.md#line-bundle) $L$ of degree $N$, the preceding solution gives $H^1(L)=0$ and $h^0(L)=N+1-g=r+1$. Choose $r$ points successively so that each imposes one independent condition on the current section space. At each stage that space is nonzero; a nonzero section has finitely many zeros, so a point outside its zero set can be chosen, also outside the finitely many previously chosen points. For their sum $B$,

$$
h^0(L(-B))=1,\qquad\deg L(-B)=g,
$$

and [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) forces $h^1(L(-B))=0$. The points may be chosen in $C(k)$ even when the fibre field extends $k$, since $C(k)$ is infinite and a nonzero section on the base-changed curve has only finitely many zeros. Thus fixed divisors $B$ defined over $k$ suffice. Upper semicontinuity gives an open neighbourhood on the base for each successful $B$.

It remains to glue the charts explicitly. On $W_B$, the locus

$$
W_{BB'}=\{E:H^1(C,\mathcal O(B+E-B'))=0\}
$$

is open. The line bundle inside the braces has degree $g$; its unique section up to scale has an effective zero divisor $E'$. Base change and the evaluation construction make $E\mapsto E'$ a morphism $W_{BB'}\to W_{B'}$. It satisfies $\mathcal O(B+E)\cong\mathcal O(B'+E')$. Reversing $B,B'$ gives its inverse. On triple overlaps the transition maps compose correctly because the residual effective divisor is unique. Hence the copies $W_B$ glue along these open isomorphisms to a [scheme](../../../ringed-space.md#scheme) $P^N$.

The normalized bundles $L_B$ glue as well: on overlaps their normalized isomorphisms exist and are unique, so they satisfy the cocycle condition. Let $\mathcal P_N$ denote the resulting universal normalized [line bundle](../../../ringed-space.md#line-bundle) on $C\times P^N$. For any $T$, the open cover where the conditions for some $B$ hold gives compatible maps $T\to W_B$, and thus a unique map $T\to P^N$. Pulling back $\mathcal P_N$ reverses this procedure. We have established a natural bijection

$$
\boxed{\operatorname{Hom}_k(T,P^N)\cong\operatorname{Pic}^N_C(T).}
$$

This proves representability of the full functor, not just a parametrization of individual line bundles. The nonspecial-divisor construction is also recorded in [Stacks Project, Picard scheme of a curve](https://stacks.math.columbia.edu/tag/0B9R).

Finally tensoring by $\mathcal O_C((N-d)p_0)$ is a natural isomorphism $\operatorname{Pic}^d_C\to\operatorname{Pic}^N_C$ for every integer $d$. Transporting the universal bundle back constructs its degree-$d$ representative $P^d$, usually denoted $\operatorname{Pic}^d_{C/k}$. Thus **every degree component is represented**. These identifications depend on the chosen point and twist; intrinsically the degree-zero component is a group scheme and each degree component is its torsor.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
