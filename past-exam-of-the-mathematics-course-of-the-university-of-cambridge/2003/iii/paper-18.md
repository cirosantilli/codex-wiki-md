# Paper 18

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper18.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper18.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
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
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [i](#8/i)
    - [Solution](#8/i/solution)
  - [ii](#8/ii)
    - [Solution](#8/ii/solution)
  - [iii](#8/iii)
    - [Solution](#8/iii/solution)
- [9](#9)
  - [i](#9/i)
    - [Solution](#9/i/solution)
  - [ii](#9/ii)
    - [Solution](#9/ii/solution)
- [10](#10)
  - [i](#10/i)
    - [Solution](#10/i/solution)
  - [ii](#10/ii)
    - [Solution](#10/ii/solution)

## 1

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $H_A=\mathcal C(-,A)$ for a [representable presheaf](../../../category.md#representable-functor). The contravariant [Yoneda lemma](../../../category.md#yoneda-lemma) states that, for every [presheaf on a category](../../../category.md#presheaf-category-theory) $X$, evaluation at the identity is a bijection

$$
\boxed{\operatorname{Nat}(H_A,X)\longrightarrow X(A),\qquad\alpha\longmapsto\alpha_A(1_A),}
$$

natural in both $A$ and $X$. Smallness of $\mathcal C$ ensures the relevant families and natural-transformation collections are sets.

For $x\in X(A)$ define $\alpha^x_B(h)=X(h)(x)$ for each $h:B\to A$. This family is a [natural transformation](../../../category.md#natural-transformation): for $u:B'\to B$, $X(u)\alpha^x_B(h)=X(u)X(h)x=X(hu)x=\alpha^x_{B'}(hu)$. Its identity value is $x$. Conversely, naturality of any $\alpha$ at $h:B\to A$ gives $\alpha_B(h)=X(h)\alpha_A(1_A)$. Thus evaluation and the displayed construction are inverse.

For a map $v:A\to A'$, precomposing a transformation $H_{A'}\to X$ with postcomposition $H_A\to H_{A'}$ corresponds to applying $X(v):X(A')\to X(A)$. For a transformation $\tau:X\to Y$, postcomposition corresponds to $x\mapsto\tau_A(x)$. These identities prove the stated [naturality](../../../category.md#naturality) in both variables.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [Yoneda embedding](../../../category.md#yoneda-embedding) is the [functor](../../../category.md#functor) $H_\bullet:\mathcal C\to[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ sending $A$ to $H_A=\mathcal C(-,A)$ and $f:A\to B$ to postcomposition, $(H_f)_U(h)=fh$. Composition and identities are preserved by associativity and the identity laws in $\mathcal C$.

Apply the [Yoneda lemma](../../../category.md#yoneda-lemma) with $X=H_B$. It gives a bijection $\operatorname{Nat}(H_A,H_B)\cong\mathcal C(A,B)$. The inverse sends $f$ precisely to $H_f$, since $H_B(h)(f)=fh$. Hence every transformation between the representables comes from exactly one morphism of $\mathcal C$. This proves that **$H_\bullet$ is a full and faithful [functor](../../../category.md#functor)**.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

If $f:A\to B$ is a [monomorphism](../../../category.md#monomorphism), every component $\mathcal C(U,A)\to\mathcal C(U,B)$ of $H_f$ is injective by left cancellation. Thus if $H_f\alpha=H_f\beta$ for two [natural transformations](../../../category.md#natural-transformation) into $H_A$, componentwise injectivity forces $\alpha=\beta$, so $H_f$ is monic.

Conversely suppose $H_f$ is monic, and let $a,b:U\to A$ satisfy $fa=fb$. Functoriality gives $H_fH_a=H_fH_b$, hence $H_a=H_b$. The [Yoneda embedding](../../../category.md#yoneda-embedding) is faithful, so $a=b$. This proves

$$
\boxed{H_f\text{ is monic if and only if }f\text{ is monic}.}
$$

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

If $f:A\to B$ has a section $g:B\to A$, functoriality gives $H_fH_g=1_{H_B}$. Thus $H_f$ is a [split epimorphism](../../../category.md#split-epimorphism) and in particular an [epimorphism](../../../category.md#epimorphism).

For the converse, justify the needed pointwise surjectivity directly. Let $I\subseteq H_B$ be the image subpresheaf of $H_f$. Form a new presheaf by taking, at every object, two copies of $H_B(U)$ and identifying their elements in $I(U)$. Restriction maps descend because $I$ is a subpresheaf. The two canonical transformations $j_1,j_2:H_B\to H_B\amalg_IH_B$ agree after $H_f$. If any component of $I$ is proper, an element outside it distinguishes $j_1$ from $j_2$. Therefore epimorphicity forces every component of $H_f$ to be surjective.

In particular, its component at $B$ has $1_B$ in its image: there is $g:B\to A$ with $fg=1_B$. This proves the [Yoneda embedding detects split epimorphisms](../../../category.md#yoneda-embedding-detects-split-epimorphisms) criterion

$$
\boxed{H_f\text{ is epic if and only if }f\text{ is split epic}.}
$$

Ordinary epimorphicity of $f$ alone would not suffice.

## 2

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The diagonal satisfies $pd=qd=1_Y$, so it equalizes the two projections. If $h:Z\to Y\times Y$ satisfies $ph=qh$, put $u=ph=qh$. The [universal property](../../../category-theory.md#universal-property) of the [product in a category](../../../category.md#product-category-theory) gives $h=(u,u)=du$. Any other factor $v$ with $dv=h$ must satisfy $v=pdv=ph=u$. Thus **the diagonal is the [equalizer](../../../category.md#equaliser) of the two product projections**.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Take the [pullback in a category](../../../category.md#pullback-category-theory) of $d_Y$ along $(f,g)$, with maps $e:E\to X$ and $k:E\to Y$ satisfying $(f,g)e=d_Yk$. Applying the two product projections gives $fe=k=ge$, so $e$ equalizes $f,g$.

Given $h:Z\to X$ with $fh=gh$, put $v=fh$. Then $(f,g)h=(v,v)=d_Yv$. The pullback property gives a unique $u:Z\to E$ with $eu=h$ and $ku=v$. Any map satisfying $eu=h$ automatically has $ku=feu=fh=v$, so uniqueness is exactly the [equalizer](../../../category.md#equaliser) uniqueness. Hence **pulling back the diagonal constructs the [equalizer](../../../category.md#equaliser) of $f,g$**.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

A [terminal object](../../../category.md#terminal-object) and [pullbacks in a category](../../../category.md#pullback-category-theory) give a binary product $X\times Y$ by pulling back $X\to1\leftarrow Y$. Repeating this gives every finite product, with the empty product supplied by the [terminal object](../../../category.md#terminal-object). The preceding parts then construct [equalizers](../../../category.md#equaliser) of arbitrary parallel arrows.

For a diagram $D:J\to\mathcal C$ with finitely many objects and arrows, form $P=\prod_{j\in\operatorname{Ob}J}D(j)$ and $Q=\prod_{a:j\to k}D(k)$. Define $r,s:P\to Q$ by $r_a=D(a)\pi_j$ and $s_a=\pi_k$. Their [equalizer](../../../category.md#equaliser) $e:L\to P$ has projections $\pi_je$ satisfying every cone equation. Conversely a [categorical cone](../../../category.md#cone-over-a-diagram) supplies a unique map to $P$, and its cone equations say that this map equalizes $r,s$, hence factors uniquely through $L$. Thus $L$ is the [categorical limit](../../../category.md#categorical-limit). This proves **a [terminal object](../../../category.md#terminal-object) and all pullbacks give all finite limits**, including the empty diagram.

## 3

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a small diagram $F:I\to\mathcal D$ in a [locally small category](../../../category.md#locally-small-category), define its cone [functor](../../../category.md#functor) on $\mathcal D^{\mathrm{op}}$ by

$$
\operatorname{Cone}_F(A)=\operatorname{Nat}(\Delta A,F)\cong\lim_{i\in I}\mathcal D(A,F(i)),
$$

where $\Delta A$ is the constant diagram. Precomposition acts on cone vertices. A [categorical limit](../../../category.md#categorical-limit) is a representation of this [functor](../../../category.md#functor): an object $L$ with natural bijections $\mathcal D(A,L)\cong\operatorname{Cone}_F(A)$. The image of $1_L$ is the universal cone, and the inverse bijection supplies the unique mediating arrow for every cone. Thus the [representable functor](../../../category.md#representable-functor) formulation and the usual terminal-cone [universal property](../../../category-theory.md#universal-property) coincide.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Choose a limit $L_j$ for each diagram $F(-,j)$, with legs $p_{i,j}:L_j\to F(i,j)$. For an arrow $v:j\to j'$, the maps $F(1_i,v)p_{i,j}$ form a cone over $F(-,j')$, since the two-variable [functor](../../../category.md#functor) respects the commuting arrows in $I\times J$. The limit property therefore gives a unique arrow $L(v):L_j\to L_{j'}$ satisfying

$$
p_{i,j'}L(v)=F(1_i,v)p_{i,j}\quad\text{for every }i.
$$

The arrows $L(1_j)$ and $1_{L_j}$ have identical composites with all projections, so they are equal. The same uniqueness shows $L(v'v)=L(v')L(v)$. Hence the assignment extends to a [functor](../../../category.md#functor) $L:J\to\mathcal D$.

For the chosen limit objects and cones it is uniquely determined, literally, by these equations. Changing the choices gives a unique family of [isomorphisms](../../../algebra.md#isomorphism) between the limits compatible with their projections; the equations above show that this family is a [natural isomorphism](../../../category.md#natural-isomorphism) of the resulting [functors](../../../category.md#functor). Thus it is **unique up to a unique cone-compatible natural [isomorphism](../../../algebra.md#isomorphism)**, not independent of choices as an equality of objects.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Let $M=\lim_{j\in J}L_j$ with projections $q_j:M\to L_j$. The composites $p_{i,j}q_j$ form a cone over $F:I\times J\to\mathcal D$: the $I$ equations hold in each inner limit, and the $J$ equations follow from the naturality of $p$ and the outer cone.

Given any cone $a_{i,j}:A\to F(i,j)$, the inner limit property gives unique $b_j:A\to L_j$ with $p_{i,j}b_j=a_{i,j}$. The $J$ cone equations for $a$ force $L(v)b_j=b_{j'}$ by uniqueness of inner mediating arrows. Thus the $b_j$ form a cone to $L$, and there is a unique $b:A\to M$ with $q_jb=b_j$. This factors all $a_{i,j}$, and the two stages of uniqueness prove uniqueness for the whole product diagram. Consequently

$$
\boxed{\lim_{(i,j)\in I\times J}F(i,j)\cong\lim_{j\in J}\lim_{i\in I}F(i,j).}
$$

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The categorical [commutation of iterated categorical limits](../../../category.md#commutation-of-iterated-categorical-limits) theorem is the following. For small categories $I,J$ and a two-variable [functor](../../../category.md#functor) $F:I\times J\to\mathcal D$, if the two collections of inner limits and their outer limits exist, then there are canonical [isomorphisms](../../../algebra.md#isomorphism)

$$
\boxed{\lim_j\lim_iF(i,j)\cong\lim_{I\times J}F\cong\lim_i\lim_jF(i,j).}
$$

In particular all these limits exist if $\mathcal D$ has all $I$-shaped and all $J$-shaped limits. The [isomorphisms](../../../algebra.md#isomorphism) are natural in $F$ and uniquely characterized by preserving every projection to $F(i,j)$.

Part (iii) proves that each iterated limit represents the [functor](../../../category.md#functor) of cones on the product diagram, with the same flattened projections. Two such representations have unique inverse cone-compatible arrows, proving the [isomorphisms](../../../algebra.md#isomorphism). For a [natural transformation](../../../category.md#natural-transformation) $F\to F'$, the two composites in any naturality square have the same product-diagram projections, hence agree by limit uniqueness. This proves naturality as well. Completeness of $\mathcal D$ is a convenient sufficient hypothesis, rather than a necessary one for this individual diagram.

## 4

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $T:\mathcal C^{\mathrm{op}}\times\mathcal C\to\mathcal D$. An [end of a functor](../../../category.md#end-of-a-functor) is an object $E$ with maps $e_C:E\to T(C,C)$ satisfying $T(1_C,f)e_C=T(f,1_D)e_D$ for every $f:C\to D$, universal among all such families. Thus every compatible family with vertex $A$ factors uniquely through $E$. Write it as $\int_CT(C,C)$. These are the wedge equations for a [dinatural transformation](../../../category.md#dinatural-transformation) from a constant [functor](../../../category.md#functor) to $T$.

Dually, a [coend of a functor](../../../category.md#coend-of-a-functor) is an object $Q$ with maps $i_C:T(C,C)\to Q$ satisfying $i_CT(f,1_C)=i_DT(1_D,f)$ as maps from $T(D,C)$, universal among compatible families with a common target. Write it as $\int^CT(C,C)$. These are cowedge equations, and every cowedge to $A$ factors uniquely through $Q$.

For small $\mathcal C$, if the needed products and [equalizers](../../../category.md#equaliser) exist, the end is the [equalizer](../../../category.md#equaliser) of $\prod_CT(C,C)\rightrightarrows\prod_{f:C\to D}T(C,D)$. If the needed coproducts and [coequalizers](../../../category.md#coequalizer) exist, the coend is the [coequalizer](../../../category.md#coequalizer) of $\coprod_{f:C\to D}T(D,C)\rightrightarrows\coprod_CT(C,C)$. The two arrows in each construction are precisely the two sides of the compatibility equation. This explains both the mixed variance and the [universal property](../../../category-theory.md#universal-property), rather than treating the integral notation as an ordinary numerical integral.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For fixed $U$, the [categorical coend](../../../category.md#coend-of-a-functor) on the right is the quotient of $\coprod_W\mathcal C(U,W)\times X(W)$ by the identifications

$$
(fh,x)_V\sim(h,X(f)x)_W\qquad(h:U\to W,\ f:W\to V,\ x\in X(V)).
$$

Define $\Phi_U([h,x])=X(h)x$. This is well defined because the contravariant [functor](../../../category.md#functor) law gives $X(fh)x=X(h)X(f)x$. Its proposed inverse sends $y\in X(U)$ to $[1_U,y]$. The composite to $X(U)$ is the identity. In the other direction the coend relation, applied with $f=h$ and initial map $1_U$, gives $[h,x]=[1_U,X(h)x]$. Thus the inverse is genuine and

$$
\boxed{X(U)\cong\int^W\mathcal C(U,W)\times X(W).}
$$

For $a:U'\to U$, the coend map replaces $h$ by $ha$; its image is $X(ha)x=X(a)X(h)x$, proving naturality in $U$. A morphism of presheaves acts on $x$ and commutes with every $X(h)$ by naturality, proving naturality in $X$. This is the [density formula for presheaves](../../../category.md#density-formula-for-presheaves).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The [category of elements](../../../category.md#category-of-elements) of $X$ has objects $(W,x)$ with $x\in X(W)$ and morphisms $f:(W,x)\to(V,y)$ satisfying $X(f)y=x$. Send $(W,x)$ to the [representable presheaf](../../../category.md#representable-functor) $H_W$ and a morphism to $H_f$. The [Yoneda lemma](../../../category.md#yoneda-lemma) gives a canonical cocone to $X$, whose leg at $(W,x)$ corresponds to $x$.

For any target presheaf $Z$, a cocone from this diagram to $Z$ is a family of maps $H_W\to Z$, or equivalently elements $z_{W,x}\in Z(W)$, with $z_{W,x}=Z(f)z_{V,y}$ whenever $X(f)y=x$. Such a family is exactly a [natural transformation](../../../category.md#natural-transformation) $X\to Z$, via $x\mapsto z_{W,x}$. This bijection respects the canonical cocone, so it proves its [colimit](../../../category.md#colimit) universal property. Consequently the [canonical colimit presentation of a presheaf](../../../category.md#canonical-colimit-presentation-of-a-presheaf) is

$$
\boxed{X\cong\operatorname*{colim}_{(W,x)\in\int X}H_W.}
$$

Equivalently, the density coend identifies the disjoint copies of the representables by exactly these element-category arrows. Smallness of $\mathcal C$ and the set-valued fibers make the indexing category small.

## 5

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Write the [adjunction](../../../category.md#adjoint-functors) bijections as $\Phi_{A,B}:\mathcal D(FA,B)\cong\mathcal C(A,GB)$, natural in $A,B$. The [adjunction unit](../../../category.md#unit-of-an-adjunction) and [adjunction counit](../../../category.md#counit-of-an-adjunction) are

$$
\boxed{\eta_A=\Phi_{A,FA}(1_{FA}),\qquad\varepsilon_B=\Phi_{GB,B}^{-1}(1_{GB}).}
$$

Thus $\eta:1_{\mathcal C}\Rightarrow GF$ and $\varepsilon:FG\Rightarrow1_{\mathcal D}$ are [natural transformations](../../../category.md#natural-transformation), by naturality of the bijections. For any $h:FA\to B$ and $k:A\to GB$, their transposes satisfy

$$
\Phi(h)=Gh\,\eta_A,\qquad\Phi^{-1}(k)=\varepsilon_BFk.
$$

The first follows by naturality in the target applied to $1_{FA}$; the second follows by naturality in the source applied to $1_{GB}$. These formulas make the definitions operational for every arrow.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Apply the inverse transpose formula to $\eta_A$, which by definition is the transpose of $1_{FA}$. This gives $\varepsilon_{FA}F\eta_A=1_{FA}$. Likewise $\varepsilon_B$ transposes to $1_{GB}$, so $G\varepsilon_B\eta_{GB}=1_{GB}$. Hence the [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) are

$$
\boxed{\varepsilon_FF\eta=1_F,\qquad G\varepsilon\eta_G=1_G.}
$$

These are equalities of [natural transformations](../../../category.md#natural-transformation); their components are exactly the two identities just proved.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Given the [natural transformations](../../../category.md#natural-transformation) and triangle identities, define $\Phi(h)=Gh\eta_A$ and $\Psi(k)=\varepsilon_BFk$. Both assignments are natural because $F,G,\eta,\varepsilon$ are natural. Naturality of the counit at $h$ gives

$$
\Psi\Phi(h)=\varepsilon_BFGhF\eta_A=h\varepsilon_{FA}F\eta_A=h.
$$

Naturality of the unit at $k$ similarly gives

$$
\Phi\Psi(k)=G\varepsilon_BGFk\eta_A=G\varepsilon_B\eta_{GB}k=k.
$$

Thus these are inverse natural Hom-set bijections, defining an [adjunction](../../../category.md#adjoint-functors) $F\dashv G$. Their identity values are the prescribed unit and counit, by their definitions. Finally every [adjunction](../../../category.md#adjoint-functors) with this unit must satisfy the first transpose formula, and every one with this counit the second, so the bijections are forced. **There is exactly one [adjunction](../../../category.md#adjoint-functors) structure with these specified unit and counit.**

## 6

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

A presheaf on $0\to1$ is an arrow $r:B=X(1)\to A=X(0)$ in sets. A morphism of presheaves is a commuting square. Define

$$
\Pi(r)=A,\qquad\Gamma(r)=B,\qquad\Delta(S)=(S\xrightarrow1S),\qquad\nabla(S)=(S\to1).
$$

A commuting square from $r$ to $\Delta S$ is determined by its map $A\to S$, while a square from $\Delta S$ to $r$ is determined by its map $S\to B$. A square from $r$ to $\nabla S$ is also determined by its map $B\to S$, because the other component is the unique map $A\to1$. Therefore these Hom-set bijections establish the [adjoint chain for evaluation in an arrow category](../../../category.md#adjoint-chain-for-evaluation-in-an-arrow-category):

$$
\boxed{\Pi\dashv\Delta\dashv\Gamma\dashv\nabla.}
$$

There is a further left adjoint to $\Pi$: $\Lambda(S)=(\varnothing\to S)$. A square $\Lambda S\to r$ is exactly a map $S\to A$, proving $\Lambda\dashv\Pi$.

There is no right adjoint to $\nabla$. If there were, $\nabla$ would be a left adjoint and preserve the [initial object](../../../category.md#initial-object). But it sends the empty set to $(\varnothing\to1)$, whereas the [initial object](../../../category.md#initial-object) of this arrow category is $(\varnothing\to\varnothing)$. They are not isomorphic. Hence **$\Pi$ does have a left adjoint, while $\nabla$ has no right adjoint**.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Let $D(S)$ be the [discrete category](../../../category.md#discrete-category) on $S$, and $I(S)$ the [indiscrete category](../../../category.md#indiscrete-category), with exactly one morphism between each ordered pair of objects. A [functor](../../../category.md#functor) $D(S)\to\mathcal A$ is precisely a map $S\to O(\mathcal A)$; a [functor](../../../category.md#functor) $\mathcal A\to I(S)$ is precisely a map $O(\mathcal A)\to S$. Thus $D\dashv O\dashv I$.

Let $C(\mathcal A)=\pi_0\mathcal A$ be the set of connected components, where objects are related by finite zigzags of morphisms in either direction. A [functor](../../../category.md#functor) $\mathcal A\to D(S)$ must take the endpoints of every morphism to the same point, so it is exactly a map $\pi_0\mathcal A\to S$. This gives the [adjoint chain for the objects of a category](../../../category.md#adjoint-chain-for-the-objects-of-a-category)

$$
\boxed{C\dashv D\dashv O\dashv I.}
$$

It cannot extend to the left. The two [functors](../../../category.md#functor) from the terminal category to $I(\{0,1\})$ selecting distinct objects have empty [equalizer](../../../category.md#equaliser) in $\mathbf{Cat}$. Applying $C$ gives two identical maps between singleton sets, whose [equalizer](../../../category.md#equaliser) is a singleton. Thus $C$ does not preserve [equalizers](../../../category.md#equaliser) and cannot be a right adjoint.

It cannot extend to the right either. The coproduct of two copies of $I(1)$ in $\mathbf{Cat}$ is the discrete two-object category. But $I(1\amalg1)$ is the indiscrete two-object category, with morphisms between its distinct objects. They are not isomorphic, or even equivalent. Hence $I$ does not preserve binary coproducts and cannot be a left adjoint. **Neither end of this chain has a further adjoint.**

## 7

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

We prove both versions. In the [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem), let $G:\mathcal D\to\mathcal C$ be a [functor](../../../category.md#functor) between locally small categories, with $\mathcal D$ complete. Then $G$ has a left adjoint if and only if it preserves small limits and satisfies the [solution-set condition](../../../category.md#solution-set-condition): for each $C\in\mathcal C$ there is a set of arrows $u_i:C\to GD_i$ such that every arrow $u:C\to GD$ factors as $G(h)u_i$ for some $i$ and $h:D_i\to D$.

First prove the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set). Let $\mathcal A$ be locally small and complete, and have a small weakly initial family $(W_i)$. Its product $W$ is weakly initial: a map $W_i\to A$ can be composed with the product projection. Take $e:E\to W$ to be the simultaneous [equalizer](../../../category.md#equaliser) of every endomorphism of $W$ and its identity. This is a small limit since $\mathcal A(W,W)$ is a set. Maps $E\to A$ exist by composing $e$ with a weakly initial map $W\to A$.

For uniqueness, take any $a,b:E\to A$ and their [equalizer](../../../category.md#equaliser) $j:Z\to E$. Weak initiality of $W$ gives $t:W\to Z$. The endomorphism $ejt$ of $W$ fixes $e$ by its defining [equalizer](../../../category.md#equaliser) property, so $ejte=e$. Since $e$ is monic, $jte=1_E$. Thus $j$ is both monic and split epic, hence invertible, forcing $a=b$. Therefore $E$ is initial. This proves the lemma without an unproved initial-object assertion.

Now fix $C\in\mathcal C$. The comma category $(C\downarrow G)$ is locally small. It is complete: take the limit of the underlying diagram in $\mathcal D$, use preservation by $G$ to factor the compatible arrows from $C$, and obtain the universal comma cone. The solution set is exactly a small weakly initial family in this comma category. The lemma provides its [initial object](../../../category.md#initial-object) $(FC,\eta_C)$. Its universal property is the natural bijection $\mathcal D(FC,D)\cong\mathcal C(C,GD)$. For $v:C\to C'$, initiality gives the unique $Fv$ satisfying $G(Fv)\eta_C=\eta_{C'}v$; uniqueness proves identities and composition. Thus these objects form a left adjoint. Conversely a left adjoint provides the singleton solution set consisting of its unit arrow, and a right adjoint preserves limits: the [adjunction](../../../category.md#adjoint-functors) bijections identify cones into the image diagram with cones from the corresponding left-adjoint object into the original diagram. This proves both directions of the general theorem.

The [limit form of the special adjoint functor theorem](../../../category.md#limit-form-of-the-special-adjoint-functor-theorem) assumes instead that $\mathcal D$ is complete, locally small and well-powered, and has a small cogenerating family $(Q_i)$. For any locally small target, a [functor](../../../category.md#functor) $G:\mathcal D\to\mathcal C$ has a left adjoint exactly when it preserves small limits. Necessity is already proved. For sufficiency we construct a solution set, so that the general theorem applies.

Fix $C$. Given $u:C\to GD$, consider all pairs $h,k:D\to Q_i$ with $G(h)u=G(k)u$. There is only a set of these pairs. Intersect their [equalizers](../../../category.md#equaliser) to obtain a [monomorphism](../../../category.md#monomorphism) $m:D'\to D$. Since $G$ preserves this limit and $u$ equalizes the images of all pairs, it factors uniquely as $u=G(m)u'$ for $u':C\to GD'$.

For each realized pair $(i,v)$ with $v=G(h)u:C\to GQ_i$, choose one such $h$. Any other $k$ with the same pair restricts to the same map on $D'$. The restricted chosen maps jointly separate morphisms into $D'$: if two such morphisms become equal after all chosen maps, they become equal after every $hm$, and the cogenerating family then makes their composites with $m$ equal; monicity of $m$ cancels it. Hence the resulting map

$$
D'\longrightarrow\prod_{(i,v)\in J}Q_i
$$

is monic, where $J$ is a subset of the fixed set $\coprod_i\mathcal C(C,GQ_i)$.

There is only a set of possible $J$, a set of subobjects of each corresponding product by well-poweredness, and a set of arrows from $C$ into $G$ of each chosen subobject representative by local smallness of $\mathcal C$. Collect all these representative comma objects. The factorization just constructed shows that they form a weakly initial set in $(C\downarrow G)$. This is the [cogenerator bound for comma-category solution sets](../../../category.md#cogenerator-bound-for-comma-category-solution-sets), with realized subsets avoiding any assumption that all proposed maps to cogenerators have lifts. The general theorem now gives the left adjoint and proves the special theorem.

## 8

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="8/i">i</h3>

↑ **Parent:** [8](#8)

<h4 id="8/i/solution">Solution</h4>

↑ **Parent:** [I](#8/i)

A [monad](../../../category-theory.md#monad) on $\mathcal C$ consists of an endofunctor $T$ and [natural transformations](../../../category.md#natural-transformation) $\eta:1\Rightarrow T$, $\mu:T^2\Rightarrow T$, satisfying

$$
\mu\,T\eta=1_T=\mu\,\eta_T,\qquad\mu\,T\mu=\mu\,\mu_T.
$$

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is $(A,a)$ with $a:TA\to A$, $a\eta_A=1_A$ and $a\mu_A=aT(a)$. A morphism $(A,a)\to(B,b)$ is an arrow $h:A\to B$ with $ha=bT(h)$. These form the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^T$.

A [functor](../../../category.md#functor) $G:\mathcal D\to\mathcal C$ is monadic when it has a left adjoint $F$ and its comparison $K:\mathcal D\to\mathcal C^{GF}$ is an equivalence; this is the [monadic adjunction](../../../category-theory.md#monadic-adjunction) convention. Some strict formulations require $K$ to be an [isomorphism](../../../algebra.md#isomorphism) over the base. The distinction affects the meaning of literal limit creation, discussed in part (iii), but not the algebra construction.

<h3 id="8/ii">ii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8/ii)

For $F\dashv G$ with unit $\eta$ and counit $\varepsilon$, set

$$
\boxed{T=GF,\qquad\mu_A=G\varepsilon_{FA},\qquad\text{unit }\eta_A.}
$$

Naturality of the unit and counit makes these [natural transformations](../../../category.md#natural-transformation). The two triangle identities give $\mu_A\eta_{TA}=1_{TA}$ and $\mu_AT\eta_A=1_{TA}$. Naturality of $\varepsilon$ at $\varepsilon_{FA}$ gives $\varepsilon_{FA}\varepsilon_{FGFA}=\varepsilon_{FA}FG\varepsilon_{FA}$. Applying $G$ proves $\mu_A\mu_{TA}=\mu_AT\mu_A$. Thus this is the [monad induced by an adjunction](../../../category-theory.md#monad-induced-by-an-adjunction).

Conversely, for any [monad](../../../category-theory.md#monad) take the free-algebra [functor](../../../category.md#functor) $F^T(A)=(TA,\mu_A)$ and the forgetful [functor](../../../category.md#functor) $U:\mathcal C^T\to\mathcal C$. For an algebra $(B,b)$, the assignments $h\mapsto h\eta_A$ and $k\mapsto bT(k)$ give inverse bijections between algebra maps $F^T(A)\to(B,b)$ and arrows $A\to B$. For the inverse identities, $bT(k)\eta_A=b\eta_Bk=k$, while $bT(h\eta_A)=h\mu_AT\eta_A=h$. The algebra and [monad](../../../category-theory.md#monad) laws also make $bT(k)$ an algebra morphism, since $bT(k)\mu_A=b\mu_BT^2k=bT(b)T^2k$. These bijections are natural, giving the [free-forgetful Eilenberg-Moore adjunction](../../../category-theory.md#free-forgetful-eilenberg-moore-adjunction). Its unit is $\eta$, its counit at $(B,b)$ is $b$, and its induced multiplication is exactly $\mu$. Thus **every [monad](../../../category-theory.md#monad) arises from an [adjunction](../../../category.md#adjoint-functors)**.

<h3 id="8/iii">iii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8/iii)

First prove strict creation for the canonical forgetful [functor](../../../category.md#functor) $U:\mathcal C^T\to\mathcal C$. Let a diagram of algebras $(A_i,a_i)$ have a chosen underlying limit cone $p_i:L\to A_i$. The maps $a_iT(p_i):TL\to A_i$ form a cone: if $h:A_i\to A_j$ is a diagram arrow, then $ha_i=a_jT(h)$ and $hp_i=p_j$. Thus the limit property gives a unique action $a:TL\to L$ with

$$
\boxed{p_i a=a_iT(p_i).}
$$

The projections are jointly monic. By naturality of $\eta$ and the algebra unit laws, $p_i a\eta_L=a_i\eta_{A_i}p_i=p_i$, hence $a\eta_L=1_L$. Likewise

$$
p_i a\mu_L=a_i\mu_{A_i}T^2p_i=a_iT(a_i)T^2p_i=p_i aT(a),
$$

so $a\mu_L=aT(a)$. Therefore $(L,a)$ is an algebra and all $p_i$ are algebra morphisms.

For any algebra cone $h_i:(B,b)\to(A_i,a_i)$, let $h:B\to L$ be its unique underlying factor. Then $p_i hb=h_i b=a_iT(h_i)=p_i aT(h)$, so joint monicity gives $hb=aT(h)$. Thus the factor is an algebra morphism, unique as such. The action on the prescribed $L$ was itself forced by the cone equations. This proves [monad algebra forgetful functor creates limits](../../../category-theory.md#monad-algebra-forgetful-functor-creates-limits), without assuming $T$ preserves them.

For a monadic $G$ with comparison an equivalence, transport $(L,a)$ and its cone across that equivalence. This yields a limiting cone in $\mathcal D$ whose image is identified with the prescribed base cone by an [isomorphism](../../../algebra.md#isomorphism), uniquely up to the corresponding cone-compatible [isomorphism](../../../algebra.md#isomorphism). Thus **a monadic [functor](../../../category.md#functor) creates limits in the equivalence-invariant sense**. If monadicity uses a comparison [isomorphism](../../../algebra.md#isomorphism) over the base, the lift is literally on the prescribed underlying cone, proving strict creation as well.

A qualification is necessary if equivalence is used to define monadicity but literal unique lifting is demanded. Let $\mathcal C$ be the [indiscrete category](../../../category.md#indiscrete-category) on two objects $0,1$, let $\mathcal D$ be the terminal category, and let $G$ select $0$. The unique $F:\mathcal C\to\mathcal D$ is left adjoint to $G$, and the comparison to the induced algebra category is an equivalence: the two algebra objects have exactly one map between each pair. Yet the chosen terminal cone with vertex $1$ in $\mathcal C$ has no literal lift, since the only object in the image of $G$ is $0$. The [creation of limits up to isomorphism](../../../category.md#creation-of-limits-up-to-isomorphism) conclusion holds, because $0$ and $1$ are uniquely isomorphic. This distinguishes the two conventions rather than claiming an invalid strict conclusion from equivalence alone.

## 9

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="9/i">i</h3>

↑ **Parent:** [9](#9)

<h4 id="9/i/solution">Solution</h4>

↑ **Parent:** [I](#9/i)

A [functor-split coequalizer pair](../../../category.md#functor-split-coequalizer-pair) for $G$ is a parallel pair $f,g:A\rightrightarrows B$ in $\mathcal D$ whose image has a split [coequalizer](../../../category.md#coequalizer) in $\mathcal C$. Explicitly there are $q:GB\to Q$, $s:Q\to GB$, $t:GB\to GA$ with

$$
qGf=qGg,\qquad qs=1_Q,\qquad(Gf)t=1_{GB},\qquad(Gg)t=sq.
$$

These equations give the [coequalizer](../../../category.md#coequalizer) property: if $hGf=hGg$, then $h=h(Gf)t=h(Gg)t=hsq$, and $q$ is split epic so the factor through it is unique. Every [functor](../../../category.md#functor) preserves such a split diagram, since it preserves these equations.

Reflection means that, for such a pair, any existing arrow $e:B\to D$ whose image is a [coequalizer](../../../category.md#coequalizer) is itself a [coequalizer](../../../category.md#coequalizer) in $\mathcal D$. A [coequalizer](../../../category.md#coequalizer) of the image pair is isomorphic to the specified split one and inherits its splitting. This is reflection of an existing quotient, not an assertion that every base quotient has a lift.

<h3 id="9/ii">ii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9/ii)

For $T=GF$, define the [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor)

$$
\boxed{K(D)=(GD,a_D),\qquad a_D=G\varepsilon_D,\qquad K(h)=Gh.}
$$

The algebra unit law is a triangle identity. Naturality of the counit at $\varepsilon_D$ gives its algebra associativity law; naturality at $h:D\to E$ gives $Gh\,a_D=a_E T(Gh)$, making $K(h)$ an algebra morphism.

Suppose first that $G$ reflects G-split [coequalizers](../../../category.md#coequalizer). For every $D$, consider the counit presentation

$$
FGFGD\underset{FG\varepsilon_D}{\overset{\varepsilon_{FGD}}{\rightrightarrows}}FGD\xrightarrow{\varepsilon_D}D.
$$

It equalizes the pair by counit naturality. After applying $G$ it becomes $T^2GD\rightrightarrows TGD\xrightarrow{a_D}GD$, with parallel maps $\mu_{GD},T(a_D)$. This is split: take $s=\eta_{GD}$ and $t=\eta_{TGD}$. The identities $a_Ds=1$, $\mu_{GD}t=1$ and $T(a_D)t=\eta_{GD}a_D$ follow from the algebra law, a [monad](../../../category-theory.md#monad) unit law, and naturality of $\eta$. Reflection therefore makes $\varepsilon_D$ a [coequalizer](../../../category.md#coequalizer) in $\mathcal D$.

For faithfulness, if $Gh=Gk$ then naturality gives $h\varepsilon_D=\varepsilon_EFGh=\varepsilon_EFGk=k\varepsilon_D$. [Coequalizers](../../../category.md#coequalizer) are epic, so $h=k$.

For fullness, let $\alpha:GD\to GE$ be an algebra morphism, so $\alpha a_D=a_E T\alpha$. Put $h_0=\varepsilon_EF\alpha:FGD\to E$. Its two composites with the counit-presentation pair are equal: by counit naturality they are $\varepsilon_EF(a_ET\alpha)$ and $\varepsilon_EF(\alpha a_D)$. Hence there is a unique $h:D\to E$ with $h\varepsilon_D=h_0$. Applying $G$ gives $Gh\,a_D=a_ET\alpha=\alpha a_D$. Since $a_D$ is split epic, $Gh=\alpha$. This proves full faithfulness directly by descent.

Conversely suppose $K$ is full and faithful. We need the following explicit algebra lifting fact. For algebra morphisms $f,g:(A,a)\rightrightarrows(B,b)$ with a split underlying [coequalizer](../../../category.md#coequalizer) $q:B\to Q$, the arrow $qb:TB\to Q$ equalizes $Tf,Tg$. The split diagram is preserved by $T$, so $Tq$ is their [coequalizer](../../../category.md#coequalizer) and there is a unique $c:TQ\to Q$ with $cTq=qb$. Precomposing the unit equation with the [epimorphism](../../../category.md#epimorphism) $q$ gives $c\eta_Qq=q$; precomposing the associativity equation with the [epimorphism](../../../category.md#epimorphism) $T^2q$ gives equality by $bT(b)=b\mu_B$. Thus $c$ is an algebra action. If an algebra map $h:B\to(Z,z)$ equalizes $f,g$, its unique underlying factor $k:Q\to Z$ satisfies $kcTq=hb=zTh=zTkTq$. Cancelling $Tq$ shows $kc=zTk$. This proves [monad algebra forgetful functor creates split coequalizers](../../../category-theory.md#monad-algebra-forgetful-functor-creates-split-coequalizers).

Now take any existing equalizing arrow $e:B\to D$ in $\mathcal D$ whose image is such a [coequalizer](../../../category.md#coequalizer). The lifting fact makes the unique compatible action on $GD$ its already given action $a_D$, since $Ke$ preserves that action. Hence $Ke$ is a [coequalizer](../../../category.md#coequalizer) of $Kf,Kg$ in the algebra category. For any arrow $h:B\to Z$ equalizing the pair, its unique algebra factor $KD\to KZ$ lifts to an arrow $D\to Z$ by fullness of $K$; faithfulness gives its factorization equation and uniqueness. Therefore $e$ is a [coequalizer](../../../category.md#coequalizer) in $\mathcal D$. We have proved the [full comparison and reflection of split coequalizers](../../../category-theory.md#full-comparison-and-reflection-of-split-coequalizers) equivalence

$$
\boxed{K\text{ is full and faithful}\iff G\text{ reflects G-split coequalizers}.}
$$

## 10

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="10/i">i</h3>

↑ **Parent:** [10](#10)

<h4 id="10/i/solution">Solution</h4>

↑ **Parent:** [I](#10/i)

A [monoidal category](../../../category-theory.md#monoidal-category) consists of a category $\mathcal C$, a bifunctor $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a unit object $I$, and natural [isomorphisms](../../../algebra.md#isomorphism) $a_{X,Y,Z}:(X\otimes Y)\otimes Z\to X\otimes(Y\otimes Z)$, $l_X:I\otimes X\to X$ and $r_X:X\otimes I\to X$. They satisfy the [pentagon identity for a monoidal category](../../../category-theory.md#pentagon-identity-for-a-monoidal-category)

$$
a_{W,X,Y\otimes Z}a_{W\otimes X,Y,Z}=(1_W\otimes a_{X,Y,Z})a_{W,X\otimes Y,Z}(a_{W,X,Y}\otimes1_Z)
$$

and the [triangle identity for a monoidal category](../../../category-theory.md#triangle-identity-for-a-monoidal-category) $(1_X\otimes l_Y)a_{X,I,Y}=r_X\otimes1_Y$. These axioms make different coherent rebracketings and unit removals agree.

It defines a [bicategory](../../../category-theory.md#bicategory) with one object $*$. The hom-category $\mathcal B(*,*)$ is $\mathcal C$; objects of $\mathcal C$ are its 1-cells and morphisms of $\mathcal C$ its 2-cells. Horizontal composition is the tensor bifunctor, the identity 1-cell is $I$, and the associator and unitors are the bicategorical coherence 2-cells. Vertical composition is composition of morphisms in $\mathcal C$, and the interchange law follows from bifunctoriality of $\otimes$. Conversely the hom-category of any one-object [bicategory](../../../category-theory.md#bicategory) has exactly this monoidal structure. Thus **a monoidal category is precisely a one-object [bicategory](../../../category-theory.md#bicategory)**, not necessarily a strict one-object 2-category.

<h3 id="10/ii">ii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10/ii)

The [Category of sets](../../../category.md#category-of-sets) is monoidal under Cartesian product, with any singleton as unit. The tensor of maps is $(f\times g)(x,y)=(f(x),g(y))$, the associator sends $((x,y),z)$ to $(x,(y,z))$, and the left and right unitors discard the singleton coordinate. These are natural bijections. Both pentagon paths send a nested quadruple to the same rebracketed quadruple, and both triangle paths discard the same singleton coordinate, verifying the axioms directly.

This is not the only structure. Disjoint union $X\amalg Y$ is another tensor bifunctor, with empty-set unit. Its associator changes parentheses while retaining the tag indicating the original summand, and its unitors remove an empty summand. Every coherence path preserves both the original tag and the element, so again the pentagon and triangle hold.

These [product and coproduct monoidal structures on sets](../../../category-theory.md#product-and-coproduct-monoidal-structures-on-sets) are distinct even up to monoidal equivalence. Any equivalence of the underlying category preserves initial and [terminal objects](../../../category.md#terminal-object) up to [isomorphism](../../../algebra.md#isomorphism). It therefore cannot carry the empty-set unit of the coproduct structure to the singleton unit of the product structure. Hence **Set has at least these two inequivalent monoidal structures**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
