# Paper 119

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_119.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_119.pdf)

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
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
    - [iv](#4/b/iv)
      - [Solution](#4/b/iv/solution)
    - [v](#4/b/v)
      - [Solution](#4/b/v/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For $A\in\mathcal C$ and $F:\mathcal C\to\mathbf{Set}$, the [Yoneda lemma](../../../category.md#yoneda-lemma) gives a natural bijection

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),
\qquad \alpha\longmapsto\alpha_A(1_A).
$$

Assume $\mathcal C$ is small. For every pair $(A,x)$ with $x\in F(A)$, let $\alpha^{A,x}:\mathcal C(A,-)\to F$ be the corresponding natural transformation. Their copairing is

$$
\coprod_{A\in\mathcal C}\coprod_{x\in F(A)}
\mathcal C(A,-)\longrightarrow F.
$$

At an object $B$, the element $x\in F(B)$ is the image of $1_B$ in the summand indexed by $(B,x)$. The map is therefore pointwise surjective and hence an [epimorphism](../../../category.md#epimorphism) in the [functor category](../../../category.md#functor-category).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $P:\mathcal E\to\mathcal D$ be a [discrete fibration](../../../category.md#discrete-fibration) and let $m:A\to A'$ be monic in $\mathcal E$. If $u,v:B\to P(A)$ satisfy $P(m)u=P(m)v$, lift $u,v$ uniquely to $\widetilde u,\widetilde v$ with codomain $A$. The composites $m\widetilde u,m\widetilde v$ are lifts of the same arrow with codomain $A'$, so uniqueness gives equality. Since $m$ is monic, $\widetilde u=\widetilde v$, hence $u=v$. Thus $P(m)$ is monic.

Use the convention that $(F\downarrow B)$ has objects $(A,u:FA\to B)$. Its forgetful functor sends $(A,u)$ to $A$. Given $h:C\to A$, the unique arrow above $h$ with codomain $(A,u)$ has domain $(C,uFh)$. Hence the forgetful functor is a discrete fibration.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Assume every morphism of $\mathcal C$ is monic. For a representable presheaf $F=\mathcal C(-,A)$, the category $(1\downarrow F)$ is the [category of elements](../../../category.md#category-of-elements), equivalently the slice $\mathcal C/A$. A morphism from $f:B\to A$ to $g:C\to A$ is an $h:B\to C$ satisfying $gh=f$. Since $g$ is monic, there is at most one such $h$. Thus $(1\downarrow F)$ is a [preorder](../../../set.md#preorder).

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Assume every category of elements of a representable presheaf is a preorder. Let

$$
P=\coprod_{A\in\operatorname{ob}\mathcal C}(1\downarrow\mathcal C(-,A)).
$$

A disjoint union of preorders is a preorder. The category-of-elements projection $P\to\mathcal C$ is a [discrete fibration](../../../category.md#discrete-fibration). It is surjective on objects because $B\in\mathcal C$ is the image of the object $1_B:B\to B$ in the summand indexed by $B$.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Suppose a preorder $P$ admits a discrete fibration $q:P\to\mathcal C$ that is surjective on objects. Given $f:B\to A$ in $\mathcal C$, choose $a\in P$ above $A$. The discrete-fibration property lifts $f$ to $\widetilde f:b\to a$. Every arrow in a preorder is monic, and a [discrete fibration](../../../category.md#discrete-fibration) preserves monomorphisms by part (b), so $f=q(\widetilde f)$ is monic. This proves the remaining implication and hence the equivalence.

## 2

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [categorical limit](../../../category.md#categorical-limit) of $D:\mathcal J\to\mathcal C$ is a terminal cone $(L,(p_j))$: every cone $(X,(x_j))$ has a unique map $X\to L$ commuting with all legs.

Assume all small products and [equalizers](../../../category.md#equaliser) exist. Put

$$
P=\prod_{j\in\mathcal J}D(j),
\qquad
Q=\prod_{u:i\to j}D(j).
$$

Define $s,t:P\rightrightarrows Q$ so that the $u:i\to j$ components are

$$
s_u=D(u)\pi_i,\qquad t_u=\pi_j.
$$

A map $X\to P$ equalizes $s,t$ exactly when its components form a cone over $D$. Therefore $\operatorname{eq}(s,t)$ represents cones and is the limit. This is the [construction of small limits from products and equalizers](../../../category.md#construction-of-small-limits-from-products-and-equalizers).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $D:\mathcal J\to\mathbf{Fld}$ be connected and nonempty. The limit of the underlying diagram of [commutative rings](../../../commutative-algebra.md#commutative-ring) is the subring

$$
L=\left\{(x_j)\in\prod_jD(j):
D(u)(x_i)=x_j\text{ for every }u:i\to j\right\}.
$$

If $x\in L$ is nonzero in one component, it is nonzero in every component: field homomorphisms are injective, and connectedness propagates this fact along zigzags. Hence the componentwise inverses $(x_j^{-1})$ are defined and compatible. Thus $L$ is a field. Since the inclusion $\mathbf{Fld}\hookrightarrow\mathbf{CRng}$ is full, the same cone is limiting in the [category of fields](../../../category.md#category-of-fields).

If $\mathcal J$ is disconnected, choose two components and use the constant field $\mathbb F_2$ on one and $\mathbb F_3$ on the other. There is no cone in fields because its apex would map to fields of two different characteristics. Hence $\mathbf{Fld}$ does not have all limits of any disconnected shape.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Consider one connected component $K$ of the category of cocones under a small diagram $D:\mathcal J\to\mathbf{Fld}$. Replace every apex by the subfield generated by the images of the fields $D(j)$. These generated fields have cardinality bounded in terms of the small diagram, so they admit a small skeleton, cofinal within $K$.

The apex functor on this small connected category has a limit $L_K$ in $\mathbf{Fld}$ by part (b). For each $j$, the maps from $D(j)$ to all apexes form a compatible cone and therefore induce $D(j)\to L_K$. These maps form a cocone $\lambda_K$ under $D$. Its limiting projections give a unique morphism from $\lambda_K$ to every cocone in $K$, so $\lambda_K$ is initial in that component. Choosing one $\lambda_K$ for each component gives a [multicolimit](../../../category.md#multicolimit).

## 3

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [adjoint functor theorem for complete lattices](../../../category.md#adjoint-functor-theorem-for-complete-lattices) says that a monotone map $f:A\to B$ between complete lattices preserves arbitrary joins exactly when it has a right adjoint

$$
f^*(b)=\bigvee\{a:f(a)\leq b\}.
$$

A right adjoint preserves arbitrary meets. Regard it as the join-preserving map

$$
f^*:B^{\mathrm{op}}\longrightarrow A^{\mathrm{op}}.
$$

Thus define $A^*=A^{\mathrm{op}}$ and send $f$ to its right adjoint. Since a left adjoint is the right adjoint of its right adjoint after reversing orders, $(f^*)^*=f$ and $(A^*)^*=A$. This gives the involutive self-duality

$$
\boxed{(-)^*:\mathbf{CSLat}^{\mathrm{op}}\longrightarrow\mathbf{CSLat}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $[A,B]$ be the set of arbitrary-join-preserving maps $A\to B$, ordered pointwise. Pointwise joins remain join-preserving because the two joins may be interchanged:

$$
\left(\bigvee_i f_i\right)\left(\bigvee_j a_j\right)
=\bigvee_{i,j}f_i(a_j).
$$

Precomposition and postcomposition preserve these joins, so $(A,B)\mapsto[A,B]$ is the required $\mathbf{CSLat}$-valued hom functor.

Sending $f:A\to B$ to its right adjoint gives

$$
[B^*,A^*]\cong[A,B].
$$

It is order-preserving because taking a right adjoint reverses pointwise order once, while the order on $A^*$ reverses it again.

A join map $\chi_a:A\to2$ is associated with $a\in A$ by

$$
\chi_a(x)=0\Longleftrightarrow x\leq a.
$$

Every join map to $2$ is of this form, and $a\mapsto\chi_a$ identifies $A^*$ with $[A,2]$. Finally, a map $A\to[B,C]$ is a function $A\times B\to C$ preserving arbitrary joins separately in each variable. Swapping the variables gives naturally

$$
\boxed{[A,[B,C]]\cong[B,[A,C]].}
$$

The assumed expression of $C$ as a limit of copies of $2$ reduces the verification to the preceding $2$-valued description.

## 4

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For an adjunction $F\dashv U:\mathcal D\to\mathcal C$ with induced monad $T=UF$, the [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) is

$$
K:\mathcal D\to\mathcal C^T,\qquad
K(D)=(UD,U\varepsilon_D).
$$

The adjunction is [monadic](../../../category-theory.md#monadic-adjunction) when $K$ is an equivalence.

The [Crude monadicity theorem](../../../category-theory.md#crude-monadicity-theorem) states that a right adjoint is monadic if it reflects isomorphisms, its source has coequalizers of reflexive pairs, and it preserves those coequalizers. The dual statement is the crude comonadicity theorem.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Assume the free functor reflects isomorphisms. If $f,g:X\rightrightarrows Y$ satisfy $Ff=Fg$, let $q:Y\to Q$ be their coequalizer in sets. As a left adjoint, $F$ preserves it. Since the coequalizer of an equal pair is an identity, $Fq$ is an isomorphism. Reflection makes $q$ an isomorphism, so $f=g$. Thus $F$ is faithful.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Assume $F$ is faithful. If $\eta_X(x)=\eta_X(y)$, regard $x,y$ as maps $1\rightrightarrows X$. Their free extensions are $F(x),F(y):F1\rightrightarrows FX$, and the adjunction identifies these with $\eta_Xx,\eta_Xy$. They are equal, so faithfulness gives $x=y$. Hence every unit component $\eta_X:X\to TX$ is monic.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Pointwise monicity of the unit immediately implies that

$$
\eta_2:2\longrightarrow T2
$$

is monic.

<h4 id="4/b/iv">iv</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/b/iv)

If $\eta_2$ is monic, then $\eta_2(0)\neq\eta_2(1)$. The free algebra $(T2,\mu_2)$ therefore has more than one element, proving the existence of a nontrivial $T$-algebra.

<h4 id="4/b/v">v</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/v/solution">Solution</h5>

↑ **Parent:** [V](#4/b/v)

Let $(A,a)$ be a $T$-algebra with at least two elements, and suppose $Ff:FX\to FY$ is an isomorphism. For every $T$-algebra $A$, precomposition with $Ff$ gives a bijection

$$
\mathbf{Set}^T(FY,A)\longrightarrow\mathbf{Set}^T(FX,A).
$$

By the free-forgetful adjunction this is

$$
\mathbf{Set}(Y,UA)\longrightarrow\mathbf{Set}(X,UA),
\qquad h\longmapsto hf.
$$

For one set $UA$ with at least two elements, bijectivity of this precomposition forces $f$ to be bijective: surjectivity detects injectivity of $f$, and injectivity detects surjectivity. Thus $f$ is an isomorphism. The free functor reflects isomorphisms, completing the cycle of equivalences.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Assume the equivalent conditions and that $T$ preserves finite coproducts. The free functor already reflects isomorphisms. By the dual [Crude monadicity theorem](../../../category-theory.md#crude-monadicity-theorem), it remains to preserve the relevant coreflexive equalizers.

A coreflexive equalizer diagram

$$
A\longrightarrow B\rightrightarrows C
$$

with $A\neq\varnothing$ can be equipped with the extra sections making it a split equalizer: choose a point of $A$ and use the common retraction to define the missing splitting maps on the complementary fibres. Every functor preserves split equalizers. If $A=\varnothing$, preservation follows from preservation of the initial object, which follows from preservation of finite coproducts. Consequently $F$ preserves all required coreflexive equalizers, and the adjunction is [comonadic](../../../category-theory.md#comonadic-adjunction).

## 5

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $(\mathcal V,\otimes,I)$ be a [symmetric monoidal category](../../../category-theory.md#symmetric-monoidal-category). A $\mathcal V$-[enriched category](../../../category-theory.md#enriched-category) has objects, hom-objects $\mathcal C(A,B)\in\mathcal V$, composition morphisms

$$
\mathcal C(B,C)\otimes\mathcal C(A,B)\to\mathcal C(A,C),
$$

and unit morphisms $I\to\mathcal C(A,A)$ satisfying the associative and unit diagrams. Its [underlying ordinary category](../../../category-theory.md#underlying-category-of-an-enriched-category) has hom-sets

$$
\mathcal V(I,\mathcal C(A,B)).
$$

If $\mathcal V$ is closed, take its internal hom $[A,B]$ as hom-object. Composition is the transpose of evaluation

$$
[B,C]\otimes[A,B]\otimes A\to[B,C]\otimes B\to C,
$$

and the unit is the transpose of $I\otimes A\cong A$. This is the [self-enrichment of a closed symmetric monoidal category](../../../category-theory.md#self-enrichment-of-a-closed-symmetric-monoidal-category).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For posets $A,B$, let $B^A$ be the poset of monotone maps $A\to B$ ordered pointwise. Evaluation

$$
B^A\times A\to B,\qquad(f,a)\mapsto f(a)
$$

is monotone. A monotone map $h:C\times A\to B$ curries to the monotone map

$$
\widehat h:C\to B^A,\qquad
\widehat h(c)(a)=h(c,a),
$$

and this correspondence is natural and invertible. Thus the [cartesian closed category of posets](../../../category.md#cartesian-closed-category-of-posets) has exponentials $B^A$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Identities are self-adjoint. If $f\dashv g$ and $f'\dashv g'$, then

$$
f'f\,gg'=f'(fg)g'\leq f'g'\leq1,
\qquad
1\leq gf\leq gg'f'f,
$$

with the second inequality written after inserting the two units in the appropriate order. Hence $f'f\dashv gg'$, so left adjoints form a subcategory.

In $\mathbf{Poset}$, these are exactly monotone maps possessing right adjoints, equivalently [lower adjoints](../../../category.md#galois-connection); when all joins exist, they are precisely the arbitrary-join-preserving maps.

In the inclusion-ordered [category of relations](../../../category.md#category-of-relations), a relation $R:A\rightsquigarrow B$ is left adjoint exactly when it is total and single-valued. It is therefore the graph of a function, and its right adjoint is $R^{\mathrm{op}}$. This is the [left adjoint relation is a function](../../../category-theory.md#left-adjoint-relation-is-a-function) criterion.

## 6

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [complex in an abelian category](../../../category-theory.md#complex-in-an-abelian-category) is a sequence $(A_n,d_n)$ with $d_nd_{n+1}=0$. A sequence is [exact](../../../category-theory.md#exact-sequence-in-an-abelian-category) when the image of every incoming map equals the kernel of the outgoing map.

The [Five lemma](../../../category-theory.md#five-lemma) says that in a morphism between exact five-term sequences, suitable epimorphism assumptions on the left and monomorphism assumptions on the right, together with isomorphisms in the four surrounding positions, force the middle map to be an isomorphism.

The [Snake lemma](../../../category-theory.md#snake-lemma) associates to a morphism of short exact sequences the exact sequence

$$
\boxed{\ker f'\to\ker f\to\ker f''
\xrightarrow{\partial}
\operatorname{coker}f'\to\operatorname{coker}f\to\operatorname{coker}f''.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Apply the [Snake lemma](../../../category-theory.md#snake-lemma) degree by degree to a short exact sequence of complexes

$$
0\to A_\bullet\to B_\bullet\to C_\bullet\to0.
$$

If $[c]\in H_n(C)$, lift a cycle $c$ to $b\in B_n$. Its boundary maps to zero in $C_{n-1}$, so it comes from a cycle $a\in A_{n-1}$; define $\partial[c]=[a]$. The Snake-lemma exactness and independence checks yield

$$
\cdots\to H_n(A)\to H_n(B)\to H_n(C)
\xrightarrow{\partial}H_{n-1}(A)\to H_{n-1}(B)\to\cdots.
$$

This is the algebraic [Mayer–Vietoris theorem](../../../algebraic-topology.md#mayer-vietoris-sequence) for homology objects.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The commutative diagram of short exact sequences of complexes induces a commutative diagram between the two long exact homology sequences from part (b). If any two vertical chain maps induce isomorphisms in every degree, then in each five-term window four of the five vertical homology maps are isomorphisms. The [Five lemma](../../../category-theory.md#five-lemma) makes the remaining map an isomorphism. Rotating the window handles each of the three possible missing columns, proving the two-out-of-three assertion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
