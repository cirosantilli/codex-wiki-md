# Paper 17

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper17.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper17.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
- [7](#7)
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
  - [iii](#7/iii)
    - [Solution](#7/iii/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [i](#9/i)
    - [Solution](#9/i/solution)
  - [ii](#9/ii)
    - [Solution](#9/ii/solution)
  - [iii](#9/iii)
    - [Solution](#9/iii/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write the [adjunction](../../../category.md#adjoint-functors) as the [natural bijection](../../../category.md#natural-bijection)

$$
\Phi_{A,B}:\mathcal D(FA,B)\longrightarrow\mathcal C(A,GB).
$$

The [unit of an adjunction](../../../category.md#unit-of-an-adjunction) and [counit of an adjunction](../../../category.md#counit-of-an-adjunction) are the [natural transformations](../../../category.md#natural-transformation) whose components are

$$
\boxed{\eta_A=\Phi_{A,FA}(1_{FA}),\qquad
\varepsilon_B=\Phi^{-1}_{GB,B}(1_{GB}).}
$$

[Naturality](../../../category.md#naturality) of the [hom-set](../../../category.md#hom-set) bijections gives, for $f:FA\to B$ and $g:A\to GB$,

$$
\Phi_{A,B}(f)=G(f)\eta_A,\qquad
\Phi^{-1}_{A,B}(g)=\varepsilon_B F(g).
$$

For example, postcomposition by $f$ in the first [hom-set](../../../category.md#hom-set) corresponds to postcomposition by $Gf$ in the second, giving the first formula; naturality in $A$ gives the second. The same [naturality](../../../category.md#naturality) says that, for $a:A\to A'$ and $b:B\to B'$,

$$
GF(a)\eta_A=\eta_{A'}a,\qquad b\varepsilon_B=\varepsilon_{B'}FG(b).
$$

Thus these components do define the asserted [natural transformations](../../../category.md#natural-transformation) $1_{\mathcal C}\to GF$ and $FG\to1_{\mathcal D}$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The two formulas for the [adjunction](../../../category.md#adjoint-functors) transposes give both [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) directly. Apply the inverse [bijection](../../../function.md#bijection) to the transpose of $1_{FA}$:

$$
1_{FA}=\Phi^{-1}_{A,FA}(\eta_A)=\varepsilon_{FA}F(\eta_A).
$$

Apply the forward [bijection](../../../function.md#bijection) to the inverse transpose of $1_{GB}$:

$$
1_{GB}=\Phi_{GB,B}(\varepsilon_B)=G(\varepsilon_B)\eta_{GB}.
$$

These are equalities of components of [natural transformations](../../../category.md#natural-transformation), so

$$
\boxed{(\varepsilon F)\circ(F\eta)=1_F,\qquad
(G\varepsilon)\circ(\eta G)=1_G.}
$$

No cancellation assumption on either [functor](../../../category.md#functor) is needed: both identities follow from the inverse [hom-set](../../../category.md#hom-set) bijections.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Define maps between the [hom-sets](../../../category.md#hom-set) by

$$
\Phi(f)=G(f)\eta_A,\qquad \Psi(g)=\varepsilon_BF(g).
$$

Using [naturality](../../../category.md#naturality) of the proposed [counit of an adjunction](../../../category.md#counit-of-an-adjunction) and then the first [triangle identity for an adjunction](../../../category.md#triangle-identities-for-an-adjunction),

$$
\Psi\Phi(f)=\varepsilon_BFG(f)F(\eta_A)
=f\varepsilon_{FA}F(\eta_A)=f.
$$

Using [naturality](../../../category.md#naturality) of the proposed [unit of an adjunction](../../../category.md#unit-of-an-adjunction) and then the other [triangle identity for an adjunction](../../../category.md#triangle-identities-for-an-adjunction),

$$
\Phi\Psi(g)=G(\varepsilon_B)GF(g)\eta_A
=G(\varepsilon_B)\eta_{GB}g=g.
$$

Hence $\Phi$ and $\Psi$ are inverse [bijections](../../../function.md#bijection). They are natural in both variables: for $a:A'\to A$ and $b:B\to B'$, the [unit of an adjunction](../../../category.md#unit-of-an-adjunction) identity gives

$$
\Phi(bfF(a))=G(b)G(f)GF(a)\eta_{A'}
=G(b)\Phi(f)a.
$$

This constructs an [adjunction](../../../category.md#adjoint-functors) $F\dashv G$. Taking $f=1_{FA}$ and $g=1_{GB}$ recovers the prescribed [unit of an adjunction](../../../category.md#unit-of-an-adjunction) and [counit of an adjunction](../../../category.md#counit-of-an-adjunction). Conversely, part (i) shows that any [adjunction](../../../category.md#adjoint-functors) with those components must have exactly these transpose formulas. **The adjunction exists and is unique with the prescribed unit and counit.**

## 2

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $\widehat{\mathcal O}=[\mathcal O(S)^{\mathrm{op}},\mathbf{Set}]$, with [categorical presheaf](../../../category.md#presheaf-category-theory) restrictions $X(U)\to X(V)$ when $V\subseteq U$. The five [functors](../../../category.md#functor) are

$$
\Pi X=X(\varnothing),\qquad \Gamma X=X(S),\qquad
(\Delta A)(U)=A,
$$



$$
(\Lambda A)(U)=
\begin{cases}A&U=\varnothing,\\\varnothing&U\ne\varnothing,\end{cases}
\qquad
(\nabla A)(U)=
\begin{cases}A&U=S,\\\{*\}&U\ne S.\end{cases}
$$

In $\Delta A$ all restriction maps are identities. In $\Lambda A$ and $\nabla A$, all nonidentity restrictions are the unique maps permitted by the displayed [sets](../../../set.md). These definitions are valid also when $A$ is empty: a restriction out of $(\nabla A)(S)$ still has singleton target. Maps of [sets](../../../set.md) act at the displayed $A$-components, and [natural transformations](../../../category.md#natural-transformation) act on $\Pi$ and $\Gamma$ by evaluation.

A [natural transformation](../../../category.md#natural-transformation) $\Lambda A\to X$ is determined by an arbitrary map $A\to X(\varnothing)$, since all other source components are empty. A [natural transformation](../../../category.md#natural-transformation) $X\to\Delta A$ is determined by its empty-open component $X(\varnothing)\to A$: the component at $U$ must first restrict $X(U)\to X(\varnothing)$. Similarly, a [natural transformation](../../../category.md#natural-transformation) $\Delta A\to X$ is determined by $A\to X(S)$, followed by the restriction $X(S)\to X(U)$. Finally, a [natural transformation](../../../category.md#natural-transformation) $X\to\nabla A$ is determined by $X(S)\to A$, since all proper-open targets are singletons. These descriptions give the [hom-set](../../../category.md#hom-set) bijections

$$
\widehat{\mathcal O}(\Lambda A,X)\cong\mathbf{Set}(A,\Pi X),\qquad
\mathbf{Set}(\Pi X,A)\cong\widehat{\mathcal O}(X,\Delta A),
$$



$$
\widehat{\mathcal O}(\Delta A,X)\cong\mathbf{Set}(A,\Gamma X),\qquad
\mathbf{Set}(\Gamma X,A)\cong\widehat{\mathcal O}(X,\nabla A).
$$

Thus the [five adjoints for constant presheaves on open sets](../../../category.md#five-adjoints-for-constant-presheaves-on-open-sets) are

$$
\boxed{\Lambda\dashv\Pi\dashv\Delta\dashv\Gamma\dashv\nabla.}
$$

The values at the empty open set are genuine [presheaf](../../../algebraic-geometry.md#presheaf-of-sets-on-a-topological-space) values here; no [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) condition or sheafification is being imposed.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $C\mathcal A=\pi_0\mathcal A$ be the [set](../../../set.md) of [connected components of a category](../../../category.md#connected-component-of-a-category): two [objects of a category](../../../category.md#object-of-a-category) are identified when joined by a finite zigzag of [morphisms](../../../algebra.md#morphism). Let $DA$ be the [discrete category](../../../category.md#discrete-category) on $A$, and let $IA$ be the [indiscrete category](../../../category.md#indiscrete-category) on $A$, with exactly one [morphism](../../../algebra.md#morphism) for every ordered pair of objects.

A [functor](../../../category.md#functor) $\mathcal A\to DA$ must give the same object value along every arrow, hence along every zigzag. Conversely a function $\pi_0\mathcal A\to A$ uniquely defines such a [functor](../../../category.md#functor). A [functor](../../../category.md#functor) $DA\to\mathcal A$ is just a choice of an [object of a category](../../../category.md#object-of-a-category) for each element of $A$. A [functor](../../../category.md#functor) $\mathcal A\to IA$ is likewise determined by an arbitrary object function, since its arrow images are forced and always compose correctly. Therefore

$$
\operatorname{Cat}(\mathcal A,DA)\cong\mathbf{Set}(C\mathcal A,A),\qquad
\operatorname{Cat}(DA,\mathcal A)\cong\mathbf{Set}(A,O\mathcal A),
$$



$$
\operatorname{Cat}(\mathcal A,IA)\cong\mathbf{Set}(O\mathcal A,A).
$$

This is the [adjoint chain for the objects of a category](../../../category.md#adjoint-chain-for-the-objects-of-a-category):

$$
\boxed{C\dashv D\dashv O\dashv I.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Use the [preservation obstructions to extending an adjoint chain](../../../category.md#preservation-obstructions-to-extending-an-adjoint-chain): a [functor](../../../category.md#functor) having a further [left adjoint](../../../category.md#adjoint-functors) must preserve [categorical limits](../../../category.md#categorical-limit), while one having a further [right adjoint](../../../category.md#adjoint-functors) must preserve [colimits](../../../category.md#colimit).

At the left end of the [presheaf category](../../../category.md#presheaf-category) chain, $\Lambda$ does not preserve the [terminal object](../../../category.md#terminal-object). The terminal [categorical presheaf](../../../category.md#presheaf-category-theory) has singleton value everywhere, whereas $(\Lambda1)(S)=\varnothing$ because $S\ne\varnothing$. Thus $\Lambda$ cannot itself be a [right adjoint](../../../category.md#adjoint-functors). At the right end, $\nabla$ does not preserve the [initial object](../../../category.md#initial-object): $(\nabla\varnothing)(\varnothing)=\{*\}$ since the empty open set is proper. Thus $\nabla$ cannot itself be a [left adjoint](../../../category.md#adjoint-functors).

For the [category of small categories](../../../category.md#category-of-small-categories) chain, take two [functors](../../../category.md#functor) from the [terminal category](../../../category.md#terminal-category) $1$ to the two-object [indiscrete category](../../../category.md#indiscrete-category) $I\{0,1\}$, selecting its distinct objects. Their [equalizer](../../../category.md#equaliser) is the empty [category](../../../category.md). But their images under $C=\pi_0$ are the same function between singleton [sets](../../../set.md), whose [equalizer](../../../category.md#equaliser) is a singleton. Hence $C$ does not preserve [equalizers](../../../category.md#equaliser) and has no further [left adjoint](../../../category.md#adjoint-functors). Finally, $I1\amalg I1$ is the two-object [discrete category](../../../category.md#discrete-category), while $I(1\amalg1)$ has arrows between its distinct objects. The canonical comparison is not an [isomorphism of categories](../../../category.md#isomorphism-of-categories), so $I$ fails to preserve this [coproduct](../../../category.md#coproduct) and has no further [right adjoint](../../../category.md#adjoint-functors).

**Neither chain extends in either direction.**

## 3

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\mathcal C$ be a [locally small category](../../../category.md#locally-small-category), let $h_A=\mathcal C(-,A)$ be a [representable presheaf](../../../category.md#representable-functor), and let $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$. The [Yoneda lemma](../../../category.md#yoneda-lemma) gives a [bijection](../../../function.md#bijection), natural in $A$ and $X$,

$$
\boxed{\operatorname{Nat}(h_A,X)\cong X(A),\qquad
\alpha\longmapsto\alpha_A(1_A).}
$$

For $x\in X(A)$, define a [natural transformation](../../../category.md#natural-transformation) $\alpha^x:h_A\to X$ by

$$
\alpha^x_B(f)=X(f)(x)\qquad(f:B\to A).
$$

For $v:C\to B$, the [functor](../../../category.md#functor) composition law gives $X(v)\alpha^x_B(f)=X(fv)(x)=\alpha^x_C(fv)$, proving [naturality](../../../category.md#naturality). Conversely, naturality of any $\alpha:h_A\to X$ along $f:B\to A$ gives

$$
\alpha_B(f)=X(f)\alpha_A(1_A).
$$

Thus $\alpha$ is determined by its displayed element, and $\alpha^x_A(1_A)=x$ proves that the constructions are inverse.

A [natural transformation](../../../category.md#natural-transformation) $\theta:X\to Y$ sends the element to $\theta_A(x)$, which corresponds to $\theta\alpha^x$. A [morphism](../../../algebra.md#morphism) $u:A'\to A$ induces $h_u:h_{A'}\to h_A$; precomposition by $h_u$ sends the element to $X(u)(x)$. This proves naturality in both variables and completes the [Yoneda lemma](../../../category.md#yoneda-lemma) proof.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [Yoneda embedding](../../../category.md#yoneda-embedding) sends $A$ to $h_A=\mathcal C(-,A)$ and $u:A\to B$ to postcomposition $h_u:h_A\to h_B$. Apply the [Yoneda lemma](../../../category.md#yoneda-lemma) with $X=h_B$:

$$
\operatorname{Nat}(h_A,h_B)\cong h_B(A)=\mathcal C(A,B).
$$

The inverse sends $u$ precisely to $h_u$, because its component at $C$ maps $f:C\to A$ to $uf$. Hence the induced maps on all [hom-sets](../../../category.md#hom-set) are [bijections](../../../function.md#bijection). **The Yoneda embedding is full and faithful.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

An [isomorphism](../../../algebra.md#isomorphism) $f:A\to B$ gives a [natural isomorphism](../../../category.md#natural-isomorphism) $h_f:h_A\to h_B$ by postcomposition, with inverse $h_{f^{-1}}$.

Conversely suppose $\alpha:h_A\to h_B$ is a [natural isomorphism](../../../category.md#natural-isomorphism), with inverse $\beta$. Since the [Yoneda embedding](../../../category.md#yoneda-embedding) is a [full and faithful functor](../../../category.md#full-and-faithful-functor), there are unique $f:A\to B$ and $g:B\to A$ with $h_f=\alpha$ and $h_g=\beta$. Their composites satisfy

$$
h_{gf}=\beta\alpha=1_{h_A}=h_{1_A},\qquad
h_{fg}=\alpha\beta=1_{h_B}=h_{1_B}.
$$

Faithfulness gives $gf=1_A$ and $fg=1_B$. Thus

$$
\boxed{A\cong B\quad\Longleftrightarrow\quad
\mathcal C(-,A)\cong\mathcal C(-,B)\text{ naturally}.}
$$

The [naturality](../../../category.md#naturality) requirement ensures that all incoming [morphisms](../../../algebra.md#morphism) are respected; unrelated componentwise [bijections](../../../function.md#bijection) alone would not justify the conclusion.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Here a [universal element](../../../category.md#universal-element-of-a-set-valued-functor) means a pair $(A,u)$, with $u\in X(A)$, such that for every $B$ and every $x\in X(B)$ there is a unique [morphism](../../../algebra.md#morphism) $f:B\to A$ satisfying $X(f)(u)=x$. Equivalently,

$$
\boxed{\mathcal C(B,A)\longrightarrow X(B),\quad f\longmapsto X(f)(u)
\text{ is bijective for every }B.}
$$

By the [Yoneda lemma](../../../category.md#yoneda-lemma) these component maps constitute a [natural transformation](../../../category.md#natural-transformation) $h_A\to X$. If $u$ is universal, every component is bijective, so this is a [natural isomorphism](../../../category.md#natural-isomorphism) and $X$ is a [representable presheaf](../../../category.md#representable-functor). Conversely a [natural isomorphism](../../../category.md#natural-isomorphism) $h_A\to X$ takes $1_A$ to an element $u$ with exactly this property. In the [category of elements](../../../category.md#category-of-elements) of the contravariant [functor](../../../category.md#functor) $X$, $(A,u)$ is a [terminal object](../../../category.md#terminal-object): every $(B,x)$ has a unique arrow to it.

## 4

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

First construct every finite [product in a category](../../../category.md#product-category-theory) by iterating binary [products in a category](../../../category.md#product-category-theory); the empty product is the [terminal object](../../../category.md#terminal-object). Let $D:J\to\mathcal C$ be a [diagram in a category](../../../category.md#diagram-category-theory) with finitely many objects and arrows. Form the finite [products in a category](../../../category.md#product-category-theory)

$$
P=\prod_{j\in\operatorname{Ob}J}D(j),\qquad
Q=\prod_{u:i\to j\text{ in }J}D(j).
$$

Define $a,b:P\rightrightarrows Q$ by their components

$$
\pi_u a=D(u)\pi_i,\qquad \pi_u b=\pi_j.
$$

Take their [equalizer](../../../category.md#equaliser) $e:L\to P$. Its components $p_j=\pi_j e$ satisfy $D(u)p_i=p_j$, so they form a [cone over a diagram](../../../category.md#cone-over-a-diagram).

For any other [categorical cone](../../../category.md#cone-over-a-diagram) $x_j:X\to D(j)$, the [product in a category](../../../category.md#product-category-theory) property supplies a unique $x:X\to P$ with $\pi_jx=x_j$. The cone equations imply $ax=bx$, so the [equalizer](../../../category.md#equaliser) property supplies a unique $\bar x:X\to L$ with $e\bar x=x$. These are exactly the required equations $p_j\bar x=x_j$, with uniqueness. Thus $L$ is a [categorical limit](../../../category.md#categorical-limit). For empty $J$, both products are terminal and this construction still gives a terminal limit. **All finite limits exist.**

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Use the explicit [construction of small limits from products and equalizers](../../../category.md#construction-of-small-limits-from-products-and-equalizers) from part (i), here with finite indexing [sets](../../../set.md). If $F$ preserves finite [products in a category](../../../category.md#product-category-theory) and [equalizers](../../../category.md#equaliser), then $F(P)$ and $F(Q)$, with their image projections, are the products of the objects $FD(j)$ and of the target objects indexed by arrows of $J$.

The image maps $F(a),F(b)$ have components

$$
F(\pi_u)F(a)=FD(u)F(\pi_i),\qquad
F(\pi_u)F(b)=F(\pi_j).
$$

Also $F(e):F(L)\to F(P)$ is their [equalizer](../../../category.md#equaliser). Therefore the same [universal property](../../../category-theory.md#universal-property) proof makes $F(L)$, with projections $F(p_j)$, a [categorical limit](../../../category.md#categorical-limit) of $FD$. Any other chosen limit of $D$ is uniquely [isomorphic](../../../algebra.md#isomorphism) to this construction, and the [functor](../../../category.md#functor) carries that isomorphism to an isomorphism. **Consequently $F$ preserves every finite limit.** Preservation of finite products includes the empty product, so the [terminal object](../../../category.md#terminal-object) is also preserved.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Given $A,B$, their [product in a category](../../../category.md#product-category-theory) is the [pullback](../../../category.md#pullback-category-theory) of the unique arrows $A\to1\leftarrow B$, where $1$ is a [terminal object](../../../category.md#terminal-object). Having constructed this [product in a category](../../../category.md#product-category-theory), define the [equalizer](../../../category.md#equaliser) of $f,g:A\rightrightarrows B$ as the [pullback](../../../category.md#pullback-category-theory)

$$
\begin{array}{ccc}
E&\longrightarrow&B\\
\downarrow&&\downarrow\scriptstyle\delta_B\\
A&\xrightarrow{(f,g)}&B\times B,
\end{array}
$$

where $\delta_B$ is the [categorical diagonal](../../../category.md#categorical-diagonal). A map $x:X\to A$ factors through this [pullback](../../../category.md#pullback-category-theory) exactly when $fx=gx$: the accompanying arrow to $B$ must equal this common composite. The factorization is unique, proving the [equalizer](../../../category.md#equaliser) property.

Thus the hypotheses give a [terminal object](../../../category.md#terminal-object), binary [products in a category](../../../category.md#product-category-theory) and all [equalizers](../../../category.md#equaliser). Part (i) now gives **all finite limits**.

## 5

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $D:J\to[\mathcal C,\mathcal S]$ be a small [diagram in a category](../../../category.md#diagram-category-theory). Since $\mathcal S$ is a [complete category](../../../category.md#complete-category), choose at each $C\in\mathcal C$ a [categorical limit](../../../category.md#categorical-limit)

$$
L(C)=\lim_{j\in J}D_j(C),\qquad p_{j,C}:L(C)\to D_j(C).
$$

For $f:C\to C'$, the arrows $D_j(f)p_{j,C}$ form a [cone over a diagram](../../../category.md#cone-over-a-diagram) at $C'$, because the diagram arrows $D_j\to D_k$ are [natural transformations](../../../category.md#natural-transformation). There is therefore a unique arrow $L(f):L(C)\to L(C')$ with

$$
p_{j,C'}L(f)=D_j(f)p_{j,C}.
$$

The [universal property](../../../category-theory.md#universal-property) immediately gives $L(1_C)=1_{L(C)}$ and $L(gf)=L(g)L(f)$: both sides have the same composites with every limit projection. Thus $L$ is a [functor](../../../category.md#functor), and the displayed equations make the $p_j$ [natural transformations](../../../category.md#natural-transformation).

Given any [categorical cone](../../../category.md#cone-over-a-diagram) $q_j:X\to D_j$ in the [functor category](../../../category.md#functor-category), its components induce unique $q_C:X(C)\to L(C)$. For $f:C\to C'$, compare $L(f)q_C$ and $q_{C'}X(f)$ after each $p_{j,C'}$; [naturality](../../../category.md#naturality) of $q_j$ makes their composites equal. Hence $q$ is a [natural transformation](../../../category.md#natural-transformation), and uniqueness is componentwise. This proves that $L$ is a [categorical limit](../../../category.md#categorical-limit) in $[\mathcal C,\mathcal S]$.

**The functor category is complete, and every evaluation functor preserves limits**, since evaluating the constructed limit at $C$ gives exactly the chosen limit in $\mathcal S$. This is the [pointwise limits in a functor category](../../../category.md#pointwise-limits-in-a-functor-category) construction; it also covers the empty diagram and its [terminal object](../../../category.md#terminal-object).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Let $a:X\to Y$ be a [natural transformation](../../../category.md#natural-transformation) of [categorical presheaves](../../../category.md#presheaf-category-theory). If every $a_C:X(C)\to Y(C)$ is a [surjective function](../../../algebra.md#surjective-function), and $r,s:Y\rightrightarrows Z$ satisfy $ra=sa$, then $r_Ca_C=s_Ca_C$ at every $C$. Surjectivity gives $r_C=s_C$ for all $C$, hence $r=s$. Thus $a$ is an [epimorphism](../../../category.md#epimorphism).

Conversely suppose $y\in Y(C)$ is outside the image of some $a_C$. Construct the [pushout witness for failure of pointwise surjectivity](../../../category.md#pushout-witness-for-failure-of-pointwise-surjectivity) explicitly: at each $D$ take

$$
P(D)=\bigl(Y(D)\times\{0,1\}\bigr)/\sim,
\qquad (a_D(x),0)\sim(a_D(x),1).
$$

Restrictions send $[(z,k)]$ to $[(Y(f)z,k)]$; [naturality](../../../category.md#naturality) of $a$ ensures that every generating identification is respected. Thus $P$ is a [categorical presheaf](../../../category.md#presheaf-category-theory), and the two inclusions $j_0,j_1:Y\to P$ are [natural transformations](../../../category.md#natural-transformation) with $j_0a=j_1a$.

All identifications concern the same element $z$ in its two copies, so an element outside the image is never identified with its other copy. Consequently $j_{0,C}(y)\ne j_{1,C}(y)$, proving $a$ is not an [epimorphism](../../../category.md#epimorphism). Therefore

$$
\boxed{a\text{ is epic}\quad\Longleftrightarrow\quad
\text{every }a_C\text{ is surjective}.}
$$

This is the [pointwise epimorphism in a functor category](../../../category.md#pointwise-epimorphism-in-a-functor-category) criterion. It requires neither a componentwise choice of preimages nor a natural section.

## 6

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

For $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$, let $\int X$ be its [category of elements](../../../category.md#category-of-elements). Its objects are $(A,a)$ with $a\in X(A)$; an arrow $(A,a)\to(B,b)$ is a [morphism](../../../algebra.md#morphism) $f:A\to B$ satisfying $X(f)b=a$. This is a [small category](../../../category.md#small-category), because $\mathcal C$ is small and all values of $X$ are [sets](../../../set.md).

Send $(A,a)$ to the [representable presheaf](../../../category.md#representable-functor) $h_A$, and send an arrow $f$ to postcomposition $h_f$. There is a [cocone](../../../category.md#cocone-under-a-diagram) to $X$ whose map at $(A,a)$ is

$$
\iota_{A,a}:h_A\to X,\qquad
(\iota_{A,a})_C(g)=X(g)a.
$$

The [functor](../../../category.md#functor) laws give its [naturality](../../../category.md#naturality) and the required [cocone](../../../category.md#cocone-under-a-diagram) compatibility.

Compute the [colimit](../../../category.md#colimit) pointwise as a disjoint union modulo its diagram identifications. At $C$ a representative is a triple $(A,a,g:C\to A)$, and it maps to $X(g)a\in X(C)$. Every $x\in X(C)$ is the image of $(C,x,1_C)$. Moreover $g$ is an arrow $(C,X(g)a)\to(A,a)$ in $\int X$, so its diagram relation identifies

$$
(A,a,g)\sim(C,X(g)a,1_C).
$$

Thus every representative is identified with the canonical representative of its image. Two representatives have equal images exactly when their canonical representatives agree. This proves a componentwise [bijection](../../../function.md#bijection); restriction maps respect it. The resulting [natural isomorphism](../../../category.md#natural-isomorphism) is the [canonical colimit presentation of a presheaf](../../../category.md#canonical-colimit-presentation-of-a-presheaf):

$$
\boxed{X\cong\operatorname{colim}_{(A,a)\in\int X}h_A.}
$$

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

A [Cartesian closed category](../../../category.md#cartesian-closed-category) has finite [products in a category](../../../category.md#product-category-theory) and, for all $X,Y$, an [exponential object](../../../category.md#exponential-object) $Y^X$ with a [natural bijection](../../../category.md#natural-bijection)

$$
\mathcal E(Z,Y^X)\cong\mathcal E(Z\times X,Y).
$$

Equivalently the [functor](../../../category.md#functor) $-\times X$ has a [right adjoint](../../../category.md#adjoint-functors). Its [counit of an adjunction](../../../category.md#counit-of-an-adjunction) is the [evaluation map of an exponential object](../../../category.md#evaluation-map-of-an-exponential-object) $Y^X\times X\to Y$.

For the [presheaf category](../../../category.md#presheaf-category), define the [exponential in a presheaf category](../../../category.md#exponential-in-a-presheaf-category) by

$$
\boxed{(Y^X)(C)=\operatorname{Nat}(h_C\times X,Y).}
$$

For $f:D\to C$, its restriction sends $\alpha$ to $\alpha\circ(h_f\times1_X)$. Composition of these restriction maps follows from composition of the $h_f$, so this is a [categorical presheaf](../../../category.md#presheaf-category-theory). Define [evaluation map of an exponential object](../../../category.md#evaluation-map-of-an-exponential-object) by

$$
e_C(\alpha,x)=\alpha_C(1_C,x).
$$

For $f:D\to C$, naturality of $\alpha$ gives

$$
Y(f)\alpha_C(1_C,x)=\alpha_D(f,X(f)x)
=e_D\bigl((Y^X)(f)\alpha,X(f)x\bigr).
$$

Thus $e$ is a [natural transformation](../../../category.md#natural-transformation).

Given a [natural transformation](../../../category.md#natural-transformation) $\beta:Z\times X\to Y$, define its [currying](../../../category.md#currying) by

$$
\widehat\beta_C(z)_D(g,x)=\beta_D(Z(g)z,x),
\qquad g:D\to C,\quad x\in X(D).
$$

[Naturality](../../../category.md#naturality) of $\beta$ proves that $\widehat\beta_C(z)$ is a natural transformation $h_C\times X\to Y$. For $f:C'\to C$, the same formula proves that $\widehat\beta:Z\to Y^X$ is natural. Evaluating at $g=1_C$ gives $e(\widehat\beta\times1_X)=\beta$.

Conversely, if $\gamma:Z\to Y^X$ and $\beta=e(\gamma\times1_X)$, then

$$
\widehat\beta_C(z)_D(g,x)=\gamma_D(Z(g)z)_D(1_D,x)
=\gamma_C(z)_D(g,x),
$$

by naturality of $\gamma$. Hence the two constructions are inverse and natural in $Z,Y$. Products are available pointwise, including the terminal singleton presheaf, so **the presheaf category is Cartesian closed**. The exponential uses [natural transformations](../../../category.md#natural-transformation) out of $h_C\times X$; simply exponentiating the individual values generally does not give this object.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

Write the [Yoneda embedding](../../../category.md#yoneda-embedding) as $h:\mathcal C\to\widehat{\mathcal C}$. For any finite [product in a category](../../../category.md#product-category-theory), its [universal property](../../../category-theory.md#universal-property) gives

$$
h_{A\times B}(D)=\mathcal C(D,A\times B)
\cong\mathcal C(D,A)\times\mathcal C(D,B),\qquad h_1(D)\cong1.
$$

These [bijections](../../../function.md#bijection) are natural, so $h$ preserves finite products. Now use the [exponential in a presheaf category](../../../category.md#exponential-in-a-presheaf-category), followed by the [Yoneda lemma](../../../category.md#yoneda-lemma) and the [exponential object](../../../category.md#exponential-object) property in $\mathcal C$:

$$
\begin{aligned}
(h_B)^{h_A}(D)
&=\operatorname{Nat}(h_D\times h_A,h_B)\\
&\cong\operatorname{Nat}(h_{D\times A},h_B)\\
&\cong\mathcal C(D\times A,B)\\
&\cong\mathcal C(D,B^A)=h_{B^A}(D).
\end{aligned}
$$

Every step is natural in $D$, so these component [bijections](../../../function.md#bijection) form a [natural isomorphism](../../../category.md#natural-isomorphism)

$$
\boxed{h_{B^A}\cong(h_B)^{h_A}.}
$$

Under this isomorphism, the image of the evaluation $B^A\times A\to B$ is the presheaf evaluation: both correspond to the same identity of the exponential under the transpose [bijection](../../../function.md#bijection). Thus the [Yoneda embedding preserves exponentials](../../../category.md#yoneda-embedding-preserves-exponentials), including their evaluation maps.

## 7

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

If $F\dashv U$, let $1$ denote a singleton [set](../../../set.md). The [adjunction](../../../category.md#adjoint-functors) gives the natural [bijections](../../../function.md#bijection)

$$
U(C)\cong\mathbf{Set}(1,U(C))\cong\mathcal C(F1,C).
$$

Thus **$U$ is represented by $F1$**, proving $A\Rightarrow R$.

If $U\cong\mathcal C(R,-)$ is a covariant [representable functor](../../../category.md#representable-functor), a [morphism](../../../algebra.md#morphism) $R\to\lim_jC_j$ is exactly a compatible family of [morphisms](../../../algebra.md#morphism) $R\to C_j$. Consequently the comparison map

$$
\mathcal C(R,\lim_jC_j)\longrightarrow\lim_j\mathcal C(R,C_j)
$$

is a [bijection](../../../function.md#bijection) for every existing small [categorical limit](../../../category.md#categorical-limit). This proves $R\Rightarrow L$ by the [universal property](../../../category-theory.md#universal-property) of a limit. In particular,

$$
\boxed{A\Rightarrow R\Rightarrow L.}
$$

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

Suppose $U(C)\cong\mathcal C(R,C)$ naturally and $\mathcal C$ has small [coproducts in a category](../../../category.md#coproduct). Define

$$
F(X)=\coprod_{x\in X}R.
$$

For a function $v:X\to Y$, define $F(v)$ by sending the $x$-summand by the identity of $R$ to the $v(x)$-summand. The [coproduct](../../../category.md#coproduct) property gives the identity and composition laws, so $F$ is a [functor](../../../category.md#functor). There are natural [bijections](../../../function.md#bijection)

$$
\mathcal C(F(X),C)\cong\prod_{x\in X}\mathcal C(R,C)
\cong\mathbf{Set}(X,U(C)).
$$

The first chooses a [morphism](../../../algebra.md#morphism) on every summand; the second views that family as a function. Hence this is the [left adjoint to a covariant representable functor](../../../category.md#left-adjoint-to-a-covariant-representable-functor):

$$
\boxed{F\dashv U,\qquad F(X)=\coprod_{x\in X}R.}
$$

For empty $X$, the formula uses the empty [coproduct](../../../category.md#coproduct), an [initial object](../../../category.md#initial-object), and the same bijection remains valid.

<h3 id="7/iii">iii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7/iii)

Only $L\Rightarrow A$ remains. Assume $U$ preserves small [categorical limits](../../../category.md#categorical-limit), and choose a [small cogenerating family](../../../category.md#cogenerating-set) $(Q_i)_{i\in I}$ in $\mathcal C$. Fix a [set](../../../set.md) $X$. The [comma category](../../../category.md#comma-category) $(X\downarrow U)$ is a [complete category](../../../category.md#complete-category): underlying limits in $\mathcal C$, together with limit preservation by $U$, lift compatible maps from $X$. It is [locally small](../../../category.md#locally-small-category), since its arrows form subsets of the [hom-sets](../../../category.md#hom-set) in $\mathcal C$.

We construct a [weakly initial set](../../../category.md#weakly-initial-set) in this comma category. Given $f:X\to U(C)$, intersect all [subobjects](../../../category.md#subobject) $m:B\hookrightarrow C$ through which $f$ lifts under $U$. There are only a [set](../../../set.md) of subobjects because $\mathcal C$ is [well-powered](../../../category.md#well-powered-category); the family includes $1_C$. Their intersection exists by completeness. Also $U$ preserves [monomorphisms](../../../category.md#monomorphism), since a map is monic precisely when its self-pullback diagonal is invertible, and $U$ preserves such [pullbacks](../../../category.md#pullback-category-theory).

Thus all lifts of $f$ are unique and compatible, and preservation of the intersection gives

$$
f=U(m_0)f_0,\qquad m_0:C_0\hookrightarrow C.
$$

No proper [subobject](../../../category.md#subobject) of $C_0$ supports a lift of $f_0$: its composite into $C$ would belong to the intersected family, forcing it to contain $C_0$. This is a [minimal supported subobject](../../../category.md#minimal-supported-subobject).

For each $i$, the map

$$
\mathcal C(C_0,Q_i)\longrightarrow\mathbf{Set}(X,UQ_i),\qquad
h\longmapsto U(h)f_0
$$

is [injective](../../../algebra.md#injective-function). Indeed, equal images mean $f_0$ lifts to the [equalizer](../../../category.md#equaliser) of the two maps, because $U$ preserves that equalizer. Minimality forces the equalizer to be invertible, so the maps agree.

The [cogenerator](../../../category.md#coseparator) property makes the evaluation map

$$
C_0\longrightarrow\prod_{i\in I,\ h:C_0\to Q_i}Q_i
$$

a [monomorphism](../../../category.md#monomorphism): any two arrows into $C_0$ that agree after all these projections are equal. The indexing pairs $(i,h)$ inject into the fixed set

$$
B_X=\coprod_{i\in I}\mathbf{Set}(X,UQ_i).
$$

Their image is some subset $J\subseteq B_X$. Consequently $C_0$ is isomorphic to a [subobject](../../../category.md#subobject) of a product $P_J$ of the $Q_i$ indexed by $J$. There are only a set of such subsets $J$, only a set of subobjects of each $P_J$, and only a set of maps $X\to U(B)$ for each representative subobject $B$.

Collect all these pairs $(B,x:X\to U(B))$. Every $(C,f)$ receives a comma arrow from one of them, via the isomorphic copy of $(C_0,f_0)$ and $m_0$. Hence they form a [weakly initial set](../../../category.md#weakly-initial-set). The [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set), proved explicitly in Question 8, gives an initial object of $(X\downarrow U)$. Its map from $X$ is a [universal arrow from an object to a functor](../../../category.md#universal-arrow-from-an-object-to-a-functor). Choosing these universal arrows for all $X$ defines a [left adjoint](../../../category.md#adjoint-functors) to $U$.

Thus

$$
\boxed{A\Longleftrightarrow R\Longleftrightarrow L.}
$$

The products indexed by realized subsets $J$ are important: one cannot assume that $C_0$ has a map to every cogenerator and simply add arbitrary missing coordinates.

## 8

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

The [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) says that, for a [functor](../../../category.md#functor) $U:\mathcal C\to\mathcal D$ with $\mathcal C$ a [complete category](../../../category.md#complete-category) and both categories [locally small](../../../category.md#locally-small-category), $U$ has a [left adjoint](../../../category.md#adjoint-functors) exactly when it preserves small [categorical limits](../../../category.md#categorical-limit) and satisfies the [solution-set condition](../../../category.md#solution-set-condition). The latter means that for each $D\in\mathcal D$ there is a set of arrows $f_i:D\to U(C_i)$ such that every $f:D\to U(C)$ factors as

$$
f=U(h)f_i\quad\text{for some }i\text{ and }h:C_i\to C.
$$

Equivalently, $(D\downarrow U)$ has a [weakly initial set](../../../category.md#weakly-initial-set).

The [limit form of the special adjoint functor theorem](../../../category.md#limit-form-of-the-special-adjoint-functor-theorem) says that, if in addition $\mathcal C$ is [well-powered](../../../category.md#well-powered-category) and has a [small cogenerating family](../../../category.md#cogenerating-set), then **$U$ has a left adjoint exactly when it preserves small limits**. These are the limit/left-adjoint forms; their duals interchange limits with [colimits](../../../category.md#colimit), left with [right adjoints](../../../category.md#adjoint-functors), and cogenerators with generators.

For the first route, let $\mathcal E$ be a [complete category](../../../category.md#complete-category) that is [locally small](../../../category.md#locally-small-category) and has a [weakly initial set](../../../category.md#weakly-initial-set) $(W_i)$. Put $P=\prod_iW_i$. It is weakly initial: for any $X$, choose an arrow $W_i\to X$ and precompose with the corresponding product projection. The [set](../../../set.md) $\mathcal E(P,P)$ indexes a simultaneous [equalizer](../../../category.md#equaliser)

$$
e:E\longrightarrow P,\qquad ue=e\quad\text{for every }u:P\to P.
$$

It exists by completeness, for example as the equalizer of the two maps $P\rightrightarrows\prod_{u:P\to P}P$ with components $u$ and $1_P$. Since $E\to P\to X$ exists for each $X$, $E$ is also weakly initial.

Choose $r:P\to E$. Applying the defining equation to $er:P\to P$ gives $ere=e$, whence $re=1_E$ because $e$ is a [monomorphism](../../../category.md#monomorphism). If $v:E\to E$ is any endomorphism, apply it to $evr:P\to P$ to obtain $evre=e$, hence $ev=e$ and $v=1_E$. Thus $E$ has only its identity endomorphism.

For two arrows $a,b:E\rightrightarrows X$, take their [equalizer](../../../category.md#equaliser) $j:Y\to E$. Weak initiality of $E$ gives $t:E\to Y$. Since $jt$ is an endomorphism of $E$, $jt=1_E$. The monic arrow $j$ with this right inverse is invertible; therefore $a=b$. Existence of an arrow $E\to X$ and this uniqueness show that **$E$ is initial**.

For the [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem), limit preservation makes each [comma category](../../../category.md#comma-category) $(D\downarrow U)$ complete, and the [solution-set condition](../../../category.md#solution-set-condition) makes it weakly initially generated by a set. The lemma provides an [initial object](../../../category.md#initial-object) $(FD,\eta_D)$. For $v:D\to D'$, the [universal property](../../../category-theory.md#universal-property) uniquely defines $Fv:FD\to FD'$ by

$$
U(Fv)\eta_D=\eta_{D'}v.
$$

Uniqueness gives the [functor](../../../category.md#functor) laws. The same property gives natural [bijections](../../../function.md#bijection)

$$
\mathcal C(FD,C)\cong\mathcal D(D,UC),
$$

so $F\dashv U$. Conversely a [right adjoint](../../../category.md#adjoint-functors) preserves limits, by applying its [hom-set](../../../category.md#hom-set) bijections to cones, and its unit $(FD,\eta_D)$ is already an initial object of each comma category, hence a singleton solution set. This proves necessity as well as sufficiency.

For the second route, assume the [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) and the additional hypotheses of the [Special adjoint functor theorem](../../../category.md#special-adjoint-functor-theorem). Let $(Q_i)_{i\in I}$ be a [small cogenerating family](../../../category.md#cogenerating-set). Fix $D\in\mathcal D$ and an arrow $f:D\to UC$. A limit-preserving [functor](../../../category.md#functor) preserves [monomorphisms](../../../category.md#monomorphism), by the self-pullback criterion. Intersect the set of all [subobjects](../../../category.md#subobject) $B\hookrightarrow C$ supporting $f$. Preservation of this [categorical limit](../../../category.md#categorical-limit) gives a minimal supporting pair $(C_0,f_0:D\to UC_0)$ and a monomorphism $m_0:C_0\to C$ with $U(m_0)f_0=f$.

If $g,h:C_0\rightrightarrows Q_i$ have $Ug f_0=Uh f_0$, their [equalizer](../../../category.md#equaliser) supports $f_0$ and must be invertible by minimality. Thus

$$
\mathcal C(C_0,Q_i)\hookrightarrow\mathcal D(D,UQ_i),\qquad
h\longmapsto Uh f_0.
$$

The evaluation map into the product of all these cogenerator targets is monic, because the family coseparates arrows. Its coordinates inject into the fixed set

$$
B_D=\coprod_{i\in I}\mathcal D(D,UQ_i).
$$

For every subset $J\subseteq B_D$, form the product $P_J$ whose coordinate $(i,z)$ has target $Q_i$. Each minimal $C_0$ is isomorphic to a [subobject](../../../category.md#subobject) of one such product, using precisely its realized coordinates. There is a set of subsets $J$; the [well-powered category](../../../category.md#well-powered-category) condition gives a set of representative subobjects of each product. For each representative $B$, include every arrow $D\to UB$, a set by local smallness of $\mathcal D$.

This is a [solution-set condition](../../../category.md#solution-set-condition): the minimal pair is isomorphic to one of these representatives, and its inclusion into $C$ supplies the required factorization of $f$. The [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) now gives the [left adjoint](../../../category.md#adjoint-functors). This is the [cogenerator bound for comma-category solution sets](../../../category.md#cogenerator-bound-for-comma-category-solution-sets) proof of the special theorem. Necessity follows again because a [right adjoint](../../../category.md#adjoint-functors) preserves limits. Both alternative proof routes are therefore supplied.

## 9

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="9/i">i</h3>

↑ **Parent:** [9](#9)

<h4 id="9/i/solution">Solution</h4>

↑ **Parent:** [I](#9/i)

A [monad](../../../category-theory.md#monad) on $\mathcal C$ consists of an [endofunctor](../../../category.md#endofunctor) $T$ and [natural transformations](../../../category.md#natural-transformation) $\eta:1\to T$, $\mu:T^2\to T$ satisfying the [unit and multiplication of a monad](../../../category-theory.md#unit-and-multiplication-of-a-monad) laws

$$
\boxed{\mu\circ T\eta=1_T=\mu\circ\eta T,\qquad
\mu\circ T\mu=\mu\circ\mu T.}
$$

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is an object $A$ equipped with $a:TA\to A$ such that

$$
a\eta_A=1_A,\qquad aT(a)=a\mu_A.
$$

A [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad) $f:(A,a)\to(B,b)$ is a [morphism](../../../algebra.md#morphism) $f:A\to B$ satisfying $fa=bT(f)$. Identities and composition obey this equation, giving the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^T$ and its [forgetful functor](../../../category.md#forgetful-functor) $U^T(A,a)=A$.

For an [adjunction](../../../category.md#adjoint-functors) $F\dashv U:\mathcal D\to\mathcal C$ with induced [monad](../../../category-theory.md#monad) $T=UF$, the [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) is

$$
K:\mathcal D\to\mathcal C^T,\qquad
K(D)=(UD,U\varepsilon_D),\quad K(h)=Uh.
$$

The [functor](../../../category.md#functor) $U$ is monadic when it has such a [left adjoint](../../../category.md#adjoint-functors) and this comparison is an [equivalence of categories](../../../category.md#equivalence-of-categories); a stricter convention requires an [isomorphism of categories](../../../category.md#isomorphism-of-categories) over $\mathcal C$. We will identify which limit-lifting conclusion each convention supports in part (iii).

<h3 id="9/ii">ii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9/ii)

For $F\dashv U$ with [unit of an adjunction](../../../category.md#unit-of-an-adjunction) $\eta$ and [counit of an adjunction](../../../category.md#counit-of-an-adjunction) $\varepsilon$, put

$$
\boxed{T=UF,\qquad\mu_A=U(\varepsilon_{FA}).}
$$

The [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give

$$
\mu_A\eta_{TA}=1_{TA},\qquad
\mu_AT(\eta_A)=1_{TA}.
$$

For associativity, [naturality](../../../category.md#naturality) of $\varepsilon$ at $\varepsilon_{FA}:FUFA\to FA$ says

$$
\varepsilon_{FA}FU(\varepsilon_{FA})
=\varepsilon_{FA}\varepsilon_{FUFA}.
$$

Apply $U$ to obtain $\mu_AT(\mu_A)=\mu_A\mu_{TA}$. Thus this is the [monad induced by an adjunction](../../../category-theory.md#monad-induced-by-an-adjunction).

Conversely, start with a [monad](../../../category-theory.md#monad) $(T,\eta,\mu)$. The [free algebra functor](../../../category-theory.md#free-algebra-functor) sends $A$ to $(TA,\mu_A)$ and $f$ to $Tf$. The [monad](../../../category-theory.md#monad) laws ensure that these are [algebras for a monad](../../../category-theory.md#algebra-for-a-monad) and [morphisms of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad). For an algebra $(B,b)$, there are inverse [bijections](../../../function.md#bijection)

$$
\mathcal C^T((TA,\mu_A),(B,b))\cong\mathcal C(A,B),
\qquad g\longmapsto g\eta_A,\quad f\longmapsto bT(f).
$$

The inverse really is an algebra map because

$$
bT(f)\mu_A=b\mu_B T^2(f)=bT(b)T^2(f)=bT(bT(f)).
$$

For a free-algebra map $g$, its algebra equation and the [monad](../../../category-theory.md#monad) unit law give

$$
bT(g\eta_A)=bT(g)T(\eta_A)=g\mu_AT(\eta_A)=g.
$$

For a base map $f$, naturality and the algebra unit law give $bT(f)\eta_A=b\eta_Bf=f$. The formulas are natural, establishing the [free-forgetful Eilenberg-Moore adjunction](../../../category-theory.md#free-forgetful-eilenberg-moore-adjunction) $F^T\dashv U^T$. Its unit is $\eta_A$, and its counit at $(B,b)$ is $b$. Hence its induced multiplication is $\mu$, and **every monad arises from an adjunction**.

<h3 id="9/iii">iii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9/iii)

First prove the exact lifting statement for the [forgetful functor](../../../category.md#forgetful-functor) $U^T:\mathcal C^T\to\mathcal C$. Take any [diagram in a category](../../../category.md#diagram-category-theory) of [algebras for a monad](../../../category-theory.md#algebra-for-a-monad) $(A_j,a_j)$ whose underlying diagram has a chosen [categorical limit](../../../category.md#categorical-limit) $p_j:L\to A_j$. The arrows $a_jT(p_j):TL\to A_j$ form a [categorical cone](../../../category.md#cone-over-a-diagram), since every diagram arrow is a [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad). Thus the [universal property](../../../category-theory.md#universal-property) gives a unique arrow $a:TL\to L$ satisfying

$$
\boxed{p_ja=a_jT(p_j)\quad\text{for every }j.}
$$

The projections are jointly monic: two arrows into $L$ with the same composites with every $p_j$ are equal. Therefore the algebra identities can be checked after these projections. For the unit,

$$
p_ja\eta_L=a_jT(p_j)\eta_L=a_j\eta_{A_j}p_j=p_j.
$$

For multiplication,

$$
\begin{aligned}
p_jaT(a)&=a_jT(p_ja)=a_jT(a_j)T^2(p_j),\\
p_ja\mu_L&=a_jT(p_j)\mu_L=a_j\mu_{A_j}T^2(p_j).
\end{aligned}
$$

The algebra law for $a_j$ makes the right-hand sides equal. Thus $(L,a)$ is an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad), and each $p_j$ is a [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad). Its action is unique with this property.

Given an algebra cone $q_j:(B,b)\to(A_j,a_j)$, let $q:B\to L$ be its unique underlying mediating map. Then

$$
p_jqb=q_jb=a_jT(q_j)=p_jaT(q),
$$

so $qb=aT(q)$ by joint monicity. Hence $q$ is an algebra map, proving the lifted cone is limiting. This establishes that the [monad algebra forgetful functor creates limits](../../../category-theory.md#monad-algebra-forgetful-functor-creates-limits), **without any assumption that $T$ preserves limits**.

For a [monadic adjunction](../../../category-theory.md#monadic-adjunction), the comparison satisfies $U=U^TK$. If $K$ is an [isomorphism of categories](../../../category.md#isomorphism-of-categories) over the base, the preceding unique lift transports back literally, so $U$ is a [limit-creating functor](../../../category.md#limit-creating-functor). If monadic means that $K$ is only an [equivalence of categories](../../../category.md#equivalence-of-categories), the precise conclusion is [creation of limits up to isomorphism](../../../category.md#creation-of-limits-up-to-isomorphism): the lifted algebra is isomorphic to an object $K(D)$, and its limiting cone transports along that isomorphism. Full faithfulness supplies the arrows and their uniqueness.

This distinction concerns prescribed underlying objects, not existence of limits. Literal creation does not follow from an arbitrary equivalence alone. For example, the inclusion of the one-object category into the two-object [indiscrete category](../../../category.md#indiscrete-category), choosing one of its objects, is an [equivalence of categories](../../../category.md#equivalence-of-categories) and is monadic under the equivalence convention. Either object of the target is terminal, but the other chosen [terminal object](../../../category.md#terminal-object) has no literal object preimage. Thus the strict reading of the requested assertion needs the strict comparison convention; the equivalence-invariant statement is proved above.

## 10

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

A form of [Beck's monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) compatible with equivalence-based [monadic adjunctions](../../../category-theory.md#monadic-adjunction) is this. A [functor](../../../category.md#functor) $U:\mathcal D\to\mathcal C$ is monadic exactly when it has a [left adjoint](../../../category.md#adjoint-functors), is a [conservative functor](../../../category.md#conservative-functor), and $\mathcal D$ has [coequalizers](../../../category.md#coequalizer) of all pairs whose images under $U$ admit a [split coequalizer](../../../category.md#split-coequalizer), with $U$ preserving these coequalizers. In the strict lifting formulation, one states creation of these coequalizers. Such a pair is a [functor-split coequalizer pair](../../../category.md#functor-split-coequalizer-pair); the splitting is required in the base category, not necessarily upstairs.

A [split coequalizer](../../../category.md#split-coequalizer) fork $A\mathrel{\substack{\xrightarrow{r}\\[-0.4ex]\xrightarrow[s]{}}}B\xrightarrow{q}Q$ has maps $u:B\to A$ and $t:Q\to B$ such that

$$
qr=qs,\qquad qt=1_Q,\qquad ru=1_B,\qquad su=tq.
$$

Every [functor](../../../category.md#functor) preserves this [coequalizer](../../../category.md#coequalizer): if $hr=hs$, then $h=hru=hsu=htq$, and $q$ is split epic, so the factor through $q$ is unique. The same equations remain true after applying any functor.

For necessity, let $U^T:\mathcal C^T\to\mathcal C$ be the [monad algebra](../../../category-theory.md#algebra-for-a-monad) forgetful functor. It has the free-algebra [left adjoint](../../../category.md#adjoint-functors). It reflects [isomorphisms](../../../algebra.md#isomorphism), because if an algebra map $f$ is invertible in $\mathcal C$, the equation $fa=bTf$ rearranges to $f^{-1}b=aT(f^{-1})$.

If two algebra maps $r,s:(A,a)\rightrightarrows(B,b)$ have an underlying [split coequalizer](../../../category.md#split-coequalizer) $q:B\to Q$, then $Tq$ and $T^2q$ are also coequalizers. Since $qb$ equalizes $Tr,Ts$, there is a unique $c:TQ\to Q$ satisfying

$$
cTq=qb.
$$

After composing with the [epimorphism](../../../category.md#epimorphism) $q$, the equation $c\eta_Q=1_Q$ reduces to the unit law for $b$. After composing with the epimorphism $T^2q$, the equation $cT(c)=c\mu_Q$ reduces to $bT(b)=b\mu_B$. Thus $(Q,c)$ is an algebra and $q$ an algebra map. If an algebra map $h:(B,b)\to(Z,z)$ equalizes $r,s$, its unique underlying factor $k:Q\to Z$ satisfies $kc=zTk$: this follows by precomposing with the epimorphism $Tq$. Therefore this is a coequalizer upstairs as well. This proves that the [monad algebra forgetful functor creates split coequalizers](../../../category-theory.md#monad-algebra-forgetful-functor-creates-split-coequalizers). The same properties transport through the comparison [equivalence of categories](../../../category.md#equivalence-of-categories), with the object-lifting convention distinguished in Question 9.

For sufficiency, suppose the three conditions hold, choose $F\dashv U$, and let $T=UF$ with comparison $K$. For each algebra $(X,a)$, consider the pair

$$
FTX\mathrel{\substack{\xrightarrow{F(a)}\\[-0.4ex]\xrightarrow[\varepsilon_{FX}]{}}}FX.
$$

Its image has coequalizer $a:TX\to X$. It is split: take $r=\mu_X$, $s=T(a)$, $q=a$, $u=\eta_{TX}$ and $t=\eta_X$. The [monad](../../../category-theory.md#monad) and algebra laws give

$$
a\mu_X=aT(a),\quad a\eta_X=1_X,\quad
\mu_X\eta_{TX}=1_{TX},\quad T(a)\eta_{TX}=\eta_Xa.
$$

By hypothesis the pair has a coequalizer $q:FX\to D_X$ and $Uq$ is also a coequalizer. Identify $UD_X$ with $X$ using the unique coequalizer isomorphism, so $Uq=a$. Since $q$ is carried by $K$ to an algebra map from the free algebra, the transported action $b:TX\to X$ satisfies

$$
bT(a)=a\mu_X=aT(a).
$$

But $T(a)$ is a [split epimorphism](../../../category.md#split-epimorphism), with right inverse $T(\eta_X)$, so $b=a$. Hence $(X,a)\cong K(D_X)$: the comparison is essentially surjective.

Next, for every $D\in\mathcal D$, put $a_D=U\varepsilon_D$. The [counit of an adjunction](../../../category.md#counit-of-an-adjunction) coequalizes

$$
FTUD\mathrel{\substack{\xrightarrow{F(a_D)}\\[-0.4ex]\xrightarrow[\varepsilon_{FUD}]{}}}FUD.
$$

This follows from naturality of the counit. The image pair has the split coequalizer $a_D$, as above. If $q:FUD\to Q$ is the hypothesized preserved coequalizer, the induced map $h:Q\to D$ has $Uh$ invertible because both $Uq$ and $a_D$ coequalize the same pair. Conservativity makes $h$ invertible. Therefore $\varepsilon_D$ itself is a coequalizer.

Let $f:K(D)\to K(E)$ be an algebra map, so $fa_D=a_ETf$. Set $g=\varepsilon_EF(f):FUD\to E$. Under the [adjunction](../../../category.md#adjoint-functors) transpose bijection, the two composites of $g$ with the displayed presentation pair correspond respectively to $fa_D$ and $a_ETf$. They are equal, so $g$ factors uniquely through $\varepsilon_D$, giving $h:D\to E$ with $h\varepsilon_D=g$. Applying $U$ yields

$$
Uh\,a_D=a_ETf=fa_D.
$$

Since $a_D$ is split epic, $Uh=f$. Thus $K$ is full. If $Uh=Uk$, the transposes of $h\varepsilon_D$ and $k\varepsilon_D$ are equal, so those composites agree. The counit is epic, hence $h=k$; thus $K$ is faithful.

The comparison is full, faithful and essentially surjective, so it is an [equivalence of categories](../../../category.md#equivalence-of-categories). **This proves monadicity.** The argument also explains the role of each hypothesis: split base presentations construct all algebras, and reflection of isomorphisms turns the counit presentations into actual coequalizers upstairs.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
