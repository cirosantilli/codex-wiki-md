# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper22.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [topological spectrum](../../../algebraic-topology.md#spectrum-topology) can be described sequentially by [based spaces](../../../algebraic-topology.md#based-space) $E_j$, $j\ge0$, and structure maps

$$
\sigma_j:S^1\wedge E_j\longrightarrow E_{j+1}.
$$

Iterating these maps gives compatible maps $S^{k-j}\wedge E_j\to E_k$. Equivalently, an [indexed prespectrum](../../../algebraic-topology.md#indexed-prespectrum) on a [universe for spectra](../../../algebraic-topology.md#universe-for-spectra) $U$ has spaces $E(V)$ and unital associative structure maps $S^{W\ominus V}\wedge E(V)\to E(W)$ for finite-dimensional inclusions $V\subset W\subset U$. Here $S^A$ denotes the [one-point compactification](../../../topology.md#alexandroff-extension) of the real [inner product space](../../../linear-algebra.md#inner-product-space) $A$.

A [map of topological spectra](../../../algebraic-topology.md#map-of-topological-spectra) $u:D\to E$ is a family of based maps $u_j:D_j\to E_j$ satisfying

$$
u_{j+1}\sigma_j^D=\sigma_j^E(1\wedge u_j).
$$

The indexed version requires the same compatibility for every inclusion of indexing subspaces. These are point-set maps, before passing to [spectrum homotopy](../../../algebraic-topology.md#spectrum-homotopy) or the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category).

An [Omega-spectrum](../../../algebraic-topology.md#omega-spectrum) is a [topological spectrum](../../../algebraic-topology.md#spectrum-topology) whose adjoint structure maps

$$
E_j\longrightarrow\Omega E_{j+1}
$$

are [weak homotopy equivalences](../../../algebraic-topology.md#weak-homotopy-equivalence). Consequently $\pi_kE=\pi_{k+j}E_j$ whenever $k+j\ge0$, using the structure identifications. In the genuine indexed point-set convention, the word spectrum already includes the stronger condition that $E(V)\to\Omega^{W\ominus V}E(W)$ is a homeomorphism; a general system without that condition is called an [indexed prespectrum](../../../algebraic-topology.md#indexed-prespectrum). Its associated spectrum is obtained by [spectrification](../../../algebraic-topology.md#spectrification). The sequential and indexed conventions present the same stable theory.

A [cell spectrum](../../../algebraic-topology.md#cell-spectrum) is built from the zero [topological spectrum](../../../algebraic-topology.md#spectrum-topology) by successive stable cell attachments. Concretely, attach a free spectrum on the inclusion $S^{m-1}\hookrightarrow D^m$ at some level $j$ by a pushout along its boundary map; its quotient is the stable cell sphere $\Sigma^{m-j}\mathbb S$. Iterating such attachments and taking the colimit gives a [cell spectrum](../../../algebraic-topology.md#cell-spectrum), with successive quotients wedges of integer [suspensions of spectra](../../../algebraic-topology.md#suspension-of-spectra) of the [sphere spectrum](../../../algebraic-topology.md#sphere-spectrum). Negative cell degrees are allowed by choosing $j>m$. In the genuine indexed model apply [spectrification](../../../algebraic-topology.md#spectrification) to this cellular prespectrum. **The compatibility of the structure maps is part of both the objects and their maps.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use derived [smash products of spectra](../../../algebraic-topology.md#smash-product-of-spectra) and replace a [based space](../../../algebraic-topology.md#based-space) by a based [CW complex](../../../algebraic-topology.md#cw-complex) when necessary. The reduced [represented homology theory](../../../homology.md#represented-homology-theory) of $E$ is

$$
\boxed{\widetilde E_k(X)=\pi_k\bigl(E\wedge\Sigma^\infty X\bigr),\qquad k\in\mathbb Z.}
$$

Thus [represented homology theory](../../../homology.md#represented-homology-theory) is covariant in $X$: a based map induces a map of [suspension spectra](../../../algebraic-topology.md#suspension-spectrum), and hence a map on the [stable homotopy groups](../../../algebraic-topology.md#stable-homotopy-group) of the displayed [smash product of spectra](../../../algebraic-topology.md#smash-product-of-spectra). In a well-based sequential model the same definition is

$$
\widetilde E_k(X)=\operatorname*{colim}_{j}\pi_{k+j}(E_j\wedge X),
$$

with $j$ sufficiently large and transition maps given by suspension followed by the structure map.

The reduced [represented cohomology theory](../../../cohomology.md#represented-cohomology-theory) is

$$
\boxed{\widetilde E^q(X)=[\Sigma^\infty X,\Sigma^qE]_{\mathrm{st}},\qquad q\in\mathbb Z.}
$$

The brackets denote maps in the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category). This is contravariant in $X$, by precomposition. For the [Omega-spectrum](../../../algebraic-topology.md#omega-spectrum) $E$ it is also the group of [based homotopy](../../../algebraic-topology.md#based-homotopy) classes $[X,E_q]_*$, where for negative $q$ we take $E_q=\Omega^{-q}E_0$. More generally, for $j\ge\max(q,0)$ the [Omega-spectrum](../../../algebraic-topology.md#omega-spectrum) identifications give $\widetilde E^q(X)=[\Sigma^{j-q}X,E_j]_*$; the shifts and loops supply its abelian group structure. In particular

$$
\widetilde E_k(S^0)=\pi_kE,\qquad\widetilde E^q(S^0)=\pi_{-q}E.
$$

All these definitions are reduced: the basepoint itself contributes zero.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Let $\operatorname{Map}_{\mathrm{sp}}(D,E)$ be the space of point-set [maps of topological spectra](../../../algebraic-topology.md#map-of-topological-spectra). Its underlying set is the first set in the comparison. A member is a compatible collection $D_j\to E_j$, rather than independently chosen maps at the levels.

Because the source is cellular and the target is an [Omega-spectrum](../../../algebraic-topology.md#omega-spectrum), taking [spectrum homotopy](../../../algebraic-topology.md#spectrum-homotopy) classes gives all maps in the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category):

$$
\boxed{[D,E]_{\mathrm{st}}=\pi_0\operatorname{Map}_{\mathrm{sp}}(D,E).}
$$

Thus the first set maps onto the second. **Two point-set maps have the same stable class precisely when they are spectrum-homotopic**, using the cellular cylinder and fibrant target. The homotopy must commute with the structure maps throughout; unrelated levelwise homotopies are not the definition.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

A stable map $u:D\to E$ induces a degree-preserving additive [natural transformation](../../../category.md#natural-transformation) of [represented cohomology theories](../../../cohomology.md#represented-cohomology-theory) by postcomposition with $\Sigma^q u$ in degree $q$. This transformation commutes with the suspension isomorphisms. The resulting map

$$
[D,E]_{\mathrm{st}}\longrightarrow\operatorname{Nat}_{\Sigma}(\widetilde D^*,\widetilde E^*)
$$

is onto, but need not be one-to-one. Its kernel consists of [hyperphantom maps of spectra](../../../algebraic-topology.md#hyperphantom-map-of-spectra): maps $u$ for which $uv=0$ for every stable map

$$
v:\Sigma^{-j}\Sigma^\infty X\longrightarrow D,
$$

for every [based space](../../../algebraic-topology.md#based-space) $X$ and every $j\ge0$. Equivalently, they induce zero in all degrees of [represented cohomology theory](../../../cohomology.md#represented-cohomology-theory) on all [based spaces](../../../algebraic-topology.md#based-space). Therefore

$$
\boxed{\operatorname{Nat}_{\Sigma}(\widetilde D^*,\widetilde E^*)\cong[D,E]_{\mathrm{st}}/\operatorname{HPh}(D,E).}
$$

This condition tests arbitrary [suspension spectra](../../../algebraic-topology.md#suspension-spectrum) with negative shifts. Merely testing [finite spectra](../../../algebraic-topology.md#finite-spectrum) defines a [phantom map of spectra](../../../algebraic-topology.md#phantom-map-of-spectra), which is a weaker condition. In particular the homology conclusion in Question 5 should not be substituted for the cohomology condition here.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The [Yoneda lemma](../../../category.md#yoneda-lemma), applied to the representing [Omega-spectrum](../../../algebraic-topology.md#omega-spectrum) spaces in each degree, makes the comparison more explicit. Put

$$
T_j=\Sigma^{-j}\Sigma^\infty D_j.
$$

The structure map of $D$ supplies $T_j\to T_{j+1}$, and $D$ is the [homotopy colimit of spectra](../../../algebraic-topology.md#homotopy-colimit-of-spectra) of this sequence. The inverse-tower transition on maps into $E$ is precomposition with $T_j\to T_{j+1}$. Under the [suspension spectrum](../../../algebraic-topology.md#suspension-spectrum) adjunction it takes $[D_{j+1},E_{j+1}]_*$ to $[D_j,E_j]_*$ by taking the adjoint through $D_j\to\Omega D_{j+1}$ and the [Omega-spectrum](../../../algebraic-topology.md#omega-spectrum) identification $E_j\simeq\Omega E_{j+1}$.

Consequently the maps of [represented cohomology theories](../../../cohomology.md#represented-cohomology-theory) are exactly the compatible degreewise operations:

$$
\boxed{\operatorname{Nat}_{\Sigma}(\widetilde D^*,\widetilde E^*)\cong\lim_j[D_j,E_j]_* .}
$$

Only nonnegative degrees need be listed, since the suspension compatibility recovers the negative degrees. The [Milnor exact sequence for maps of spectra](../../../algebraic-topology.md#milnor-exact-sequence-for-maps-of-spectra) gives the sharper description

$$
0\longrightarrow\lim\nolimits^1_j[\Sigma D_j,E_j]_*\longrightarrow[D,E]_{\mathrm{st}}\longrightarrow\lim_j[D_j,E_j]_*\longrightarrow0.
$$

Thus $\operatorname{HPh}(D,E)\cong\lim^1_j[\Sigma D_j,E_j]_*$, with bonding maps coming from the same telescope. For an inverse tower $A_j$ with maps $r_j:A_{j+1}\to A_j$, $\lim A_j$ is the kernel and $\lim^1 A_j$ is the cokernel of

$$
\prod_j A_j\longrightarrow\prod_j A_j,\qquad(a_j)\longmapsto(a_j-r_j(a_{j+1})).
$$

**The first comparison quotients by spectrum homotopy; the second quotients by hyperphantom maps.** These are different identifications.

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $f_x$ for the [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) specified at $x$. Choose a cofinal sequence $V_i$ from the indexing family $I$, and write the target part of the supplied [subordinate flag for a family of linear isometries](../../../algebraic-topology.md#subordinate-flag-for-a-family-of-linear-isometries) as $W_i$. After a cofinal enlargement it has

$$
V_i\subset V_{i+1},\qquad W_i\subset W_{i+1},\qquad f_x(V_i)\subset W_i\quad(x\in X).
$$

Both flags exhaust their [universe for spectra](../../../algebraic-topology.md#universe-for-spectra). Compactness of the parameter space ensures that a finite target stage can contain all images of each fixed source stage.

Let $\xi_i$ be the [vector bundle](../../../fiber-bundle.md#vector-bundle) on $X$ with fiber

$$
(\xi_i)_x=W_i\ominus f_x(V_i).
$$

Here $\ominus$ is the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) in the indicated ambient subspace. Its rank is $\dim W_i-\dim V_i$. Let $\operatorname{Th}(\xi_i)$ be its [Thom space](../../../fiber-bundle.md#thom-space), the disk bundle modulo its sphere bundle, so that every fiber is compactified and all its points at infinity become the single basepoint. For the zero bundle this convention gives $\operatorname{Th}(0_X)=X_+$. Define a target [indexed prespectrum](../../../algebraic-topology.md#indexed-prespectrum) on the flag by

$$
P(W_i)=\operatorname{Th}(\xi_i)\wedge E(V_i).
$$

The [smash product](../../../algebraic-topology.md#smash-product) here is of [based spaces](../../../algebraic-topology.md#based-space), not yet the derived [smash product of spectra](../../../algebraic-topology.md#smash-product-of-spectra).

To specify all structure maps, for $i\le j$ use the continuous fiberwise orthogonal isomorphism

$$
(W_j\ominus W_i)\oplus(\xi_i)_x\cong(\xi_j)_x\oplus f_x(V_j\ominus V_i).
$$

Both sides identify with the complement of $f_x(V_i)$ in $W_j$. In particular this is the isometry obtained by orthogonally projecting onto $f_x(V_j\ominus V_i)$ and its complement; it is not an assertion that the displayed summands coincide separately. Pass to fiberwise [one-point compactifications](../../../topology.md#alexandroff-extension), identify the last summand with $V_j\ominus V_i$ using $f_x^{-1}$, and apply the source structure map. This defines

$$
S^{W_j\ominus W_i}\wedge P(W_i)\longrightarrow P(W_j).
$$

More explicitly, decompose $z+w\in W_j\ominus f_x(V_i)$, where $z\in W_j\ominus W_i$ and $w\in(\xi_i)_x$, as $w'+f_x(v)$ with $w'\in(\xi_j)_x$ and $v\in V_j\ominus V_i$. Send its pair with $e\in E(V_i)$ to the pair $(w',\sigma_{V_i,V_j}(v,e))$ over $x$. The notation for finite vectors extends to the compactifications, sending infinities and basepoints to the basepoint. Orthogonal decomposition and associativity of the source structure maps prove the prespectrum identities.

Extend the [indexed prespectrum](../../../algebraic-topology.md#indexed-prespectrum) from the cofinal flag to the target indexing family and apply [spectrification](../../../algebraic-topology.md#spectrification) $L$. The point-set definition is

$$
\boxed{X\ltimes_f E=LP.}
$$

On a [map of topological spectra](../../../algebraic-topology.md#map-of-topological-spectra) $u:E\to E'$ it is induced at stage $i$ by $1_{\operatorname{Th}(\xi_i)}\wedge u(V_i)$. Thus the prescribed isometry family, indexing family and flag have all been used. A common cofinal refinement identifies the resulting objects in the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category); the point-set model retains the chosen flag. If $f$ is a constant standard inclusion, the complement bundles are trivial and this recovers the usual reindexed $X_+\wedge E$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [associativity of twisted half-smash products](../../../algebraic-topology.md#associativity-of-twisted-half-smash-products) follows from an actual isomorphism of the complement bundles. First work over compact parameter spaces, so that a common choice of flags can be made. Choose source, intermediate and target stages $V_i,W_i,Z_i$ satisfying

$$
f_x(V_i)\subset W_i,\qquad g_y(W_i)\subset Z_i.
$$

For the two [twisted half-smash products](../../../algebraic-topology.md#twisted-half-smash-product) and their composite the relevant [vector bundles](../../../fiber-bundle.md#vector-bundle) have fibers

$$
\xi_x=W_i\ominus f_x(V_i),\qquad\eta_y=Z_i\ominus g_y(W_i),\qquad\zeta_{y,x}=Z_i\ominus g_yf_x(V_i).
$$

Pull the first two bundles back to $Y\times X$. Since $g_y$ is a [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces), the decomposition of $Z_i$ into $g_y(W_i)$ and its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) gives the fiberwise [vector bundle isomorphism](../../../fiber-bundle.md#vector-bundle-isomorphism)

$$
\boxed{\zeta_{y,x}=\eta_y\oplus g_y(\xi_x).}
$$

Its inverse is given by the two orthogonal projections. The isomorphism varies continuously with $(y,x)$, and the ranks agree:

$$
\dim Z_i-\dim V_i=(\dim Z_i-\dim W_i)+(\dim W_i-\dim V_i).
$$

The [one-point compactification](../../../topology.md#alexandroff-extension) of an external orthogonal direct sum gives the [smash product](../../../algebraic-topology.md#smash-product) of its [Thom spaces](../../../fiber-bundle.md#thom-space). Using $g_y$ to identify $g_y(\xi_x)$ with $\xi_x$, the isomorphism therefore gives

$$
\operatorname{Th}(\zeta)\wedge E(V_i)\cong\operatorname{Th}(\eta)\wedge\operatorname{Th}(\xi)\wedge E(V_i).
$$

The left side is a stage of $(Y\times X)\ltimes_hE$ and the right side is the corresponding two-step prespectrum presentation of $Y\ltimes_g(X\ltimes_fE)$.

These stage comparisons commute with structure maps. Indeed, increasing a stage decomposes a suspension vector into its component in $g_yf_x(V_j\ominus V_i)$ and the two residual complement components. In either construction the same source component is pulled back to $V_j\ominus V_i$ and used in the same structure map of $E$; the residual components are left in the same final complement. Iterated orthogonal decomposition gives the same result whether the intermediate complement is separated first or last. They also commute with maps of $E$, since the comparison only rearranges the suspension coordinates.

For clarity about the intervening [spectrification](../../../algebraic-topology.md#spectrification), maps out of $LP$ into a genuine indexed spectrum $T$ are precisely compatible prespectrum maps $P\to T$. At stage $i$, adjunction from the Thom coordinate identifies such a map with a continuous family

$$
E(V_i)\longrightarrow\Omega^{(\xi_i)_x}T(W_i)\cong T(f_x(V_i)),
$$

where the last identification is the genuine indexed spectrum structure of $T$. Compatibility between stages is exactly compatibility of this family with the source structure maps. Thus maps out of the twisted construction are continuous families of maps over the specified [linear isometries](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces). A family of such maps over $g$ out of $X\ltimes_fE$ is, by applying this universal property a second time, exactly a family of maps out of $E$ over $g_yf_x$. This is the same orthogonal-coordinate correspondence just constructed; it respects the identifications imposed by each [spectrification](../../../algebraic-topology.md#spectrification). Consequently it descends from the prespectrum presentations to the associated spectra. Common cofinal refinements remove any incompatibility between the independently chosen flags.

The printed hypothesis does not require $Y$ to be compact. For an arbitrary compactly generated parameter space $Y$, use the same construction on compact test spaces mapping into $Y$. Each such family admits the common flags above, and the comparisons agree under restriction because their formula is the canonical orthogonal projection. They therefore assemble into the continuous global comparison in the compactly generated point-set construction. Equivalently, the preceding universal-property correspondence is valid for arbitrary $Y$ and does not impose a uniform finite target stage on all of it. Passing to cellular models for the derived construction gives the requested natural isomorphism

$$
\boxed{Y\ltimes_g(X\ltimes_fE)\cong(Y\times X)\ltimes_hE\quad\text{in the stable homotopy category}.}
$$

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category), a [ring spectrum](../../../algebraic-topology.md#ring-spectrum) is a unital associative monoid object for the [smash product of spectra](../../../algebraic-topology.md#smash-product-of-spectra). Thus it consists of a [topological spectrum](../../../algebraic-topology.md#spectrum-topology) $E$ with multiplication and unit

$$
\mu:E\wedge E\longrightarrow E,\qquad\eta:\mathbb S\longrightarrow E,
$$

where $\mathbb S$ is the [sphere spectrum](../../../algebraic-topology.md#sphere-spectrum), and the identities are

$$
\mu(\mu\wedge1)=\mu(1\wedge\mu),\qquad\mu(\eta\wedge1)=1_E=\mu(1\wedge\eta).
$$

The canonical associativity and unit identifications of the [symmetric monoidal category](../../../category-theory.md#symmetric-monoidal-category) are understood in these formulas. All identities are identities of maps in the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category).

A [commutative ring spectrum](../../../algebraic-topology.md#commutative-ring-spectrum) also satisfies

$$
\boxed{\mu\tau=\mu,}
$$

where $\tau:E\wedge E\to E\wedge E$ interchanges the two factors. This is the ring-object convention; a coherently structured ring spectrum has additional point-set or higher-homotopy data. In particular homotopy-category commutativity alone is not an assertion of such a coherent enhancement.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $A=\Sigma^\infty X_+$ and $H=F(A,E)=F(X_+,E)$. The diagonal of $X$ and its map to a point induce

$$
\Delta:A\longrightarrow A\wedge A,\qquad\epsilon:A\longrightarrow\mathbb S.
$$

Here the identification $(X\times X)_+\cong X_+\wedge X_+$ explains the target of $\Delta$. These maps satisfy the coassociativity, cocommutativity and counit identities, since their underlying maps send $x$ to repeated copies of the same $x$.

Use the defining adjunction of the [function spectrum](../../../algebraic-topology.md#function-spectrum) to define $m:H\wedge H\to H$. Its adjoint is the composite

$$
H\wedge H\wedge A\xrightarrow{1\wedge\Delta}H\wedge H\wedge A\wedge A\xrightarrow{\text{interchange}}(H\wedge A)\wedge(H\wedge A)\xrightarrow{\mathrm{ev}\wedge\mathrm{ev}}E\wedge E\xrightarrow{\mu}E.
$$

Define $u:\mathbb S\to H$ to have adjoint

$$
A\xrightarrow{\epsilon}\mathbb S\xrightarrow{\eta}E.
$$

Thus $m$ is pointwise multiplication, while $u$ is the constant unit. These are genuine stable maps, defined through the internal [function spectrum](../../../algebraic-topology.md#function-spectrum), so the argument does not presume that stable functions have ordinary points.

To verify associativity, take the adjoints of $m(m\wedge1)$ and $m(1\wedge m)$. Both are maps $H^{\wedge3}\wedge A\to E$. Both use the triple diagonal $A\to A^{\wedge3}$, evaluate the three copies of $H$, and multiply the three outputs. The triple diagonals agree by coassociativity; the output maps agree by associativity of the [ring spectrum](../../../algebraic-topology.md#ring-spectrum) $E$. The [function spectrum](../../../algebraic-topology.md#function-spectrum) adjunction therefore makes the original two maps equal. For the left unit, the adjunct of $m(u\wedge1)$ uses $(\epsilon\wedge1)\Delta=1_A$ and $\mu(\eta\wedge1)=1_E$, leaving exactly evaluation. Its adjoint is $1_H$. The same calculation with $(1\wedge\epsilon)\Delta$ proves the right unit. Hence

$$
\boxed{F(X_+,E)\text{ is a ring spectrum}.}
$$

If $E$ is a [commutative ring spectrum](../../../algebraic-topology.md#commutative-ring-spectrum), cocommutativity of $\Delta$ proves that this [function spectrum](../../../algebraic-topology.md#function-spectrum) is commutative as well.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Take a based [CW complex](../../../algebraic-topology.md#cw-complex) model for $X$. Since it is $(n-1)$-connected and $n\ge2$, its reduced ordinary [homology](../../../homology.md) vanishes below degree $n$, with arbitrary constant coefficients. This also follows from a [CW complex](../../../algebraic-topology.md#cw-complex) model with no non-basepoint cells below degree $n$. The [connective spectrum](../../../algebraic-topology.md#connective-spectrum) $E$ has $\pi_qE=0$ for $q<0$.

Filter $X$ by its skeleta. The quotients of consecutive stages are wedges of spheres, so the exact sequences in [represented homology theory](../../../homology.md#represented-homology-theory) give the [homological Atiyah-Hirzebruch spectral sequence](../../../cohomology.md#homological-atiyah-hirzebruch-spectral-sequence)

$$
E^2_{p,q}=\widetilde H_p(X;\pi_qE)\Longrightarrow\widetilde E_{p+q}(X),\qquad d_r:E^r_{p,q}\longrightarrow E^r_{p-r,q+r-1}.
$$

It is first quadrant because $E$ is a [connective spectrum](../../../algebraic-topology.md#connective-spectrum). In a fixed total degree it converges with a finite filtration: cells of sufficiently high dimension cannot contribute in that degree or affect it through a boundary, by the same connectivity bound.

In total degree $n$, every term with $p<n$ is zero, and terms with $q<0$ are zero. The only possible term is

$$
E^2_{n,0}=\widetilde H_n(X;\pi_0E)=H_n(X;\mathbb Z).
$$

No differential can leave it: the target has spatial degree $n-r<n$. No differential can enter it: its source would be $(n+r,1-r)$, whose coefficient degree is negative for every $r\ge2$. Thus it survives unchanged and is the only filtration quotient of $\widetilde E_n(X)$; there is no extension problem. The ordinary [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem) now yields

$$
\boxed{\widetilde E_n(X)\cong H_n(X;\mathbb Z)\cong\pi_n(X).}
$$

The isomorphism uses the stated identification $\pi_0E\cong\mathbb Z$ and is natural in $X$. This is the [bottom-degree generalized Hurewicz isomorphism](../../../algebraic-topology.md#bottom-degree-generalized-hurewicz-isomorphism).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose basepoints and replace the spaces and map by [CW complex](../../../algebraic-topology.md#cw-complex) models. If the hypothesis is stated for unreduced [represented homology theory](../../../homology.md#represented-homology-theory), the basepoint coefficient summands split naturally, so it also gives an isomorphism in reduced [represented homology theory](../../../homology.md#represented-homology-theory). Let $C$ be the homotopy [mapping cone](../../../homology.md#mapping-cone-homological-algebra) of $f$. Its reduced [represented homology theory](../../../homology.md#represented-homology-theory) is zero in every degree, by the exact sequence of the corresponding [cofiber sequence of spectra](../../../algebraic-topology.md#cofiber-sequence-of-spectra).

The [mapping cone](../../../homology.md#mapping-cone-homological-algebra) $C$ is a [simply connected space](../../../algebraic-topology.md#simply-connected-space): the mapping cylinder retracts onto $Z$, and coning off the path-connected space $Y$ adds no fundamental-group generators; the van Kampen calculation gives the quotient of $\pi_1Z$ by the image of $\pi_1Y$, which is trivial. Suppose some positive-degree integral [homology](../../../homology.md) group of $C$ were nonzero, and let $n$ be the least such degree. Then $n\ge2$. Starting with $\pi_1C=0$, the [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem) shows inductively that $\pi_iC=0$ for $i<n$: at each first possible degree $i$, its [homotopy group](../../../algebraic-topology.md#homotopy-group) is identified with the zero group $H_i(C;\mathbb Z)$. It then identifies

$$
\pi_nC\cong H_n(C;\mathbb Z)\ne0.
$$

Applying the result of part (a) to the $(n-1)$-connected [based space](../../../algebraic-topology.md#based-space) $C$ gives $\widetilde E_n(C)\cong\pi_nC\ne0$, contradicting the vanishing of its [represented homology theory](../../../homology.md#represented-homology-theory).

Thus $C$ is integrally acyclic, and the ordinary [homology](../../../homology.md) exact sequence says that $f$ is an integral homology isomorphism. The allowed [homological Whitehead theorem](../../../algebraic-topology.md#homological-whitehead-theorem) for [simply connected spaces](../../../algebraic-topology.md#simply-connected-space) makes the map of [CW complex](../../../algebraic-topology.md#cw-complex) models a homotopy equivalence. Returning to the original spaces therefore gives

$$
\boxed{f\text{ is a weak homotopy equivalence}.}
$$

The simply connected hypothesis is used both in the first-nonzero-degree [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem) argument and in the final [homological Whitehead theorem](../../../algebraic-topology.md#homological-whitehead-theorem).

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Choose a small skeleton $\mathcal F$ of the [finite spectra](../../../algebraic-topology.md#finite-spectrum), including every integer suspension. There is such a set of representatives: a finite list of stable cells and their attaching maps specifies a finite cell model, and the possible attaching maps form sets. For every $F\in\mathcal F$ and every stable map $v:F\to D$, take one copy of $F$ and form

$$
X=\bigvee_{(F,v)}F.
$$

Define the evaluation map $e:X\to D$ by taking its restriction to the $(F,v)$ summand to be $v$. Complete it to the [cofiber sequence of spectra](../../../algebraic-topology.md#cofiber-sequence-of-spectra)

$$
X\xrightarrow{e}D\xrightarrow{p}E\longrightarrow\Sigma X.
$$

This is the [universal evaluation phantom map](../../../algebraic-topology.md#universal-evaluation-phantom-map) construction.

First, $p$ is nonzero. If $p=0$, applying $[D,-]_{\mathrm{st}}$ to the [cofiber sequence of spectra](../../../algebraic-topology.md#cofiber-sequence-of-spectra) gives the exact portion

$$
[D,X]_{\mathrm{st}}\xrightarrow{e_*}[D,D]_{\mathrm{st}}\xrightarrow{p_*}[D,E]_{\mathrm{st}}.
$$

Since $p_*(1_D)=p=0$, exactness supplies $s:D\to X$ with $es=1_D$. Thus $D$ is a [retract](../../../algebraic-topology.md#retract) of $X$. This is also a wedge summand: complete $s$ to a [cofiber sequence of spectra](../../../algebraic-topology.md#cofiber-sequence-of-spectra) $D\to X\to C'\to\Sigma D$. The left inverse $e$ makes this triangle split, giving $X\cong D\vee C'$ in the [stable homotopy category](../../../algebraic-topology.md#stable-homotopy-category). One can see the splitting directly from exactness: the connecting map is zero because $e$ extends $1_D$ across $s$, and consequently the quotient map $X\to C'$ admits a section. This contradicts the assumption on $D$. Hence $p\ne0$.

For any [finite spectrum](../../../algebraic-topology.md#finite-spectrum) $F$ and any $v:F\to D$, its chosen representative has a summand inclusion $\iota_v:F\to X$ with $e\iota_v=v$, after transferring along the representative isomorphism. Consecutive maps of a [cofiber sequence of spectra](../../../algebraic-topology.md#cofiber-sequence-of-spectra) compose to zero, so

$$
pv=pe\iota_v=0.
$$

Thus $p$ is a [phantom map of spectra](../../../algebraic-topology.md#phantom-map-of-spectra). To establish the requested conclusion on all spaces, rather than just coefficient groups, let $K$ first be a finite based [CW complex](../../../algebraic-topology.md#cw-complex). Put $A=\Sigma^\infty K$. The [Spanier-Whitehead dual](../../../algebraic-topology.md#spanier-whitehead-dual) $A^\vee=F(A,\mathbb S)$ is a [finite spectrum](../../../algebraic-topology.md#finite-spectrum). The evaluation and coevaluation adjunction of [Spanier-Whitehead duality](../../../algebraic-topology.md#spanier-whitehead-duality) identifies

$$
\widetilde D_k(K)=\pi_k(D\wedge A)\cong[\Sigma^kA^\vee,D]_{\mathrm{st}}.
$$

Under this identification $p_*$ is postcomposition with $p$. Its source is a [finite spectrum](../../../algebraic-topology.md#finite-spectrum), including when $k$ is negative, so the calculation $pv=0$ proves that $p_*$ is zero on $\widetilde D_k(K)$ for every $k$.

Now let $Y$ be an arbitrary based [CW complex](../../../algebraic-topology.md#cw-complex). It is the filtered union, or filtered [homotopy colimit of spaces](../../../algebraic-topology.md#homotopy-colimit-of-spaces), of its finite based subcomplexes $K$. The [suspension spectrum](../../../algebraic-topology.md#suspension-spectrum) functor and [smash product of spectra](../../../algebraic-topology.md#smash-product-of-spectra) preserve that homotopy colimit. The shifted [sphere spectrum](../../../algebraic-topology.md#sphere-spectrum) is compact, so taking [stable homotopy groups](../../../algebraic-topology.md#stable-homotopy-group) gives

$$
\widetilde D_k(Y)=\operatorname*{colim}_{K\subset Y\ \mathrm{finite}}\widetilde D_k(K),\qquad\widetilde E_k(Y)=\operatorname*{colim}_{K\subset Y\ \mathrm{finite}}\widetilde E_k(K).
$$

Every element of the first group therefore comes from a finite $K$, where $p_*$ has just been proved zero. Consequently $p_*$ is zero on $Y$ as well. A based [CW complex](../../../algebraic-topology.md#cw-complex) replacement extends the conclusion to arbitrary based spaces in the homotopy category. We have constructed

$$
\boxed{p:D\longrightarrow E,\qquad p\ne0\text{ stably},\qquad p_*:\widetilde D_*(Y)\longrightarrow\widetilde E_*(Y)\text{ is zero for every }Y.}
$$

This uses continuity of [represented homology theory](../../../homology.md#represented-homology-theory), not a continuity assertion for [represented cohomology theory](../../../cohomology.md#represented-cohomology-theory); the latter need not hold.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
