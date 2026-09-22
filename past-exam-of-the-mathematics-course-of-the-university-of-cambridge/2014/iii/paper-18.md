# Paper 18

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_18.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_18.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)

## 1

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [monomorphism](../../../category.md#monomorphism) is a morphism $m:X\to Y$ such that $mu=mv$ implies $u=v$ for every pair $u,v:Z\to X$. Dually, an [epimorphism](../../../category.md#epimorphism) $e:X\to Y$ satisfies $ue=ve\Rightarrow u=v$. A [regular epimorphism](../../../category.md#regular-epimorphism) is a [coequalizer](../../../category.md#coequalizer) of some parallel pair. An [isomorphism](../../../algebra.md#isomorphism) has a two-sided inverse.

For a [product in a category](../../../category.md#product-category-theory), write $\Delta_A:A\to A\times A$ for its [categorical diagonal](../../../category.md#categorical-diagonal). Since $\pi_1\Delta_A=1_A$, equality $\Delta_Au=\Delta_Av$ gives $u=\pi_1\Delta_Au=\pi_1\Delta_Av=v$. Thus **the diagonal is a monomorphism**, indeed a [split monomorphism](../../../category.md#split-monomorphism).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Here use the [left lifting property against monomorphisms](../../../category.md#left-lifting-property-against-monomorphisms) as the definition of “strong”; epimorphicity will be established separately. In a lifting square write $g:C\to D$, $m:A\to B$, $k:C\to A$ and $l:D\to B$, with $mk=lg$ and $m$ a [monomorphism](../../../category.md#monomorphism). Any two lifts agree because $mt=mt'=l$.

First let $g$ be the [coequalizer](../../../category.md#coequalizer) of $r,s:E\rightrightarrows C$. Every [coequalizer](../../../category.md#coequalizer) is an [epimorphism](../../../category.md#epimorphism): if $ug=vg$, the uniqueness clause for the [coequalizer](../../../category.md#coequalizer) applied to this common composite gives $u=v$. Moreover,

$$
mkr=lgr=lgs=mks,
$$

so $kr=ks$ by [monomorphism](../../../category.md#monomorphism) cancellation. The [coequalizer](../../../category.md#coequalizer) therefore supplies $t:D\to A$ with $tg=k$. Then $mtg=mk=lg$, and [epimorphism](../../../category.md#epimorphism) cancellation gives $mt=l$. This proves that [regular epimorphisms are strong epimorphisms](../../../category.md#regular-epimorphisms-are-strong-epimorphisms).

If $g:C\to D$ is also a [monomorphism](../../../category.md#monomorphism), take $m=g$, $k=1_C$ and $l=1_D$. Its lift satisfies $tg=1_C$ and $gt=1_D$. Hence **[monic lifting-only strong morphisms are invertible](../../../category.md#monic-lifting-only-strong-morphisms-are-invertible)**.

Next suppose $gf:A\to C$ has the [left lifting property against monomorphisms](../../../category.md#left-lifting-property-against-monomorphisms). Given a lifting square for $g:B\to C$, with $mk=lg$, precompose its top arrow with $f$. A lift for $gf$ gives $t:C\to X$ with $mt=l$ and $tgf=kf$. Crucially, one does not cancel $f$: instead $mtg=lg=mk$, and the [monomorphism](../../../category.md#monomorphism) $m$ gives $tg=k$. Thus **the right factor of a strong composite is strong**, proving [right-factor cancellation for lifting-only strong morphisms](../../../category.md#right-factor-cancellation-for-lifting-only-strong-morphisms).

Finally, in $u=iv$ with $u$ strong and $i$ monic, the preceding result makes $i$ strong. The monic-strong argument then makes **$i$ an isomorphism**. None of these arguments assumed that a lifting-only strong morphism was already epic.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $g:C\to D$ have the [left lifting property against monomorphisms](../../../category.md#left-lifting-property-against-monomorphisms), and suppose $\alpha,\beta:D\to B$ satisfy $\alpha g=\beta g$. Use the [categorical diagonal](../../../category.md#categorical-diagonal) $\Delta_B:B\to B\times B$, which is a [monomorphism](../../../category.md#monomorphism) by part (a). The square with top arrow $\alpha g$, bottom arrow $\langle\alpha,\beta\rangle$, left arrow $g$ and right arrow $\Delta_B$ commutes, since both product components are $\alpha g$.

Its lift $t:D\to B$ satisfies $\Delta_Bt=\langle\alpha,\beta\rangle$. Applying the two [product in a category](../../../category.md#product-category-theory) projections gives $t=\alpha$ and $t=\beta$. Thus **$g$ is an epimorphism**. This [binary-product criterion for lifting-only strong epimorphisms](../../../category.md#binary-product-criterion-for-lifting-only-strong-epimorphisms) requires binary products, rather than any assumption about [equalizers](../../../category.md#equaliser).

## 2

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The covariant form of the [Yoneda lemma](../../../category.md#yoneda-lemma) says that for a [locally small category](../../../category.md#locally-small-category) $\mathcal C$, a [functor](../../../category.md#functor) $F:\mathcal C\to\mathbf{Set}$ and an object $A$, there is a [bijection](../../../function.md#bijection), natural in $A$ and $F$,

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A).
$$

Explicitly its two directions are

$$
\boxed{\alpha\longmapsto\alpha_A(1_A),\qquad x\longmapsto\alpha^x,
\quad\alpha^x_B(f)=F(f)(x).}
$$

For $u:B\to B'$, functoriality gives $F(u)\alpha^x_B(f)=F(uf)(x)=\alpha^x_{B'}(uf)$, so $\alpha^x$ is a [natural transformation](../../../category.md#natural-transformation). Conversely, naturality of $\alpha$ at $f:A\to B$ gives $\alpha_B(f)=F(f)(\alpha_A(1_A))$. This proves that the displayed maps are inverses.

Naturality in $F$ follows because postcomposition by $\theta:F\Rightarrow F'$ sends $x$ to $\theta_A(x)$. For $u:A'\to A$, precomposition of transformations by $\mathcal C(u,-)$ sends $\alpha^x$ to $\alpha^{F(u)(x)}$. This also verifies naturality in the representing object.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In the [Category of sets](../../../category.md#category-of-sets), an [epimorphism](../../../category.md#epimorphism) is exactly a [surjective function](../../../algebra.md#surjective-function). A [surjective function](../../../algebra.md#surjective-function) is right-cancellable. If $q:X\to Y$ misses $y\in Y$, the constant-zero function and the function that is one at $y$ and zero elsewhere are distinct maps $Y\to\{0,1\}$ with equal composites with $q$.

If every $\alpha_A$ is surjective, equality $\beta\alpha=\gamma\alpha$ for [natural transformations](../../../category.md#natural-transformation) $\beta,\gamma:G\Rightarrow H$ gives $\beta_A=\gamma_A$ for every $A$. Thus $\alpha$ is an [epimorphism](../../../category.md#epimorphism) in the [functor category](../../../category.md#functor-category).

For the converse, construct the pointwise amalgamated double

$$
H(A)=(G(A)\times\{0,1\})/\sim,
$$

where exactly the two copies of each element of $\operatorname{im}\alpha_A$ are identified; different elements of $G(A)$ remain different. Define $H(u)[y,i]=[G(u)y,i]$. Naturality of $\alpha$ implies that $G(u)$ takes its image into the image at the target, so this formula is well-defined and gives a [functor](../../../category.md#functor). The maps $j_{i,A}(y)=[y,i]$ form [natural transformations](../../../category.md#natural-transformation) $j_0,j_1:G\Rightarrow H$, with $j_0\alpha=j_1\alpha$.

If $\alpha$ is an [epimorphism](../../../category.md#epimorphism), $j_0=j_1$. Since the two copies of an element outside $\operatorname{im}\alpha_A$ would be distinct, every element must lie in that image. Hence **$\alpha$ is epic if and only if every component is epic**. This proves the [pointwise epimorphism in a functor category](../../../category.md#pointwise-epimorphism-in-a-functor-category) criterion directly, including the needed existence and naturality of the separating functor.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A [projective object in a category](../../../category.md#projective-object) is an object $P$ such that, for every [epimorphism](../../../category.md#epimorphism) $e:X\to Y$ and every $u:P\to Y$, there is $v:P\to X$ with $ev=u$.

Let $P=\coprod_{i\in I}P_i$ be a [coproduct in a category](../../../category.md#coproduct) of [projective objects in a category](../../../category.md#projective-object), with injections $\iota_i$. Given $e:X\to Y$ epic and $u:P\to Y$, projectivity supplies $v_i:P_i\to X$ with $ev_i=u\iota_i$. Choose these lifts for the set-indexed family. The [coproduct in a category](../../../category.md#coproduct) supplies a unique $v:P\to X$ satisfying $v\iota_i=v_i$. Since $ev\iota_i=u\iota_i$ for every $i$, its universal property gives $ev=u$.

Thus **[coproducts of projective objects are projective](../../../category.md#coproducts-of-projective-objects-are-projective)**. For an empty family, $P$ is the [initial object](../../../category.md#initial-object), and the lifting assertion follows directly from its unique maps. The family-of-lifts step uses the usual [axiom of choice](../../../set-theory.md#axiom-of-choice).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take an [epimorphism](../../../category.md#epimorphism) $\alpha:F\Rightarrow G$ in $[\mathcal C,\mathbf{Set}]$ and a [natural transformation](../../../category.md#natural-transformation) $\beta:\mathcal C(A,-)\Rightarrow G$. By the [Yoneda lemma](../../../category.md#yoneda-lemma), $\beta$ corresponds to $x=\beta_A(1_A)\in G(A)$. By the [pointwise epimorphism in a functor category](../../../category.md#pointwise-epimorphism-in-a-functor-category) criterion, choose $y\in F(A)$ with $\alpha_A(y)=x$.

The [Yoneda lemma](../../../category.md#yoneda-lemma) gives $\gamma_B(f)=F(f)(y)$, a [natural transformation](../../../category.md#natural-transformation) $\mathcal C(A,-)\Rightarrow F$. Naturality of $\alpha$ yields

$$
\alpha_B\gamma_B(f)=\alpha_BF(f)(y)=G(f)(\alpha_Ay)=G(f)(x)=\beta_B(f).
$$

Therefore **[covariant representables are projective](../../../category.md#covariant-representables-are-projective)** in the set-valued [functor category](../../../category.md#functor-category). Local smallness ensures that $\mathcal C(A,-)$ is set-valued.

## 3

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [functor](../../../category.md#functor) $U:\mathcal C\to\mathbf{Set}$ is a [representable functor](../../../category.md#representable-functor) if some object $R$ admits a [natural isomorphism](../../../category.md#natural-isomorphism) $\mathcal C(R,-)\cong U$. Here the representable is covariant.

For the identity [functor](../../../category.md#functor) on the [Category of sets](../../../category.md#category-of-sets), choose the singleton $1=\{*\}$. The evaluation maps

$$
\mathbf{Set}(1,X)\longrightarrow X,\qquad f\longmapsto f(*)
$$

are [bijections](../../../function.md#bijection) with inverse $x\mapsto(*\mapsto x)$. For $u:X\to Y$, evaluation of $uf$ is $u(f(*))$, proving naturality. Hence **the identity functor on sets is represented by a singleton**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a set $S$, let $\iota_s:1\to S$ select $s$. Given any family $f_s:1\to X$, define $f:S\to X$ by $f(s)=f_s(*)$. Then $f\iota_s=f_s$, and these equations determine every value of $f$, so it is unique.

This is precisely the universal property of a [coproduct in a category](../../../category.md#coproduct), giving

$$
\boxed{S\cong\coprod_{s\in S}1.}
$$

The empty set gives the empty [coproduct in a category](../../../category.md#coproduct), namely the [initial object](../../../category.md#initial-object) of the [Category of sets](../../../category.md#category-of-sets).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Suppose $F:\mathbf{Set}\to\mathcal C$ is a [left adjoint](../../../category.md#adjoint-functors) to $U$. The [adjunction](../../../category.md#adjoint-functors) gives [bijections](../../../function.md#bijection), natural in $X$,

$$
\mathcal C(F1,X)\cong\mathbf{Set}(1,U X)\cong U X.
$$

The second map is evaluation at the singleton element, as in part (a). Thus **$U$ is represented by $F1$**. This argument uses the one-point set as a generator of the particular set-valued adjunction; it does not claim that every arbitrary right adjoint is representable.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $U\cong\mathcal C(R,-)$ be a [representable functor](../../../category.md#representable-functor), and let $(L,p_j)$ be the [categorical limit](../../../category.md#categorical-limit) of a small diagram $D:J\to\mathcal C$. A morphism $R\to L$ is uniquely equivalent to a family $f_j:R\to D(j)$ satisfying $D(u)f_j=f_k$ for every $u:j\to k$.

Such compatible families are exactly the elements of the [categorical limit](../../../category.md#categorical-limit) of the set-valued diagram $\mathcal C(R,D(-))$. Consequently the canonical comparison

$$
\mathcal C(R,L)\longrightarrow\lim_{j\in J}\mathcal C(R,D(j)),\qquad f\longmapsto(p_jf)_j,
$$

is a [bijection](../../../function.md#bijection). Transporting it through the representing [natural isomorphism](../../../category.md#natural-isomorphism) proves that **$U$ preserves every small limit that exists in $\mathcal C$**. This proves that [covariant representables preserve limits](../../../category.md#covariant-representables-preserve-limits). For an empty diagram this says that maps into a terminal object form a singleton.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Choose a representing object $R$ and a [natural isomorphism](../../../category.md#natural-isomorphism) $\theta_X:\mathcal C(R,X)\cong U X$. Using the assumed small [coproducts in a category](../../../category.md#coproduct), define

$$
\boxed{F(S)=\coprod_{s\in S}R.}
$$

For a function $v:S\to S'$, define $F(v)$ by $F(v)\iota_s=\iota_{v(s)}$. The [coproduct in a category](../../../category.md#coproduct) uniqueness clause proves preservation of identities and composition, so this is a [functor](../../../category.md#functor).

Restriction to the coproduct summands, followed by $\theta$, gives

$$
\mathcal C(F(S),X)\cong\prod_{s\in S}\mathcal C(R,X)\cong\mathbf{Set}(S,U X).
$$

These [bijections](../../../function.md#bijection) are natural in $S$ by the definition of $F(v)$, and natural in $X$ by naturality of $\theta$. They establish **$F\dashv U$**, the [left adjoint to a covariant representable functor](../../../category.md#left-adjoint-to-a-covariant-representable-functor). The empty set is sent to the empty coproduct.

## 4

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $F:\mathcal C\to\mathcal D$ and $G:\mathcal D\to\mathcal C$. The characterization concerns an [adjunction](../../../category.md#adjoint-functors) with the specified [unit and counit of an adjunction](../../../category.md#unit-and-counit-of-an-adjunction) $\eta$ and $\varepsilon$. Its [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) are

$$
\boxed{\varepsilon_{FA}F\eta_A=1_{FA},\qquad G\varepsilon_D\eta_{GD}=1_{GD}.}
$$

Assume these identities. Define the hom-set maps

$$
\Phi(h)=Gh\,\eta_A\quad(h:FA\to D),\qquad
\Psi(f)=\varepsilon_DFf\quad(f:A\to GD).
$$

Naturality of $\eta$ and $\varepsilon$ makes these maps natural in both objects. Naturality and the [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give

$$
\begin{aligned}
\Psi\Phi(h)&=\varepsilon_DFGh\,F\eta_A
=h\varepsilon_{FA}F\eta_A=h,\\
\Phi\Psi(f)&=G\varepsilon_DGFf\,\eta_A
=G\varepsilon_D\eta_{GD}f=f.
\end{aligned}
$$

Thus they are inverse [bijections](../../../function.md#bijection) and define $F\dashv G$.

Conversely, from the natural hom-set [bijections](../../../function.md#bijection) of an [adjunction](../../../category.md#adjoint-functors), define $\eta_A=\Phi(1_{FA})$ and $\varepsilon_D=\Phi^{-1}(1_{GD})$. Naturality gives the same formulas for $\Phi$ and $\Psi$ above. Applying $\Psi\Phi$ to $1_{FA}$ and $\Phi\Psi$ to $1_{GD}$ gives the two [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction). Therefore these identities are exactly the compatibility conditions on the specified unit and counit. If the printed equivalence were read as mere existence of some adjunction, independently of the supplied transformations, its only-if direction would be false: on the category of [abelian groups](../../../group.md#abelian-group), $F=G=1$ are adjoint, but choosing both transformations to be zero does not satisfy either triangle on a nonzero object.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $e_A=\varepsilon_{FA}F\eta_A$. This is a [natural transformation](../../../category.md#natural-transformation) $F\Rightarrow F$. Only the $G$-triangle $G\varepsilon_D\eta_{GD}=1_{GD}$ is assumed. Naturality gives two useful absorption identities:

$$
\begin{aligned}
Ge_A\eta_A
&=G\varepsilon_{FA}GF\eta_A\eta_A
=G\varepsilon_{FA}\eta_{GFA}\eta_A=\eta_A,\\
\varepsilon_D e_{GD}
&=\varepsilon_D\varepsilon_{FGD}F\eta_{GD}
=\varepsilon_DFG\varepsilon_DF\eta_{GD}=\varepsilon_D.
\end{aligned}
$$

For the second equality in the last line use naturality of $\varepsilon$ at $\varepsilon_D$, and then the assumed $G$-triangle. Naturality of $\varepsilon$ at $F\eta_A$ and of $\eta$ at $\eta_A$ now gives

$$
\begin{aligned}
e_A^2
&=\varepsilon_{FA}\varepsilon_{FGFA}FGF\eta_A F\eta_A\\
&=\varepsilon_{FA}\varepsilon_{FGFA}F\eta_{GFA}F\eta_A
=\varepsilon_{FA}e_{GFA}F\eta_A=e_A.
\end{aligned}
$$

Hence **$e$ is an idempotent in the functor category**: this is the [one-triangle adjunction idempotent](../../../category.md#one-triangle-adjunction-idempotent).

For the [splitting of an idempotent morphism](../../../category.md#splitting-of-an-idempotent-morphism), suppose this [idempotent morphism](../../../category.md#idempotent-morphism) splits as [natural transformations](../../../category.md#natural-transformation) $r:F\Rightarrow H$ and $s:H\Rightarrow F$, with $sr=e$ and $rs=1_H$. Define

$$
\eta'_A=Gr_A\eta_A,\qquad \varepsilon'_D=\varepsilon_Ds_{GD}.
$$

The first absorption identity gives

$$
G\varepsilon'_D\eta'_{GD}
=G\varepsilon_DGe_{GD}\eta_{GD}=1_{GD}.
$$

For the other triangle, naturality of $s$ at $\eta'_A$ and of $\varepsilon$ at $r_A$ gives

$$
\begin{aligned}
\varepsilon'_{HA}H\eta'_A
&=\varepsilon_{HA}s_{GHA}H\eta'_A
=\varepsilon_{HA}F\eta'_A s_A\\
&=\varepsilon_{HA}FGr_A F\eta_A s_A
=r_A\varepsilon_{FA}F\eta_A s_A
=r_Ae_As_A=1_{HA}.
\end{aligned}
$$

Thus the [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) prove $H\dashv G$.

Conversely, suppose $H\dashv G$, with unit $\psi:1_{\mathcal C}\Rightarrow GH$ and counit $\varphi:HG\Rightarrow1_{\mathcal D}$. The unit has target $GH$, as its type requires. Define

$$
\boxed{s_A=\varphi_{FA}H\eta_A:HA\to FA,\qquad
r_A=\varepsilon_{HA}F\psi_A:FA\to HA.}
$$

These are [natural transformations](../../../category.md#natural-transformation). Transposition under $H\dashv G$ gives $Gs_A\psi_A=\eta_A$. Independently, naturality of $\eta$ at $\psi_A$ and the assumed $G$-triangle give

$$
Gr_A\eta_A=G\varepsilon_{HA}GF\psi_A\eta_A
=G\varepsilon_{HA}\eta_{GHA}\psi_A=\psi_A.
$$

The transpose of $r_As_A$ is therefore $Gr_AGs_A\psi_A=\psi_A$, the transpose of $1_{HA}$. Injectivity of the hom-set [bijection](../../../function.md#bijection) implies $r_As_A=1_{HA}$. Naturality of $\varepsilon$ at $s_A$ gives

$$
s_Ar_A=\varepsilon_{FA}FGs_AF\psi_A
=\varepsilon_{FA}F(Gs_A\psi_A)=\varepsilon_{FA}F\eta_A=e_A.
$$

Consequently **$G$ has a left adjoint if and only if $e$ splits**. This is the criterion for [splitting a one-triangle adjunction idempotent](../../../category.md#splitting-a-one-triangle-adjunction-idempotent). The argument gives both the explicit splitting and the new unit and counit, without assuming the other triangle for $F$.

## 5

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For $A\in\mathcal C$, the [comma category](../../../category.md#comma-category) $(A\downarrow G)$ has objects $(D,u)$ with $D\in\mathcal D$ and $u:A\to GD$. A morphism $(D,u)\to(D',u')$ is $h:D\to D'$ satisfying $Gh\,u=u'$. Identities and composition are those of $\mathcal D$, and functoriality of $G$ verifies the condition under composition.

The [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) states: if $\mathcal D$ is a [locally small category](../../../category.md#locally-small-category) with all small [categorical limits](../../../category.md#categorical-limit), and $\mathcal C$ is locally small, then $G:\mathcal D\to\mathcal C$ has a [left adjoint](../../../category.md#adjoint-functors) if and only if it preserves small limits and satisfies the [solution-set condition](../../../category.md#solution-set-condition). The latter means that for each $A$ there is a set-indexed family $u_i:A\to GD_i$ such that every $u:A\to GD$ equals $Gh\,u_i$ for some $i$ and some $h:D_i\to D$.

For necessity, use the standard result that a [right adjoint](../../../category.md#adjoint-functors) preserves [categorical limits](../../../category.md#categorical-limit). If $F\dashv G$, the singleton family containing the [unit of an adjunction](../../../category.md#unit-of-an-adjunction) $\eta_A:A\to GFA$ is a solution set, since transposition gives $u=Gh\,\eta_A$ for a unique $h:FA\to D$.

For sufficiency, use the following standard limit fact: if $\mathcal D$ is complete and $G$ preserves limits, the projection $(A\downarrow G)\to\mathcal D$ creates small limits. Indeed, a compatible family $A\to GD_j$ induces a unique arrow into $G(\lim D_j)$, and this makes the underlying limit a limit in the comma category. The [comma category](../../../category.md#comma-category) is locally small because each of its hom-sets is a subset of a hom-set of $\mathcal D$. Its solution family is a [weakly initial set](../../../category.md#weakly-initial-set).

We prove the remaining [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set). In any [locally small category](../../../category.md#locally-small-category) $\mathcal K$ with all small limits and a weakly initial set $(K_i)$, form $W=\prod_iK_i$. It is weakly initial: for any $X$, some $K_i\to X$ exists and may be composed with the projection $W\to K_i$. The empty family cannot be weakly initial in a nonempty complete category, which has a terminal object.

The set $\operatorname{End}(W)$ is small. Form a simultaneous [equalizer](../../../category.md#equaliser) $e:E\to W$ of every endomorphism of $W$ and $1_W$; thus

$$
u e=e\quad\text{for every }u:W\to W.
$$

This equalizer exists by completeness, for example as the equalizer of two maps $W\rightrightarrows W^{\operatorname{End}(W)}$. The object $E$ is still weakly initial, since it maps to $W$.

Given $a,b:E\to X$, take their [equalizer](../../../category.md#equaliser) $j:Y\to E$. Weak initiality of $W$ gives $t:W\to Y$. Since $ejt$ is an endomorphism of $W$, we have $ejte=e$, and cancellation of the [monomorphism](../../../category.md#monomorphism) $e$ gives $jte=1_E$. Thus $j$ is a [split epimorphism](../../../category.md#split-epimorphism) as well as a [monomorphism](../../../category.md#monomorphism), so it is an [isomorphism](../../../algebra.md#isomorphism). From $aj=bj$ follows $a=b$. There is at least one map $E\to X$ by weak initiality, so **$E$ is initial**.

Apply this lemma to every $(A\downarrow G)$ and choose its [initial object](../../../category.md#initial-object) $(FA,\eta_A)$. For $v:A\to A'$, initiality gives the unique $Fv:FA\to FA'$ satisfying $GFv\,\eta_A=\eta_{A'}v$. Uniqueness proves the functor laws. The same initiality gives natural [bijections](../../../function.md#bijection)

$$
\mathcal D(FA,D)\cong\mathcal C(A,GD),\qquad h\longmapsto Gh\,\eta_A.
$$

Hence **$F\dashv G$**, completing the theorem without invoking another adjoint functor theorem.

## 6

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [monad](../../../category-theory.md#monad) consists of an endofunctor $T:\mathcal C\to\mathcal C$ and [natural transformations](../../../category.md#natural-transformation) $\eta:1\Rightarrow T$ and $\mu:T^2\Rightarrow T$, the [unit and multiplication of a monad](../../../category-theory.md#unit-and-multiplication-of-a-monad), satisfying

$$
\mu_A T\eta_A=\mu_A\eta_{TA}=1_{TA},\qquad
\mu_A T\mu_A=\mu_A\mu_{TA}.
$$

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is $(A,a)$ with $a:TA\to A$ satisfying $a\eta_A=1_A$ and $a\mu_A=aTa$. A [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad) $h:(A,a)\to(B,b)$ satisfies $ha=bTh$. These objects and morphisms form the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^T$; its composition works because $T$ is a [functor](../../../category.md#functor).

For the [list monad](../../../category-theory.md#list-monad), $TX=\coprod_{n\geq0}X^n$ is the set of finite ordered lists, including the empty list. The map $Tf$ applies $f$ to each entry; $\eta_X(x)=[x]$ and $\mu_X$ concatenates a list of lists. The unit laws say that adding singleton brackets and then flattening changes nothing. Associativity says that flattening a list of lists of lists in either order produces the same ordered sequence. These descriptions also prove naturality.

If $a:TX\to X$ is an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad), define

$$
e=a([]),\qquad x*y=a([x,y]).
$$

The singleton law gives $a([x])=x$. Apply the algebra associativity law to $[[],[x]]$ and $[[x],[]]$ to obtain $e*x=x=x*e$. Applying it to $[[x,y],[z]]$ and $[[x],[y,z]]$ shows

$$
(x*y)*z=a([x,y,z])=x*(y*z).
$$

Thus $(X,*,e)$ is a [monoid](../../../algebra.md#monoid). Applying the same law to $[[x_1,\ldots,x_{n-1}],[x_n]]$ shows inductively that $a$ is necessarily ordered multiplication of its entries, with the empty product $e$.

Conversely, any [monoid](../../../algebra.md#monoid) defines such a list-fold map $a$. The monoid unit proves $a\eta=1$, and associativity and the unit prove that multiplying flattened lists equals multiplying their individual products, including empty sublists. Hence $a\mu=aTa$. An algebra morphism preserves the empty-list value and two-entry-list values, so it is a [monoid homomorphism](../../../algebra.md#monoid-homomorphism); conversely a [monoid homomorphism](../../../algebra.md#monoid-homomorphism) preserves every ordered product and is an algebra morphism. Therefore

$$
\boxed{\mathbf{Set}^{\mathrm{List}}\cong\mathbf{Mon}.}
$$

Thus [list-monad algebras are monoids](../../../category-theory.md#list-monad-algebras-are-monoids), with the identification also matching every morphism.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [free algebra functor](../../../category-theory.md#free-algebra-functor) is

$$
F(A)=(TA,\mu_A),\qquad F(f)=Tf.
$$

The [monad](../../../category-theory.md#monad) laws make $\mu_A$ an algebra action, and naturality of $\mu$ makes $Tf$ a [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad). Let $U:\mathcal C^T\to\mathcal C$ forget the action. Define

$$
\boxed{\mathcal C^T(F A,(B,b))\cong\mathcal C(A,B),\qquad
h\longmapsto h\eta_A,\quad f\longmapsto bTf.}
$$

The proposed inverse is an algebra morphism because

$$
(bTf)\mu_A=b\mu_B T^2f=bTb\,T^2f=bT(bTf).
$$

Naturality of $\eta$ and the algebra unit law give $(bTf)\eta_A=f$. If $h$ is an algebra morphism, then

$$
bT(h\eta_A)=bTh\,T\eta_A=h\mu_A T\eta_A=h.
$$

The formulas are natural in both variables, so **$F\dashv U$**. Its unit is $\eta$, and its counit at $(B,b)$ has underlying map $b:TB\to B$. Thus the [monad induced by an adjunction](../../../category-theory.md#monad-induced-by-an-adjunction) has endofunctor $UF=T$, unit $\eta$, and multiplication $U\varepsilon_F=\mu$. It is **exactly the original monad**, not merely a monad with the same endofunctor.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) $(A,a)$, consider the fork in the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category)

$$
\boxed{F(TA)\ \mathrel{\substack{\xrightarrow{\ \mu_A\ }\\[-2pt]\xrightarrow[\ Ta\ ]{}}}\ F(A)\xrightarrow{\ a\ }(A,a).}
$$

Here $\mu_A:F(TA)\to F(A)$ is the counit at $F(A)$, and $Ta=F(a)$. The arrow $a$ is an algebra morphism by $a\mu_A=aTa$, which also says that it coequalizes the two arrows.

Let $h:F(A)\to(B,b)$ be an algebra morphism with $h\mu_A=hTa$. Define $g=h\eta_A:A\to B$. Naturality of $\eta$ at $a$ gives

$$
ga=h\eta_Aa=hTa\,\eta_{TA}=h\mu_A\eta_{TA}=h.
$$

Since $h$ is an algebra morphism,

$$
bTg=bTh\,T\eta_A=h\mu_A T\eta_A=h=ga.
$$

Thus $g:(A,a)\to(B,b)$ is an algebra morphism with $ga=h$. Any other such factorization satisfies $g'=g'a\eta_A=h\eta_A=g$. This proves the full [coequalizer](../../../category.md#coequalizer) universal property inside the algebra category.

The pair is moreover a [reflexive pair](../../../category-theory.md#reflexive-pair): its common section is $F(\eta_A)$, with underlying map $T\eta_A$, because $\mu_AT\eta_A=1_{TA}$ and $Ta\,T\eta_A=T(a\eta_A)=1_{TA}$. Hence **every monad algebra is a reflexive coequalizer of free algebras**. This [reflexive free-algebra presentation of a monad algebra](../../../category-theory.md#reflexive-free-algebra-presentation-of-a-monad-algebra) needs no general existence theorem for arbitrary algebra-category colimits.

## 7

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

An [isomorphism](../../../algebra.md#isomorphism) $f:A\to B$ is a morphism with an inverse $f^{-1}:B\to A$ satisfying $f^{-1}f=1_A$ and $ff^{-1}=1_B$. A [groupoid](../../../category.md#groupoid) is a [category](../../../category.md) in which every morphism is an [isomorphism](../../../algebra.md#isomorphism).

With the given one-sided inverses,

$$
g=g1_B=g(fh)=(gf)h=1_Ah=h.
$$

Consequently **$f$ is an isomorphism with $f^{-1}=g=h$**. This argument uses only the category axioms.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

A [preadditive category](../../../category.md#preadditive-category) has an [abelian group](../../../group.md#abelian-group) structure on every hom-set, with composition additive in each variable. Neither a [zero object](../../../category.md#zero-object) nor [biproducts](../../../category-theory.md#biproduct) are part of this definition.

Fix $C$ and use the [reflexive pair](../../../category-theory.md#reflexive-pair) $f,g:A\rightrightarrows B$, $r:B\to A$, with $fr=gr=1_B$. Take objects $x:C\to B$ and arrows $a:C\to A$, with source $fa$, target $ga$, and identity at $x$ equal to $rx$. For composable $a,b$, so $ga=fb$, define

$$
\boxed{b\circ a=a+b-rga.}
$$

The [preadditive category](../../../category.md#preadditive-category) axioms give

$$
f(b\circ a)=fa+fb-ga=fa,\qquad
g(b\circ a)=ga+gb-ga=gb.
$$

Thus the formula has the required endpoints. The identities satisfy $(rga)\circ a=a$ and $a\circ(rfa)=a$, using $gr=fr=1_B$.

For $ga=fb$ and $gb=fc$, both ways of composing three arrows equal

$$
a+b+c-rga-rgb.
$$

Indeed $g(b\circ a)=gb$, while expanding $c\circ b$ and then composing with $a$ gives the same expression. Hence composition is associative.

Every arrow has inverse

$$
\boxed{a^{-1}=rfa+rga-a.}
$$

Its source is $ga$ and its target is $fa$. Substituting in the composition formula gives $a^{-1}\circ a=rfa$ and $a\circ a^{-1}=rga$. Therefore this is a [groupoid](../../../category.md#groupoid).

For $u:C'\to C$, precomposition by $u$ preserves sources, targets, identities, composition and inverses by bilinearity. Thus the construction is natural in $C$, giving the requested [internal groupoid](../../../category-theory.md#internal-groupoid) structure in its hom-set formulation. If the composable-arrow [pullback in a category](../../../category.md#pullback-category-theory) exists, the same formula defines its internal composition morphism. The [reflexive-pair groupoid formula in a preadditive category](../../../category-theory.md#reflexive-pair-groupoid-formula-in-a-preadditive-category) requires no extra additive-category hypotheses.

## 8

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

In a [pointed category](../../../category.md#pointed-category), a [zero object](../../../category.md#zero-object) defines zero morphisms between all objects. A [categorical cokernel](../../../category.md#cokernel-in-a-category) of $f:A\to B$ is a map $g:B\to C$ with $gf=0$ such that every $u:B\to X$ with $uf=0$ factors uniquely as $u=\bar u g$. Equivalently it is the [coequalizer](../../../category.md#coequalizer) of $f$ and the zero map, so $g$ is an [epimorphism](../../../category.md#epimorphism).

Write $a:A\to A'$, $b:B\to B'$, and $c:C\to C'$ for the vertical arrows, with $g'=\operatorname{coker}f'$ and $cg=g'b$. The left [pushout in a category](../../../category.md#pushout-in-a-category) applied to the compatible pair $g:B\to C$ and $0:A'\to C$ gives $h:B'\to C$ satisfying $hb=g$ and $hf'=0$. The [categorical cokernel](../../../category.md#cokernel-in-a-category) property of $g'$ then gives $d:C'\to C$ with $dg'=h$.

Now $dcg=dg'b=hb=g$. Cancel the [epimorphism](../../../category.md#epimorphism) $g$ to obtain $dc=1_C$. To prove the other identity, the two arrows $cdg',g':B'\to C'$ agree after $b$, because $cdg'b=cg=g'b$, and after $f'$, because both composites are zero. The [pushout in a category](../../../category.md#pushout-in-a-category) uniqueness clause gives $cdg'=g'$. Cancelling the [epimorphism](../../../category.md#epimorphism) $g'$ gives $cd=1_{C'}$.

Thus **$c$ is an isomorphism**: [cokernel invariance under pushout](../../../category.md#cokernel-invariance-under-pushout) holds already in pointed categories with the indicated cokernels.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Let $q:B\to Q$ be the [categorical cokernel](../../../category.md#cokernel-in-a-category) of $f$ in an [abelian category](../../../category-theory.md#abelian-category). If $f$ is an [epimorphism](../../../category.md#epimorphism), the equality $qf=0f$ implies $q=0$. Since $q$ is also an [epimorphism](../../../category.md#epimorphism), $1_Qq=0q$ implies $1_Q=0$. An object with zero identity is a [zero object](../../../category.md#zero-object): every morphism to or from it is zero. Hence the cokernel object is zero.

Conversely, suppose the cokernel object is zero. If $uf=vf$, additivity gives $(u-v)f=0$. The [categorical cokernel](../../../category.md#cokernel-in-a-category) property makes $u-v$ factor through the zero object, so $u-v=0$ and $u=v$. Thus

$$
\boxed{f\text{ is epic}\quad\Longleftrightarrow\quad\operatorname{coker}f=0.}
$$

This is the [zero-cokernel criterion for epimorphisms](../../../category-theory.md#zero-cokernel-criterion-for-epimorphisms). In a [pushout in a category](../../../category.md#pushout-in-a-category), the two horizontal morphisms have isomorphic cokernels by part (a). Therefore the lower morphism is epic if and only if the upper morphism is epic. In particular **pushouts reflect epimorphisms** in an [abelian category](../../../category-theory.md#abelian-category); the same argument also proves preservation.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Use the displayed square's notation $f:A\to B$, $h:A\to C$, $g:B\to D$, $k:C\to D$, with $gf=kh$ and $g$ epic. Form the [biproduct](../../../category-theory.md#biproduct) and the morphisms

$$
q=[g,-k]:B\oplus C\to D,\qquad j=\binom f h:A\to B\oplus C.
$$

The map $q$ is an [epimorphism](../../../category.md#epimorphism), since its restriction to $B$ is $g$: equality after $q$ implies equality after $g$. The [pullback in a category](../../../category.md#pullback-category-theory) property says exactly that $j$ is a [categorical kernel](../../../category.md#kernel-in-a-category) of $q$. Indeed $qj=gf-kh=0$, and a map into $B\oplus C$ killed by $q$ is a pair $(x,y)$ with $gx=ky$, which factors uniquely through $(f,h)$.

Use the standard [abelian category](../../../category-theory.md#abelian-category) property that every [epimorphism](../../../category.md#epimorphism) is the [categorical cokernel](../../../category.md#cokernel-in-a-category) of its [categorical kernel](../../../category.md#kernel-in-a-category). If $u:B\to X$ and $v:C\to X$ satisfy $uf=vh$, then $[u,-v]j=0$. Hence there is a unique $w:D\to X$ with $wq=[u,-v]$. Restriction to the two summands gives $wg=u$ and $wk=v$. This is the [pushout in a category](../../../category.md#pushout-in-a-category) universal property. Thus **a [pullback of an epimorphism is a pushout in an abelian category](../../../category-theory.md#pullback-of-an-epimorphism-is-a-pushout-in-an-abelian-category)**.

In this pushout, $g$ is the pushout of $h$ along $f$. The reflection result of part (b) therefore makes $h$ epic. This proves [pullback stability of epimorphisms in an abelian category](../../../category-theory.md#pullback-stability-of-epimorphisms-in-an-abelian-category).

Finally, let $e:E\to B$ be an [epimorphism](../../../category.md#epimorphism) and let $p_1,p_2:R\rightrightarrows E$ be its [kernel pair](../../../category.md#kernel-pair). Their pullback square is a pushout by the result just proved. If $u:E\to X$ satisfies $up_1=up_2$, the two copies of $u$ form a pushout cocone. There is a unique $v:B\to X$ with $ve=u$. Hence **[epimorphisms in an abelian category are coequalizers of their kernel pairs](../../../category.md#epimorphisms-in-an-abelian-category-are-coequalizers-of-their-kernel-pairs)**, so they are [regular epimorphisms](../../../category.md#regular-epimorphism).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
