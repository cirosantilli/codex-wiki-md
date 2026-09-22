# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_22.pdf)

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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)
    - [iii](#6/c/iii)
      - [Solution](#6/c/iii/solution)
    - [iv](#6/c/iv)
      - [Solution](#6/c/iv/solution)

## 1

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [locally small category](../../../category.md#locally-small-category) $\mathcal C$, an object $C$, and a [categorical presheaf](../../../category.md#presheaf-category-theory) $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$, the [Yoneda lemma](../../../category.md#yoneda-lemma) gives the [natural bijection](../../../category.md#natural-bijection)

$$
\boxed{\Phi_{C,X}:\operatorname{Nat}(\mathcal C(-,C),X)\cong X(C).}
$$

Its two maps are explicitly

$$
\Phi_{C,X}(\alpha)=\alpha_C(1_C),\qquad
\Psi_{C,X}(x)_A(f)=X(f)(x)\quad(f:A\to C).
$$

For $u:A'\to A$, the equation $X(u)X(f)(x)=X(fu)(x)$ proves [naturality](../../../category.md#naturality) of $\Psi(x)$. Evaluating it at the [identity morphism](../../../algebra.md#identity-morphism) gives $\Phi\Psi(x)=x$. Conversely, [naturality](../../../category.md#naturality) of $\alpha$ at $f:A\to C$ gives

$$
\alpha_A(f)=X(f)(\alpha_C(1_C)),
$$

so $\Psi\Phi(\alpha)=\alpha$. **Evaluation at the identity and transport of an element along a morphism are mutually inverse.**

The [bijection](../../../function.md#bijection) is natural in both variables: a [natural transformation](../../../category.md#natural-transformation) $\theta:X\Rightarrow Y$ sends $\Phi(\alpha)$ to $\theta_C(\Phi(\alpha))$, matching $\Phi(\theta\alpha)$; and $g:C\to C'$ gives

$$
\Phi_{C,X}(\alpha\circ\mathcal C(-,g))
=X(g)(\Phi_{C',X}(\alpha))
\quad\bigl(\alpha:\mathcal C(-,C')\Rightarrow X\bigr).
$$

For completeness, the covariant [Yoneda lemma](../../../category.md#yoneda-lemma) for $Y:\mathcal C\to\mathbf{Set}$ is $\operatorname{Nat}(\mathcal C(C,-),Y)\cong Y(C)$, with $\alpha\mapsto\alpha_C(1_C)$ and inverse $y\mapsto(f:C\to A\mapsto Y(f)(y))$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the [categorical presheaf](../../../category.md#presheaf-category-theory) $X$, its [category of elements](../../../category.md#category-of-elements) has objects $(C,x)$ with $x\in X(C)$. A [morphism](../../../algebra.md#morphism) $(C,x)\to(D,y)$ is a [morphism](../../../algebra.md#morphism) $f:C\to D$ satisfying $X(f)(y)=x$. [Composition in a category](../../../category.md#composition-in-a-category) is inherited from $\mathcal C$: if also $X(g)(z)=y$, then $X(gf)(z)=X(f)X(g)(z)=x$. The [identity morphisms](../../../algebra.md#identity-morphism) are inherited as well. The [forgetful functor](../../../category.md#forgetful-functor) sends $(C,x)$ to $C$ and $f$ to $f$.

A [universal element](../../../category.md#universal-element-of-a-set-valued-functor) is a pair $(R,r)$ for which each $x\in X(C)$ is uniquely of the form $X(f)(r)$ for $f:C\to R$. Thus $(R,r)$ is a [terminal object](../../../category.md#terminal-object) of the [category of elements](../../../category.md#category-of-elements), with the variance appropriate to a [categorical presheaf](../../../category.md#presheaf-category-theory).

Given a [universal element](../../../category.md#universal-element-of-a-set-valued-functor), define

$$
\psi_C:\mathcal C(C,R)\longrightarrow X(C),\qquad f\longmapsto X(f)(r).
$$

The defining uniqueness makes each map a [bijection](../../../function.md#bijection); $X(u)\psi_C(f)=\psi_{C'}(fu)$ gives [naturality](../../../category.md#naturality) for $u:C'\to C$. Hence $\psi$ is a [natural isomorphism](../../../category.md#natural-isomorphism) and $X$ is a [representable presheaf](../../../category.md#representable-functor). Conversely, from a [natural isomorphism](../../../category.md#natural-isomorphism) $\psi:\mathcal C(-,R)\cong X$, take $r=\psi_R(1_R)$. The [Yoneda lemma](../../../category.md#yoneda-lemma) gives $\psi_C(f)=X(f)(r)$; its bijectivity makes $(R,r)$ a [universal element](../../../category.md#universal-element-of-a-set-valued-functor). Therefore **the two descriptions coincide**:

$$
\boxed{X\text{ is representable}\iff\operatorname{Elts}(X)\text{ has a terminal object}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $b:B\to B'$ in $\mathcal B$, conjugate the induced [natural transformation](../../../category.md#natural-transformation) by the chosen [representations of a functor](../../../category.md#representation-of-a-functor):

$$
\tau_b=\psi_{B'}^{-1}\,H(-,b)\,\psi_B:
\mathcal A(-,GB)\Rightarrow\mathcal A(-,GB').
$$

The [Yoneda lemma](../../../category.md#yoneda-lemma) gives a unique [morphism](../../../algebra.md#morphism) $Gb:GB\to GB'$ whose postcomposition map is $\tau_b$. Explicitly,

$$
\boxed{Gb=(\psi_{B',GB})^{-1}\!\left(H(GB,b)(\psi_{B,GB}(1_{GB}))\right).}
$$

Consequently, for every $f:A\to GB$,

$$
H(A,b)(\psi_{B,A}(f))=\psi_{B',A}(Gb\circ f).
$$

This is precisely the required [naturality](../../../category.md#naturality) in $B$. The identities $\tau_{1_B}=1$ and $\tau_{b'b}=\tau_{b'}\tau_b$ force $G1_B=1_{GB}$ and $G(b'b)=Gb'\,Gb$, because the [Yoneda embedding](../../../category.md#yoneda-embedding) is [fully faithful](../../../category.md#full-and-faithful-functor). Thus **the representing objects extend uniquely to a functor** $G:\mathcal B\to\mathcal A$. Uniqueness follows by the same [Yoneda lemma](../../../category.md#yoneda-lemma): any candidate satisfying that [naturality](../../../category.md#naturality) must induce $\tau_b$, so must have exactly the displayed action on [morphisms](../../../algebra.md#morphism).

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Fix the chosen [categorical limit](../../../category.md#categorical-limit) object $LA$ and its [categorical cone](../../../category.md#cone-over-a-diagram) $p_{A,j}:LA\to(DA)_j$. For $a:A\to A'$, the family

$$
LA\xrightarrow{p_{A,j}}(DA)_j\xrightarrow{(Da)_j}(DA')_j
$$

is a [categorical cone](../../../category.md#cone-over-a-diagram), by [naturality](../../../category.md#naturality) of $Da$. The [universal property](../../../category-theory.md#universal-property) of $LA'$ supplies a unique [morphism](../../../algebra.md#morphism)

$$
\boxed{La:LA\to LA',\qquad p_{A',j}La=(Da)_jp_{A,j}\text{ for every }j.}
$$

The [identity morphism](../../../algebra.md#identity-morphism) of $LA$ satisfies the equations for $a=1_A$, so $L1_A=1_{LA}$. For composable $a,a'$, the equations for $La'\,La$ agree with those for $L(a'a)$; uniqueness gives $L(a'a)=La'\,La$. Hence **the chosen limits define a functor** $L:\mathcal A\to\mathcal C$. This argument also handles an empty indexing [category](../../../category.md), when each chosen [categorical limit](../../../category.md#categorical-limit) is a [terminal object](../../../category.md#terminal-object).

Equivalently, $LA$ represents the [categorical cone](../../../category.md#cone-over-a-diagram) [functor](../../../category.md#functor) $C\mapsto\operatorname{Nat}(\Delta_JC,DA)$, and [functoriality of chosen representations](../../../category.md#functoriality-of-chosen-representations) supplies the same $L$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Assume $F$ preserves existing [categorical limits](../../../category.md#categorical-limit). For a [diagram in a category](../../../category.md#diagram-category-theory) $E:I\to\mathcal B$ with [categorical limit](../../../category.md#categorical-limit) cone $\ell_i:L\to E_i$, its image $F\ell_i$ is a [categorical limit](../../../category.md#categorical-limit) cone of $FE$. For any $C\in\mathcal C$, a [morphism](../../../algebra.md#morphism) $C\to FL$ is therefore uniquely equivalent to a compatible family of [morphisms](../../../algebra.md#morphism) $C\to FE_i$. In the [Category of sets](../../../category.md#category-of-sets), compatible families are exactly the [categorical limit](../../../category.md#categorical-limit) of the resulting [hom-sets](../../../category.md#hom-set). Thus

$$
\boxed{\mathcal C(C,FL)\cong\lim_i\mathcal C(C,FE_i).}
$$

The maps are induced by $F\ell_i$, so **$\mathcal C(C,F-)$ preserves the given limit**. Applying this to every existing [categorical limit](../../../category.md#categorical-limit) proves the implication, with no completeness hypothesis on $\mathcal B$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Conversely, assume that every [hom-set](../../../category.md#hom-set) [functor](../../../category.md#functor) $\mathcal C(C,F-)$ preserves existing [categorical limits](../../../category.md#categorical-limit). For a [categorical limit](../../../category.md#categorical-limit) cone $\ell_i:L\to E_i$ in $\mathcal B$, a [categorical cone](../../../category.md#cone-over-a-diagram) $q_i:C\to FE_i$ determines an element of $\lim_i\mathcal C(C,FE_i)$. The assumed [bijection](../../../function.md#bijection)

$$
\mathcal C(C,FL)\longrightarrow\lim_i\mathcal C(C,FE_i),
\qquad u\longmapsto(F\ell_i\,u)_i
$$

gives one and only one such $u$ for every $C$ and every [categorical cone](../../../category.md#cone-over-a-diagram). That is the [universal property](../../../category-theory.md#universal-property) of the image cone itself. Therefore **the hom-set tests detect limit preservation**:

$$
\boxed{F\text{ preserves limits}\iff\mathcal C(C,F-)\text{ does so for every }C.}
$$

This proof works for all diagram sizes for which the relevant [categorical limits](../../../category.md#categorical-limit) and compatible-family [sets](../../../set.md) are under consideration.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The representing object in the [functor category](../../../category.md#functor-category) $[J,\mathcal C]$ is the constant [diagram in a category](../../../category.md#diagram-category-theory) $\Delta_JC$. If $p_j:\lim_jE_j\to E_j$ is the chosen [categorical limit](../../../category.md#categorical-limit) cone, the [natural bijection](../../../category.md#natural-bijection) is

$$
\boxed{\mathcal C(C,\lim_jE_j)\cong[J,\mathcal C](\Delta_JC,E),
\qquad f\longmapsto(p_jf)_j.}
$$

A [natural transformation](../../../category.md#natural-transformation) from the constant [diagram in a category](../../../category.md#diagram-category-theory) is precisely a [categorical cone](../../../category.md#cone-over-a-diagram) with vertex $C$, and its inverse is the unique mediating [morphism](../../../algebra.md#morphism) from the [universal property](../../../category-theory.md#universal-property) of the [categorical limit](../../../category.md#categorical-limit). For $\alpha:E\Rightarrow E'$, the defining equations for $\lim\alpha$ show that postcomposition by $\lim\alpha$ corresponds to postcomposition by $\alpha$ on the right. This establishes [naturality](../../../category.md#naturality) in $E$ and proves **representability by the constant diagram**.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For every $C$, the preceding part identifies the composite $\mathcal C(C,\lim_J-)$ with the covariant [representable functor](../../../category.md#representable-functor) $[J,\mathcal C](\Delta_JC,-)$. A covariant [representable functor](../../../category.md#representable-functor) preserves every existing [categorical limit](../../../category.md#categorical-limit), since a [morphism](../../../algebra.md#morphism) into a [categorical limit](../../../category.md#categorical-limit) is the same as a compatible family of [morphisms](../../../algebra.md#morphism) into the diagram objects. **The limit functor preserves limits.** The [hom-set detection of categorical limits](../../../category.md#hom-set-detection-of-categorical-limits) gives

$$
\boxed{\lim_J:[J,\mathcal C]\to\mathcal C\text{ preserves categorical limits}.}
$$

In particular, it preserves all small [categorical limits](../../../category.md#categorical-limit). They exist in $[J,\mathcal C]$: compute each one at every $j$ using completeness of $\mathcal C$, and use the uniqueness of the pointwise mediating [morphisms](../../../algebra.md#morphism) to obtain its [functor](../../../category.md#functor) structure and universal [natural transformations](../../../category.md#natural-transformation). Another expression of the same result is the [adjunction](../../../category.md#adjoint-functors) $\Delta_J\dashv\lim_J$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Regard the bifunctor as $D^{(2)}:K\to[J,\mathcal C]$. Its pointwise [categorical limit](../../../category.md#categorical-limit) $E=\lim_kD^{(2)}k$ satisfies

$$
E(j)=\lim_kD(j,k),
$$

with its action on [morphisms](../../../algebra.md#morphism) obtained by the construction in part (a). Applying the limit-preservation result from part (d) gives

$$
\boxed{\lim_j\lim_kD(j,k)
=\lim_J E\cong\lim_k\bigl(\lim_JD^{(2)}k\bigr)
=\lim_k\lim_jD(j,k).}
$$

The comparison [isomorphism](../../../algebra.md#isomorphism) is canonical relative to the chosen [categorical limit](../../../category.md#categorical-limit) cones: it is the unique [morphism](../../../algebra.md#morphism) identifying all the projections to $D(j,k)$. This proves **[commutation of iterated categorical limits](../../../category.md#commutation-of-iterated-categorical-limits)**, including an empty $J$ or $K$. Equivalently, both iterated constructions have the [universal property](../../../category-theory.md#universal-property) of the [categorical limit](../../../category.md#categorical-limit) of $D$ on $J\times K$.

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the orientation $F:\mathcal C\to\mathcal D$ and $G:\mathcal D\to\mathcal C$. An [adjunction](../../../category.md#adjoint-functors) $F\dashv G$ is equivalently specified by the [natural transformations](../../../category.md#natural-transformation)

$$
\eta:1_{\mathcal C}\Rightarrow GF,\qquad
\varepsilon:FG\Rightarrow1_{\mathcal D},
$$

called the [unit and counit of an adjunction](../../../category.md#unit-and-counit-of-an-adjunction), satisfying the [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction)

$$
\boxed{\varepsilon_{FC}\circ F(\eta_C)=1_{FC},\qquad
G(\varepsilon_D)\circ\eta_{GD}=1_{GD}.}
$$

The corresponding [natural bijection](../../../category.md#natural-bijection) is $\mathcal D(FC,D)\cong\mathcal C(C,GD)$, with $f\mapsto G(f)\eta_C$ and inverse $g\mapsto\varepsilon_DF(g)$. **The two triangular equations are the required compatibility conditions.** No proof of equivalence of the formulations is needed here.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Suppose $X\cong\mathcal C(-,R)$. As a [functor](../../../category.md#functor) on the [opposite category](../../../category.md#opposite-category), a [representable presheaf](../../../category.md#representable-functor) preserves every existing [categorical limit](../../../category.md#categorical-limit): a [colimit](../../../category.md#colimit) in $\mathcal C$ is defined by the [bijection](../../../function.md#bijection) between [morphisms](../../../algebra.md#morphism) from its vertex into $R$ and compatible families of [morphisms](../../../algebra.md#morphism) from its diagram objects into $R$. This remains valid for a possibly large [diagram in a category](../../../category.md#diagram-category-theory) whenever that [colimit](../../../category.md#colimit) exists and the compatible-family collection is the corresponding [set](../../../set.md).

The [category of elements](../../../category.md#category-of-elements) has a [terminal object](../../../category.md#terminal-object) $(R,r)$, where $r$ is the image of $1_R$ under the representation. For each $(C,x)$ let $u_{C,x}:C\to R$ be its unique [morphism](../../../algebra.md#morphism) to $(R,r)$. These form a [cocone](../../../category.md#cocone-under-a-diagram) for the [forgetful functor](../../../category.md#forgetful-functor) $G$. Any competing [cocone](../../../category.md#cocone-under-a-diagram) $v_{C,x}:C\to A$ satisfies

$$
v_{C,x}=v_{R,r}\,u_{C,x}.
$$

The component at $(R,r)$ uniquely determines the mediating [morphism](../../../algebra.md#morphism). Thus **the representing object is the colimit of the elements projection**:

$$
\boxed{\operatorname{colim}_{(C,x)\in\operatorname{Elts}(X)}C\cong R.}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Let $u_{C,x}:C\to R$ be a [colimit](../../../category.md#colimit) cocone for $G:\operatorname{Elts}(X)\to\mathcal C$. Here the preservation hypothesis must include the [categorical limit](../../../category.md#categorical-limit) of $G^{\mathrm{op}}$ in $\mathcal C^{\mathrm{op}}$; this indexing [category](../../../category.md) can be large. For a [morphism](../../../algebra.md#morphism) $f:(C,x)\to(D,y)$ of the [category of elements](../../../category.md#category-of-elements), the defining equation $X(f)(y)=x$ says that the family of distinguished elements $(x)_{(C,x)}$ is compatible. Preservation gives a unique $r\in X(R)$ with

$$
X(u_{C,x})(r)=x\quad\text{for every }(C,x).
$$

In particular each $u_{C,x}$ is now a [morphism](../../../algebra.md#morphism) $(C,x)\to(R,r)$ in the [category of elements](../../../category.md#category-of-elements). Naturality of the [colimit](../../../category.md#colimit) cocone gives

$$
u_{R,r}\,u_{C,x}=u_{C,x}.
$$

The [universal property](../../../category-theory.md#universal-property) of the [colimit](../../../category.md#colimit) forces $u_{R,r}=1_R$, since it and $1_R$ agree after every cocone leg. If $f:C\to R$ also satisfies $X(f)(r)=x$, it is a [morphism](../../../algebra.md#morphism) $(C,x)\to(R,r)$, and cocone compatibility now yields $u_{C,x}=u_{R,r}f=f$. Thus $(R,r)$ is a [universal element](../../../category.md#universal-element-of-a-set-valued-functor). By the preceding representability criterion, **the presheaf is represented by the colimit object**:

$$
\boxed{\mathcal C(-,R)\cong X,\qquad f\longmapsto X(f)(r).}
$$

The size qualification matters. If preservation means only small [categorical limits](../../../category.md#categorical-limit), the implication as printed is false for general [locally small categories](../../../category.md#locally-small-category). For an explicit counterexample, let $\mathcal C$ be the ordered [category](../../../category.md) of all [ordinals](../../../set-theory.md#ordinal) with an extra greatest object $\infty$. Put $X(\alpha)=\{*\}$ for every [ordinal](../../../set-theory.md#ordinal) $\alpha$ and $X(\infty)=\varnothing$, with the forced restriction maps. Every small [colimit](../../../category.md#colimit) in $\mathcal C$ is the supremum of its object values: it is an [ordinal](../../../set-theory.md#ordinal) unless the diagram contains $\infty$. Applying $X$ therefore gives the appropriate small [categorical limit](../../../category.md#categorical-limit) of singletons, or the empty [set](../../../set.md) when a value is empty; an empty diagram gives $X(0)=\{*\}$. Hence $X$ preserves all small [categorical limits](../../../category.md#categorical-limit).

Its [category of elements](../../../category.md#category-of-elements) consists of all [ordinals](../../../set-theory.md#ordinal), whose projection has the large [colimit](../../../category.md#colimit) $\infty$ in $\mathcal C$. Nevertheless, no [ordinal](../../../set-theory.md#ordinal) represents $X$, because its representable vanishes on larger ordinals; $\infty$ does not represent it either, since $\mathcal C(\infty,\infty)$ is nonempty while $X(\infty)$ is empty. The valid proof consequently uses preservation of the displayed possibly large limit, or a smallness hypothesis making that diagram small.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [right-adjoint criterion using comma-category colimits](../../../category.md#right-adjoint-criterion-using-comma-category-colimits) is as follows. Under the given colimit-preservation hypothesis, with preservation including the possibly large colimits below, $F:\mathcal X\to\mathcal A$ has a [right adjoint](../../../category.md#adjoint-functors) exactly when, for every $A$, the projection

$$
U_A:(F\downarrow A)\to\mathcal X,\qquad (X,f:FX\to A)\longmapsto X
$$

has a [colimit](../../../category.md#colimit) in $\mathcal X$. **The right adjoint is obtained from these comma-category colimits.** Thus the objects to construct are

$$
\boxed{GA=\operatorname{colim}_{(X,f)\in(F\downarrow A)}X.}
$$

For necessity, if $F\dashv G$ with [adjunction counit](../../../category.md#counit-of-an-adjunction) $\varepsilon$, $(GA,\varepsilon_A)$ is a [terminal object](../../../category.md#terminal-object) of the [comma category](../../../category.md#comma-category) $(F\downarrow A)$. Its unique incoming [morphisms](../../../algebra.md#morphism) give a [colimit](../../../category.md#colimit) cocone for $U_A$, exactly as for the elements projection in the preceding part.

For sufficiency, choose such a [colimit](../../../category.md#colimit) $L$ with legs $u_{X,f}:X\to L$. The [morphisms](../../../algebra.md#morphism) $f:FX\to A$ are a [cocone](../../../category.md#cocone-under-a-diagram) on $FU_A$. Since $F$ preserves this [colimit](../../../category.md#colimit), there is a unique $\varepsilon_A:FL\to A$ satisfying

$$
\varepsilon_A F(u_{X,f})=f.
$$

Each $u_{X,f}$ is thus a [morphism](../../../algebra.md#morphism) $(X,f)\to(L,\varepsilon_A)$ in the [comma category](../../../category.md#comma-category). The original [colimit](../../../category.md#colimit) cocone gives $u_{L,\varepsilon_A}u_{X,f}=u_{X,f}$ for every object, hence $u_{L,\varepsilon_A}=1_L$ by the [universal property](../../../category-theory.md#universal-property). For any other [morphism](../../../algebra.md#morphism) $h:(X,f)\to(L,\varepsilon_A)$, cocone compatibility gives

$$
u_{X,f}=u_{L,\varepsilon_A}h=h.
$$

So $(L,\varepsilon_A)$ is a [terminal object](../../../category.md#terminal-object). Equivalently, $L$ represents the [categorical presheaf](../../../category.md#presheaf-category-theory) $\mathcal A(F-,A)$, via $h\mapsto\varepsilon_A Fh$. The [functoriality of chosen representations](../../../category.md#functoriality-of-chosen-representations) makes these $L$ into $G:\mathcal A\to\mathcal X$, yielding a [natural bijection](../../../category.md#natural-bijection)

$$
\boxed{\mathcal X(X,GA)\cong\mathcal A(FX,A),\qquad F\dashv G.}
$$

The preservation of these possibly large [colimits](../../../category.md#colimit) is essential to the construction of $\varepsilon_A$. Under a small-only interpretation, the preceding [ordinal](../../../set-theory.md#ordinal) counterexample also disproves the unqualified converse here. Take $F=X^{\mathrm{op}}:\mathcal C\to\mathbf{Set}^{\mathrm{op}}$. It preserves all small [colimits](../../../category.md#colimit). For a nonempty [set](../../../set.md) $A$, the [comma category](../../../category.md#comma-category) $(F\downarrow A)$ has one object over each [ordinal](../../../set-theory.md#ordinal) and none over $\infty$, so its projection has [colimit](../../../category.md#colimit) $\infty$. For $A=\varnothing$, the projection is the identity of $\mathcal C$, again with [colimit](../../../category.md#colimit) $\infty$. Thus all these projection colimits exist, but $F$ has no [right adjoint](../../../category.md#adjoint-functors): the [categorical presheaf](../../../category.md#presheaf-category-theory) $\mathbf{Set}^{\mathrm{op}}(F-,\{*\})=X$ is not [representable](../../../category.md#representable-functor). This makes the large-preservation qualification substantive.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) has the following limit form. Let $U:\mathcal C\to\mathcal D$ be a [functor](../../../category.md#functor), where $\mathcal C$ is a [complete category](../../../category.md#complete-category) and both [categories](../../../category.md) are [locally small](../../../category.md#locally-small-category). Then **$U$ has a left adjoint exactly when it preserves small limits and satisfies the solution-set condition**.

The [solution-set condition](../../../category.md#solution-set-condition) requires that, for each $D\in\mathcal D$, there be a [set](../../../set.md) of pairs $(C_i,d_i:D\to UC_i)$ such that every $d:D\to UC$ factors as

$$
\boxed{d=U(h)d_i\quad\text{for some }i\text{ and }h:C_i\to C.}
$$

Equivalently, each [comma category](../../../category.md#comma-category) $(D\downarrow U)$ has a [weakly initial set](../../../category.md#weakly-initial-set). All completeness and preservation requirements here concern small [categorical limits](../../../category.md#categorical-limit). Dually, a small-colimit-preserving [functor](../../../category.md#functor) from a [cocomplete category](../../../category.md#cocomplete-category) has a [right adjoint](../../../category.md#adjoint-functors) precisely when each $(U\downarrow D)$ has a [weakly terminal set](../../../category.md#weakly-terminal-set).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Special adjoint functor theorem](../../../category.md#special-adjoint-functor-theorem) says: if $\mathcal C$ is a [locally small category](../../../category.md#locally-small-category), a [complete category](../../../category.md#complete-category), a [well-powered category](../../../category.md#well-powered-category), and has a [small cogenerating family](../../../category.md#cogenerating-set), then a [functor](../../../category.md#functor) $U:\mathcal C\to\mathcal D$ into any [locally small category](../../../category.md#locally-small-category) has a [left adjoint](../../../category.md#adjoint-functors) if and only if it preserves small [categorical limits](../../../category.md#categorical-limit).

A [small cogenerating family](../../../category.md#cogenerating-set) $(Q_i)_{i\in I}$, with $I$ a [set](../../../set.md), distinguishes unequal parallel [morphisms](../../../algebra.md#morphism) by postcomposition: for $f\ne g:A\to B$, some $q:B\to Q_i$ has $qf\ne qg$. Being [well-powered](../../../category.md#well-powered-category) means that the [subobjects](../../../category.md#subobject) of each object form a [set](../../../set.md) up to the usual equivalence of [monomorphisms](../../../category.md#monomorphism). **These hypotheses make the solution-set condition automatic.**

The dual formulation uses a [cocomplete category](../../../category.md#cocomplete-category), being a [well-copowered category](../../../category.md#well-copowered-category) and having a [small generating family](../../../category.md#generating-set-in-a-category), and concludes that every small-colimit-preserving [functor](../../../category.md#functor) has a [right adjoint](../../../category.md#adjoint-functors).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

It is enough to prove the [solution-set condition](../../../category.md#solution-set-condition) and then apply the [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem). Fix $D\in\mathcal D$ and a [morphism](../../../algebra.md#morphism) $d:D\to UC$. We will factor it through one object in a [set](../../../set.md) depending only on $D$.

First construct a [minimal supported subobject](../../../category.md#minimal-supported-subobject). Among the [subobjects](../../../category.md#subobject) $m:M\hookrightarrow C$ for which $d=U(m)d_M$ for some $d_M:D\to UM$, include $1_C$ and take their intersection $m_0:C_0\hookrightarrow C$. This is a small intersection, by well-poweredness. It exists by completeness as the [categorical limit](../../../category.md#categorical-limit) of the diagram consisting of these [monomorphisms](../../../category.md#monomorphism) into $C$. Its map to $C$ is a [monomorphism](../../../category.md#monomorphism): two maps with the same composite to $C$ have equal projections to every $M$, since each $m$ is monic, and are then equal by the [categorical limit](../../../category.md#categorical-limit) property. One can equivalently construct these intersections by [pullbacks in a category](../../../category.md#pullback-category-theory) and small [products in a category](../../../category.md#product-category-theory), using stability of [monomorphisms](../../../category.md#monomorphism) under [pullback in a category](../../../category.md#pullback-category-theory).

Choose the factorizations $d_M$. They form a compatible [categorical cone](../../../category.md#cone-over-a-diagram) into the image diagram under $U$, all with common composite $d$ to $UC$. Preservation of small [categorical limits](../../../category.md#categorical-limit) yields $d_0:D\to UC_0$ with $U(m_0)d_0=d$. If $n:N\hookrightarrow C_0$ is another [subobject](../../../category.md#subobject) through which $d_0$ factors after applying $U$, then $m_0n$ is among the original supported [subobjects](../../../category.md#subobject). The intersection property gives $r:C_0\to N$ with $m_0nr=m_0$. Since $m_0$ is monic, $nr=1_{C_0}$; since $n$ is monic, also $rn=1_N$. Thus **every supported subobject of $C_0$ is invertible**.

For each member $Q_i$ of the [small cogenerating family](../../../category.md#cogenerating-set), consider

$$
\theta_i:\mathcal C(C_0,Q_i)\longrightarrow\mathcal D(D,UQ_i),\qquad q\longmapsto U(q)d_0.
$$

This map is [injective](../../../algebra.md#injective-function). If $U(q)d_0=U(q')d_0$, preservation of the [equalizer](../../../category.md#equaliser) of $q,q'$ makes $d_0$ factor through the image of that [equalizer](../../../category.md#equaliser). Minimality makes its inclusion an [isomorphism](../../../algebra.md#isomorphism), so $q=q'$.

Write $R_i=\mathcal D(D,UQ_i)$; it is a [set](../../../set.md) by local smallness of $\mathcal D$. Let $S_i\subseteq R_i$ be the image of $\theta_i$. For each $s\in S_i$, there is exactly one corresponding $q_{i,s}:C_0\to Q_i$. These maps define the [evaluation embedding into cogenerator products](../../../category.md#evaluation-embedding-into-cogenerator-products)

$$
e:C_0\longrightarrow P_S:=\prod_{i\in I}\prod_{s\in S_i}Q_i.
$$

It is a [monomorphism](../../../category.md#monomorphism): if $eg=eh$ and $g\ne h$, cogeneration supplies some $q:C_0\to Q_i$ distinguishing $g,h$; that $q$ is one of the projections of $e$, a contradiction. The product is small. It is important to use the subfamilies $S_i$, since some missing coordinate in $R_i$ need not correspond to a [morphism](../../../algebra.md#morphism) out of $C_0$.

There are only a [set](../../../set.md) of possible families $(S_i\subseteq R_i)_{i\in I}$. For each such family form $P_S$, choose a [set](../../../set.md) of representatives $N\hookrightarrow P_S$ of its [subobjects](../../../category.md#subobject), and take all pairs $(N,d_N:D\to UN)$. Local smallness of $\mathcal D$ and well-poweredness make their union a [set](../../../set.md). In the case just constructed, $e$ identifies $C_0$ with one chosen representative $N$. Transporting $d_0$ to $UN$ and composing the inverse identification with $m_0$ gives a factorization of the original $d$ through that pair. Therefore these pairs form a [weakly initial set](../../../category.md#weakly-initial-set) in $(D\downarrow U)$.

The [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) now supplies a [left adjoint](../../../category.md#adjoint-functors) to $U$. Conversely, a [right adjoint](../../../category.md#adjoint-functors) preserves small [categorical limits](../../../category.md#categorical-limit), either by the [adjunction](../../../category.md#adjoint-functors) [hom-set](../../../category.md#hom-set) bijections and the [hom-set detection of categorical limits](../../../category.md#hom-set-detection-of-categorical-limits), or directly from their [universal properties](../../../category-theory.md#universal-property). Hence **the stated special theorem is proved in both directions**.

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $K:\mathcal B\to\mathcal C$, $J:\mathcal C\to\mathcal B$, with [adjunction unit](../../../category.md#unit-of-an-adjunction) $\rho$ and [adjunction counit](../../../category.md#counit-of-an-adjunction) $\varepsilon$. The [adjunction](../../../category.md#adjoint-functors) gives

$$
\mathcal C(KJC,C')\cong\mathcal B(JC,JC'),\qquad h\longmapsto J(h)\rho_{JC}.
$$

For $f:C\to C'$, precomposition with $\varepsilon_C$ followed by this [bijection](../../../function.md#bijection) gives

$$
J(f\varepsilon_C)\rho_{JC}=Jf,
$$

by the [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction). Thus $J$ is [fully faithful](../../../category.md#full-and-faithful-functor) exactly when precomposition with $\varepsilon_C$ is bijective for every $C,C'$.

A [morphism](../../../algebra.md#morphism) $e:P\to Q$ with this property is an [isomorphism](../../../algebra.md#isomorphism). Surjectivity for target $P$ supplies $u:Q\to P$ with $ue=1_P$. Since $(eu)e=e=1_Qe$, injectivity for target $Q$ gives $eu=1_Q$. Conversely, precomposition with an [isomorphism](../../../algebra.md#isomorphism) is always bijective. Applied to every $\varepsilon_C$, this proves **the fully faithful right-adjoint criterion**:

$$
\boxed{J\text{ is fully faithful}\iff\varepsilon:KJ\Rightarrow1_{\mathcal C}\text{ is a natural isomorphism}.}
$$

When the [adjunction counit](../../../category.md#counit-of-an-adjunction) is invertible, the inverse to $f\mapsto Jf$ is explicitly $h\mapsto\varepsilon_{C'}K(h)\varepsilon_C^{-1}$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

If $B$ belongs to the [full subcategory](../../../category.md#full-subcategory) $\mathcal C$, the [adjunction](../../../category.md#adjoint-functors) and fullness of its inclusion give, for every $B'\in\mathcal B$,

$$
\boxed{\mathcal B(KB',B)=\mathcal C(KB',B)\cong\mathcal B(B',B),
\qquad h\longmapsto h\rho_{B'}.}
$$

Therefore **membership implies the hom-set condition**. In addition, $J$ is [fully faithful](../../../category.md#full-and-faithful-functor), so the [adjunction counit](../../../category.md#counit-of-an-adjunction) is invertible by the preceding criterion. The triangular equation $J\varepsilon_B\,\rho_B=1_B$ then shows that $\rho_B$ is an [isomorphism](../../../algebra.md#isomorphism). As in the printed inclusion notation, $J$ is suppressed when writing $KB$ as an object of $\mathcal B$.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Assume the [hom-set](../../../category.md#hom-set) condition. Its surjectivity at $B'=B$ gives $u:KB\to B$ with $u\rho_B=1_B$. We show that this splitting is two-sided.

Because $J$ is [fully faithful](../../../category.md#full-and-faithful-functor), $\varepsilon_{KB}$ is invertible. Both [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give, after suppressing $J$,

$$
K\rho_B=\rho_{KB}=\varepsilon_{KB}^{-1}.
$$

Applying $K$ to $u\rho_B=1_B$ yields $Ku\,\rho_{KB}=1_{KB}$. [Naturality](../../../category.md#naturality) of the [adjunction unit](../../../category.md#unit-of-an-adjunction) at $u$ gives $\rho_Bu=Ku\,\rho_{KB}$, hence $\rho_Bu=1_{KB}$. Consequently **the hom-set condition forces the unit to be invertible**:

$$
\boxed{\rho_B^{-1}=u.}
$$

Only surjectivity at $B'=B$ was needed for this direction; the given family of [bijections](../../../function.md#bijection) certainly supplies it.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

If $\rho_B:B\to KB$ is an [isomorphism](../../../algebra.md#isomorphism), then $B$ is isomorphic in $\mathcal B$ to an object of $\mathcal C$. Since $\mathcal C$ is a [replete subcategory](../../../category.md#replete-subcategory), it contains $B$. Thus **invertibility of the unit implies membership**, completing the cycle of implications:

$$
\boxed{B\in\mathcal C\iff
\bigl[h\mapsto h\rho_{B'}\text{ is bijective for every }B'\bigr]
\iff\rho_B\text{ is invertible}.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $J:\mathcal C\hookrightarrow\mathcal B$ exhibit a [reflective subcategory](../../../category.md#reflective-subcategory), with [reflector](../../../category.md#reflector) $K$, and let $E:I\to\mathcal C$ be a small [diagram in a category](../../../category.md#diagram-category-theory). Completeness of $\mathcal B$ gives a [categorical limit](../../../category.md#categorical-limit) $L$ of $JE$. For every $B'\in\mathcal B$, the [universal property](../../../category-theory.md#universal-property) of this [categorical limit](../../../category.md#categorical-limit) and the reflection [adjunction](../../../category.md#adjoint-functors) give

$$
\begin{aligned}
\mathcal B(JKB',L)
&\cong\lim_i\mathcal B(JKB',JE_i)\\
&\cong\lim_i\mathcal B(B',JE_i)\\
&\cong\mathcal B(B',L).
\end{aligned}
$$

The composite is precomposition with $\rho_{B'}$, so $L$ satisfies the [hom-set](../../../category.md#hom-set) condition from the preceding part. Its proof of invertibility of $\rho_L$ did not require repleteness. Thus $L\cong JKL$ whether or not the chosen full reflective subcategory is replete.

Transport the ambient limit cone along $\rho_L^{-1}:JKL\to L$. Its legs lie in the [full subcategory](../../../category.md#full-subcategory), and their ambient [universal property](../../../category-theory.md#universal-property), restricted to objects of $\mathcal C$, is exactly the internal [categorical limit](../../../category.md#categorical-limit) property. Hence **every small diagram in the reflective subcategory has a limit**:

$$
\boxed{\mathcal C\text{ is complete, with a chosen limit }KL.}
$$

For a [replete subcategory](../../../category.md#replete-subcategory), the ambient limit object $L$ itself belongs to $\mathcal C$. This argument includes the empty diagram and requires no limit-preservation hypothesis on the [reflector](../../../category.md#reflector).

## 6

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For the [monad](../../../category-theory.md#monad) $\mathbb T=(T,\eta,\mu)$ define the [free algebra functor](../../../category-theory.md#free-algebra-functor) by

$$
F^{\mathbb T}X=(TX,\mu_X),\qquad F^{\mathbb T}f=Tf.
$$

The unit and associativity identities of the [monad](../../../category-theory.md#monad) make $(TX,\mu_X)$ an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad), and [naturality](../../../category.md#naturality) of $\mu$ makes $Tf$ a [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad). Let $G^{\mathbb T}$ be the [forgetful functor](../../../category.md#forgetful-functor). For $(A,a)$ in the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category), set

$$
\Phi(h)=h\eta_X,\qquad \Psi(f)=a\,Tf.
$$

The inverse candidate is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad), since

$$
a\,Tf\,\mu_X=a\mu_A\,T^2f=a\,Ta\,T^2f
=a\,T(a\,Tf).
$$

The two composites are identities:

$$
\Phi\Psi(f)=a\eta_Af=f,\qquad
\Psi\Phi(h)=a\,Th\,T\eta_X=h\mu_X\,T\eta_X=h.
$$

These use respectively the [unit law for a monad algebra](../../../category-theory.md#unit-law-for-a-monad-algebra), the algebra-morphism equation, and a unit identity of the [monad](../../../category-theory.md#monad). The formulas commute with precomposition in $X$ and postcomposition by [monad algebra morphisms](../../../category-theory.md#morphism-of-algebras-for-a-monad), so they form a [natural bijection](../../../category.md#natural-bijection). Therefore **the free-algebra functor is left adjoint to forgetting**:

$$
\boxed{\mathcal X^{\mathbb T}(F^{\mathbb T}X,(A,a))\cong\mathcal X(X,A),
\qquad F^{\mathbb T}\dashv G^{\mathbb T}.}
$$

Its [adjunction unit](../../../category.md#unit-of-an-adjunction) is $\eta_X$, and its [adjunction counit](../../../category.md#counit-of-an-adjunction) at $(A,a)$ is $a:(TA,\mu_A)\to(A,a)$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Write $F:\mathcal X\to\mathcal A$ and $G:\mathcal A\to\mathcal X$, with [adjunction counit](../../../category.md#counit-of-an-adjunction) $\varepsilon$. The induced [monad](../../../category-theory.md#monad) has $T=GF$ and $\mu=G\varepsilon F$. Define the [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) by

$$
\boxed{K(A)=(GA,G\varepsilon_A),\qquad K(f)=Gf.}
$$

The action $a_A=G\varepsilon_A:TGA\to GA$ satisfies $a_A\eta_{GA}=1_{GA}$ by a triangular equation. [Naturality](../../../category.md#naturality) of $\varepsilon$ at $\varepsilon_A:FGA\to A$ gives

$$
\varepsilon_A FG\varepsilon_A=\varepsilon_A\varepsilon_{FGA}.
$$

Applying $G$ yields $a_A T(a_A)=a_A\mu_{GA}$, the other algebra identity. For $f:A\to A'$, [naturality](../../../category.md#naturality) gives

$$
Gf\,G\varepsilon_A=G\varepsilon_{A'}\,GF(Gf),
$$

so $Gf$ is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad). Identities and compositions are respected because $G$ is a [functor](../../../category.md#functor). Finally,

$$
G^{\mathbb T}K(A)=GA,\qquad
KF(X)=(GFX,G\varepsilon_{FX})=(TX,\mu_X)=F^{\mathbb T}X,
$$

and the same equalities hold on [morphisms](../../../algebra.md#morphism). Thus **both comparison identities hold**, strictly when $\mathbb T$ is the specified induced [monad](../../../category-theory.md#monad):

$$
\boxed{G^{\mathbb T}K=G,\qquad KF=F^{\mathbb T}.}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

If the multiplication in the [unit and multiplication of a monad](../../../category-theory.md#unit-and-multiplication-of-a-monad) $\mu$ is invertible, the two unit identities of the [monad](../../../category-theory.md#monad)

$$
\mu\circ T\eta=1_T,\qquad \mu\circ\eta T=1_T
$$

make both $T\eta$ and $\eta T$ its inverse. Hence **idempotence implies equality of the two unit insertions**:

$$
\boxed{T\eta=\eta T=\mu^{-1}.}
$$

This is the first implication in the characterization of an [idempotent monad](../../../category-theory.md#idempotent-monad).

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

Assume $T\eta=\eta T$, and let $(A,a)$ be an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad). Its unit identity gives $a\eta_A=1_A$. [Naturality](../../../category.md#naturality) of $\eta$ at $a:TA\to A$, followed by the assumed equality, gives

$$
\eta_Aa=Ta\,\eta_{TA}=Ta\,T\eta_A=T(a\eta_A)=1_{TA}.
$$

Thus **every algebra action is invertible**, with its inverse prescribed by the unit:

$$
\boxed{a^{-1}=\eta_A.}
$$

<h4 id="6/c/iii">iii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/c/iii)

Suppose every algebra action is an [isomorphism](../../../algebra.md#isomorphism). Its inverse is $\eta_A$, by the [unit law for a monad algebra](../../../category-theory.md#unit-law-for-a-monad-algebra). For any underlying [morphism](../../../algebra.md#morphism) $f:A\to B$ between two [algebras for a monad](../../../category-theory.md#algebra-for-a-monad), [naturality](../../../category.md#naturality) of $\eta$ gives

$$
\eta_B f=Tf\,\eta_A\quad\Longrightarrow\quad
fa=b\,Tf.
$$

Therefore every underlying [morphism](../../../algebra.md#morphism) is automatically a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad). The [forgetful functor](../../../category.md#forgetful-functor) is always faithful, because a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) has no data beyond its underlying [morphism](../../../algebra.md#morphism), and it is now full as well. Hence **invertible algebra actions imply**

$$
\boxed{G^{\mathbb T}:\mathcal X^{\mathbb T}\to\mathcal X\text{ is fully faithful}.}
$$

<h4 id="6/c/iv">iv</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/c/iv)

If $G^{\mathbb T}$ is [fully faithful](../../../category.md#full-and-faithful-functor), the criterion proved for a [right adjoint](../../../category.md#adjoint-functors) says that the [adjunction counit](../../../category.md#counit-of-an-adjunction) of $F^{\mathbb T}\dashv G^{\mathbb T}$ is a [natural isomorphism](../../../category.md#natural-isomorphism). Its component at $(A,a)$ is precisely the algebra action $a$. In particular, its component at the free [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) $(TX,\mu_X)$ has underlying [morphism](../../../algebra.md#morphism) $\mu_X:T^2X\to TX$. Thus every $\mu_X$ is an [isomorphism](../../../algebra.md#isomorphism), and the [natural transformation](../../../category.md#natural-transformation) $\mu$ is invertible. **This closes the cycle and proves all four conditions equivalent**:

$$
\boxed{\mu\text{ invertible}\iff T\eta=\eta T
\iff\text{every algebra action is invertible}
\iff G^{\mathbb T}\text{ is fully faithful}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
