# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_25.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
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

## 1

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the covariant version of the [Yoneda embedding](../../../category.md#yoneda-embedding), put $Y(A)=\mathcal C(A,-)$. A [morphism](../../../algebra.md#morphism) $u:A\to B$ induces the [natural transformation](../../../category.md#natural-transformation) $Y(u):Y(B)\to Y(A)$ whose component sends $v:B\to X$ to $vu$. Thus $Y$ is a [functor](../../../category.md#functor) from the [opposite category](../../../category.md#opposite-category) $\mathcal C^{\mathrm{op}}$ to the [functor category](../../../category.md#functor-category) $[\mathcal C,\mathbf{Set}]$. The [locally small category](../../../category.md#locally-small-category) hypothesis makes each value a [set](../../../set.md).

The [Yoneda lemma](../../../category.md#yoneda-lemma) says that, for a [functor](../../../category.md#functor) $F:\mathcal C\to\mathbf{Set}$, evaluation at the [identity morphism](../../../algebra.md#identity-morphism) gives a [natural bijection](../../../category.md#natural-bijection)

$$
\boxed{\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),\qquad \theta\longmapsto\theta_A(1_A).}
$$

Given $a\in F(A)$, define $\theta^a_X(v)=F(v)(a)$. For $w:X\to X'$, the [functor](../../../category.md#functor) law gives $F(w)\theta^a_X(v)=F(wv)(a)=\theta^a_{X'}(wv)$, proving [naturality](../../../category.md#naturality). Conversely, [naturality](../../../category.md#naturality) of $\theta$ at $v:A\to X$ gives $\theta_X(v)=F(v)\theta_A(1_A)$. These two constructions are inverse, because $F(1_A)(a)=a$.

The [bijection](../../../function.md#bijection) is natural in both variables. A [natural transformation](../../../category.md#natural-transformation) $\beta:F\to H$ sends the element $a$ to $\beta_A(a)$, matching postcomposition by $\beta$. For $u:A\to B$, precomposing with $Y(u)$ sends $\theta$ to a transformation from $Y(B)$ and its distinguished element is $\theta_B(u)=F(u)(a)$. This is exactly the required dependence on $A$.

Taking $F=Y(B)$ gives $\operatorname{Nat}(Y(A),Y(B))\cong\mathcal C(B,A)$. Consequently **the covariant [Yoneda embedding](../../../category.md#yoneda-embedding) is [full and faithful](../../../category.md#full-and-faithful-functor)**, with the reversal of arrows accounted for by its [opposite category](../../../category.md#opposite-category) domain.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Suppose every component $\alpha_A$ is a [monomorphism](../../../category.md#monomorphism) in the [Category of sets](../../../category.md#category-of-sets), hence an [injective function](../../../algebra.md#injective-function). If $\beta,\gamma:H\to F$ are [natural transformations](../../../category.md#natural-transformation) with $\alpha\beta=\alpha\gamma$, then $\alpha_A\beta_A=\alpha_A\gamma_A$ at every object. Componentwise cancellation gives $\beta_A=\gamma_A$, so $\beta=\gamma$. Thus $\alpha$ is a [monomorphism](../../../category.md#monomorphism) in the [functor category](../../../category.md#functor-category).

Conversely, suppose $\alpha$ is a [monomorphism](../../../category.md#monomorphism) and $x,y\in F(A)$ satisfy $\alpha_A(x)=\alpha_A(y)$. The [Yoneda lemma](../../../category.md#yoneda-lemma) supplies [natural transformations](../../../category.md#natural-transformation) $\theta^x,\theta^y:Y(A)\to F$. Its [naturality](../../../category.md#naturality) in $F$ identifies $\alpha\theta^x$ and $\alpha\theta^y$ with the equal elements $\alpha_A(x)$ and $\alpha_A(y)$. Cancellation by $\alpha$ gives $\theta^x=\theta^y$; evaluating at $1_A$ gives $x=y$. Therefore **a [natural transformation](../../../category.md#natural-transformation) is a [monomorphism](../../../category.md#monomorphism) exactly when all its components are [injective functions](../../../algebra.md#injective-function)**. This is the [pointwise monomorphism in a set-valued functor category](../../../category.md#pointwise-monomorphism-in-a-set-valued-functor-category) criterion.

## 2

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $D:J\to\mathcal C$ be a finite [diagram in a category](../../../category.md#diagram-category-theory). Form the finite [products in a category](../../../category.md#product-category-theory)

$$
P=\prod_{j\in\operatorname{Ob}J}D(j),\qquad Q=\prod_{a:j\to k\ \text{in }J}D(k).
$$

Define $s,t:P\rightrightarrows Q$ by $\pi_a s=D(a)\pi_j$ and $\pi_a t=\pi_k$. Take their [equalizer](../../../category.md#equaliser) $e:L\to P$. The maps $\lambda_j=\pi_j e$ satisfy $D(a)\lambda_j=\lambda_k$, so they constitute a [categorical cone](../../../category.md#cone-over-a-diagram).

Any other [categorical cone](../../../category.md#cone-over-a-diagram) $x_j:X\to D(j)$ gives a unique $x:X\to P$ by the [product in a category](../../../category.md#product-category-theory) property. Its cone equations say $sx=tx$, so the [equalizer](../../../category.md#equaliser) gives a unique $\bar x:X\to L$ with $e\bar x=x$. The projections then give $\lambda_j\bar x=x_j$, and uniqueness follows from both universal properties. Thus **this [equalizer](../../../category.md#equaliser) of two product maps is the [finite limit](../../../category.md#finite-limit) of the [diagram in a category](../../../category.md#diagram-category-theory)**.

The empty indexing [category](../../../category.md) is included: its empty [product in a category](../../../category.md#product-category-theory) is a [terminal object](../../../category.md#terminal-object), which is the empty [categorical limit](../../../category.md#categorical-limit). Hence no nonemptiness restriction has entered the construction.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

With a [terminal object](../../../category.md#terminal-object) $1$, the [pullback in a category](../../../category.md#pullback-category-theory) of $A\to1\leftarrow B$ is the binary [product in a category](../../../category.md#product-category-theory) $A\times B$. Repetition gives all nonempty finite [products in a category](../../../category.md#product-category-theory), and $1$ supplies the empty one.

For $f,g:A\rightrightarrows B$, form the diagonal $\Delta_B:B\to B\times B$ and pull it back along $\langle f,g\rangle:A\to B\times B$. Write the resulting maps as $e:E\to A$ and $h:E\to B$. The equation $\langle f,g\rangle e=\Delta_B h$ says $fe=ge=h$. A map $x:X\to A$ with $fx=gx$ pairs with $fx:X\to B$ to give a unique map into this [pullback in a category](../../../category.md#pullback-category-theory). Thus $e$ is the [equalizer](../../../category.md#equaliser) of $f,g$.

We now have the finite [products in a category](../../../category.md#product-category-theory) and [equalizers](../../../category.md#equaliser) needed in part (a). **A [terminal object](../../../category.md#terminal-object) and [pullbacks in a category](../../../category.md#pullback-category-theory) therefore suffice for all [finite limits](../../../category.md#finite-limit).**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

An object of the [slice category](../../../category.md#slice-category) $\mathcal C/A$ is a [morphism](../../../algebra.md#morphism) $x:X\to A$; a map from $x$ to $y:Y\to A$ is $u:X\to Y$ with $yu=x$. The [identity morphism](../../../algebra.md#identity-morphism) $1_A:A\to A$ is a [terminal object](../../../category.md#terminal-object) of this [slice category](../../../category.md#slice-category), even when $\mathcal C$ itself has no [terminal object](../../../category.md#terminal-object).

For a cospan $X\xrightarrow{u}Z\xleftarrow{v}Y$ in the [slice category](../../../category.md#slice-category), form its underlying [pullback in a category](../../../category.md#pullback-category-theory) $P$ in $\mathcal C$, with maps $p:P\to X$ and $q:P\to Y$. If $x,y,z$ are the structure maps to $A$, then $xp=zup=zvq=yq$. This common map equips $P$ with its slice structure. An underlying mediating map into $P$ is automatically over $A$, because its composite with $xp$ is the prescribed structure map. Hence the same square is a [pullback in a category](../../../category.md#pullback-category-theory) in $\mathcal C/A$.

Part (b) applies to the slice's [terminal object](../../../category.md#terminal-object) and [pullbacks in a category](../../../category.md#pullback-category-theory). **Every [slice category](../../../category.md#slice-category) has all [finite limits](../../../category.md#finite-limit) when the ambient [category](../../../category.md) has [pullbacks in a category](../../../category.md#pullback-category-theory).** The [finite completeness of slice categories](../../../category.md#finite-completeness-of-slice-categories) result needs no ambient terminal-object hypothesis.

## 3

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [monomorphism](../../../category.md#monomorphism) $m:A\to B$ satisfies $mu=mv\Rightarrow u=v$ for every parallel pair into $A$. An [epimorphism](../../../category.md#epimorphism) $e:X\to Y$ satisfies $ue=ve\Rightarrow u=v$ for every parallel pair out of $Y$. A [strong monomorphism](../../../category.md#strong-monomorphism) is a [monomorphism](../../../category.md#monomorphism) with the following lifting property: whenever $e:X\to Y$ is an [epimorphism](../../../category.md#epimorphism) and $mu=ve$, with $u:X\to A$ and $v:Y\to B$, there is a unique $d:Y\to A$ with $de=u$ and $md=v$. A [regular monomorphism](../../../category.md#regular-monomorphism) is a [morphism](../../../algebra.md#morphism) occurring as the [equalizer](../../../category.md#equaliser) of two parallel maps. A [balanced category](../../../category.md#balanced-category) is one in which every [morphism](../../../algebra.md#morphism) that is both a [monomorphism](../../../category.md#monomorphism) and an [epimorphism](../../../category.md#epimorphism) is an [isomorphism](../../../algebra.md#isomorphism).

Suppose $m:A\to B$ equalizes $p,q:B\rightrightarrows D$. If $mu=mv$, the common composite has two factorizations through the [equalizer](../../../category.md#equaliser), so its uniqueness property gives $u=v$. Hence every [regular monomorphism](../../../category.md#regular-monomorphism) is indeed a [monomorphism](../../../category.md#monomorphism).

Now take the lifting square just described. The equations $pmu=qmu$ imply $pve=qve$. Cancel the [epimorphism](../../../category.md#epimorphism) $e$ to obtain $pv=qv$. The [equalizer](../../../category.md#equaliser) gives a unique $d$ with $md=v$. Since $mde=ve=mu$ and $m$ is a [monomorphism](../../../category.md#monomorphism), $de=u$. Thus **every [regular monomorphism](../../../category.md#regular-monomorphism) is a [strong monomorphism](../../../category.md#strong-monomorphism)**; the existence of the lift uses epic cancellation, and its uniqueness uses the equalizer property.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

If every [monomorphism](../../../category.md#monomorphism) is strong, let $m:A\to B$ be both a [monomorphism](../../../category.md#monomorphism) and an [epimorphism](../../../category.md#epimorphism). Use $m$ as both vertical maps in the lifting square, with horizontal maps $1_A$ and $1_B$. The [strong monomorphism](../../../category.md#strong-monomorphism) property gives $d:B\to A$ satisfying $dm=1_A$ and $md=1_B$. Thus $m$ is an [isomorphism](../../../algebra.md#isomorphism), proving that the [category](../../../category.md) is [balanced](../../../category.md#balanced-category).

For the converse, take $e:X\to Y$ epic, $m:A\to B$ monic, and $mu=ve$. Form the [pullback in a category](../../../category.md#pullback-category-theory) of $m$ along $v$:

$$
P=Y\times_B A,\qquad p:P\to Y,\quad q:P\to A,\quad mq=vp.
$$

The equality $mu=ve$ gives $t:X\to P$ with $pt=e$ and $qt=u$. By preservation of [monomorphisms](../../../category.md#monomorphism) under [pullback in a category](../../../category.md#pullback-category-theory), $p$ is monic. It is also epic: if $hp=kp$, then $he=hpt=kpt=ke$, and cancellation of $e$ gives $h=k$. The [balanced category](../../../category.md#balanced-category) hypothesis therefore makes $p$ an [isomorphism](../../../algebra.md#isomorphism).

Set $d=qp^{-1}$. Then $md=v$ and $de=qt=u$. Any other such lift agrees with $d$ after composing with the [monomorphism](../../../category.md#monomorphism) $m$, so it is equal to $d$. Consequently **in a [category](../../../category.md) with [pullbacks in a category](../../../category.md#pullback-category-theory), being [balanced](../../../category.md#balanced-category) is equivalent to every [monomorphism](../../../category.md#monomorphism) being a [strong monomorphism](../../../category.md#strong-monomorphism)**. This is the [balanced categories with pullbacks have strong monomorphisms](../../../category.md#balanced-categories-with-pullbacks-have-strong-monomorphisms) principle; the proof does not assume pullback stability of epimorphisms.

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The limit form of the [Special adjoint functor theorem](../../../category.md#special-adjoint-functor-theorem) is as follows. Let $\mathcal C$ be a [locally small category](../../../category.md#locally-small-category), a [complete category](../../../category.md#complete-category), and a [well-powered category](../../../category.md#well-powered-category), and suppose it has a [small cogenerating family](../../../category.md#cogenerating-set) $(Q_i)_{i\in I}$. Let $\mathcal D$ be a [locally small category](../../../category.md#locally-small-category). Then a [functor](../../../category.md#functor) $G:\mathcal C\to\mathcal D$ has a [left adjoint](../../../category.md#adjoint-functors) **if and only if it preserves all small [categorical limits](../../../category.md#categorical-limit)**. The dual exchanges completeness, well-poweredness and cogenerators for cocompleteness, well-copoweredness and generators, and characterizes [functors](../../../category.md#functor) with a [right adjoint](../../../category.md#adjoint-functors).

Here a [cogenerating set](../../../category.md#cogenerating-set) distinguishes unequal parallel maps by postcomposition into one of the $Q_i$. A [well-powered category](../../../category.md#well-powered-category) has a set of [subobjects](../../../category.md#subobject) of each fixed object. Completeness means existence of all small [categorical limits](../../../category.md#categorical-limit). We use the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set): a [complete category](../../../category.md#complete-category) that is [locally small](../../../category.md#locally-small-category) has an [initial object](../../../category.md#initial-object) exactly when it has a [weakly initial set](../../../category.md#weakly-initial-set). A proof is given in Question 5(c). We also use the fact that when $G$ preserves small [categorical limits](../../../category.md#categorical-limit), the [comma category](../../../category.md#comma-category) $(B\downarrow G)$ is complete, with its limits constructed in $\mathcal C$; local smallness is inherited from $\mathcal C$. Finally, having an [initial object](../../../category.md#initial-object) in $(B\downarrow G)$ for each $B$ is the [universal arrow from an object to a functor](../../../category.md#universal-arrow-from-an-object-to-a-functor) characterization of a [left adjoint](../../../category.md#adjoint-functors).

Assume $G$ preserves small [categorical limits](../../../category.md#categorical-limit), and fix $B\in\mathcal D$. We will construct a [weakly initial set](../../../category.md#weakly-initial-set) in $(B\downarrow G)$, rather than assume a solution set. Start with an arbitrary object $(C,x)$, where $x:B\to GC$. Call a [subobject](../../../category.md#subobject) $m:S\hookrightarrow C$ supporting if $x=G(m)x_S$ for some $x_S:B\to GS$. There is at least one, namely $1_C$. Because $G$ preserves [pullbacks in a category](../../../category.md#pullback-category-theory), it preserves [monomorphisms](../../../category.md#monomorphism): the self-pullback characterization of a monic map is preserved. Consequently each $x_S$ is unique.

There is a set of supporting [subobjects](../../../category.md#subobject) by well-poweredness. Their [intersection of subobjects](../../../category.md#intersection-of-subobjects) exists by completeness; write it $m_0:C_0\hookrightarrow C$. Applying $G$ to this intersection [categorical limit](../../../category.md#categorical-limit) gives a unique $x_0:B\to GC_0$ lifting all the $x_S$, and hence $x=G(m_0)x_0$. Minimality says that any [subobject](../../../category.md#subobject) $n:R\hookrightarrow C_0$ supporting $x_0$ is invertible: $m_0n$ supports $x$, so $m_0$ factors through $m_0n$, giving a right inverse to the monic $n$.

If $u,v:C_0\to Q_i$ satisfy $G(u)x_0=G(v)x_0$, their [equalizer](../../../category.md#equaliser) supports $x_0$, since $G$ preserves that [equalizer](../../../category.md#equaliser). It is therefore an [isomorphism](../../../algebra.md#isomorphism), and $u=v$. We have obtained an [injective function](../../../algebra.md#injective-function)

$$
\mathcal C(C_0,Q_i)\longrightarrow\mathcal D(B,GQ_i),\qquad u\longmapsto G(u)x_0.
$$

Let $J_i$ be its image, a subset of the fixed [set](../../../set.md) $S_i=\mathcal D(B,GQ_i)$. The [evaluation embedding into cogenerator products](../../../category.md#evaluation-embedding-into-cogenerator-products) is a [monomorphism](../../../category.md#monomorphism)

$$
C_0\hookrightarrow P_J:=\prod_{i\in I}\prod_{s\in J_i}Q_i.
$$

Indeed each $s\in J_i$ corresponds to a unique map $C_0\to Q_i$, and the [cogenerating set](../../../category.md#cogenerating-set) property makes the resulting family jointly monic. Notice that we use the realized subsets $J_i$, not all of $S_i$: there need not be a map $C_0\to Q_i$ available for an unused index.

There is a set of tuples $J=(J_i)$, since $I$ and every $S_i$ are sets. For each resulting $P_J$, choose representatives of its [subobjects](../../../category.md#subobject); these form a set by well-poweredness. For every representative $R$, include every map $y:B\to GR$, a set by local smallness of $\mathcal D$. All resulting pairs $(R,y)$ form a set. Our given $(C,x)$ receives a map from such a pair: transport $x_0$ along the [isomorphism](../../../algebra.md#isomorphism) between $C_0$ and the chosen representative, then compose its inverse with $m_0$. Thus these pairs form a [weakly initial set](../../../category.md#weakly-initial-set) in $(B\downarrow G)$. This is the [cogenerator bound for comma-category solution sets](../../../category.md#cogenerator-bound-for-comma-category-solution-sets).

The [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set) gives an [initial object](../../../category.md#initial-object) $(LB,\eta_B)$. For $h:B\to B'$, define $Lh$ by the unique equation

$$
G(Lh)\eta_B=\eta_{B'}h.
$$

Uniqueness proves the [functor](../../../category.md#functor) laws and gives the [natural bijections](../../../category.md#natural-bijection)

$$
\boxed{\mathcal C(LB,C)\cong\mathcal D(B,GC),\qquad f\longmapsto G(f)\eta_B.}
$$

Thus $L\dashv G$. Conversely, a [right adjoint](../../../category.md#adjoint-functors) preserves small [categorical limits](../../../category.md#categorical-limit): its adjunction identifies maps into the proposed limiting object with compatible families of maps into the diagram. This proves both directions of the [limit form of the special adjoint functor theorem](../../../category.md#limit-form-of-the-special-adjoint-functor-theorem). Applying the argument to the [opposite categories](../../../category.md#opposite-category) proves the dual statement. Choices of representatives and adjoint objects are understood in the usual ambient-universe convention for large [categories](../../../category.md).

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [comma category](../../../category.md#comma-category) $(X\downarrow G)$ has objects $(A,x)$ with $A\in\mathcal C$ and a [function](../../../function.md) $x:X\to G(A)$. Its [morphisms](../../../algebra.md#morphism) $(A,x)\to(B,y)$ are maps $f:A\to B$ in $\mathcal C$ satisfying $G(f)x=y$. The [identity morphism](../../../algebra.md#identity-morphism) and [composition in a category](../../../category.md#composition-in-a-category) are inherited from $\mathcal C$; the [functor](../../../category.md#functor) laws make the defining equations stable under both.

For a singleton $1$, its map $1\to G(A)$ is just an element $a\in G(A)$. Thus $(1\downarrow G)$ is the covariant [category of elements](../../../category.md#category-of-elements) of $G$, with arrows $f:(A,a)\to(B,b)$ satisfying $G(f)(a)=b$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Suppose $G$ is a [representable functor](../../../category.md#representable-functor), with a [natural isomorphism](../../../category.md#natural-isomorphism) $\theta:\mathcal C(R,-)\to G$. Put $r=\theta_R(1_R)$. For any $(A,a)$ in the [comma category](../../../category.md#comma-category) $(1\downarrow G)$, the representing [bijection](../../../function.md#bijection) gives a unique $f:R\to A$ with $\theta_A(f)=a$. By [naturality](../../../category.md#naturality), $\theta_A(f)=G(f)(r)$, exactly the condition for $f:(R,r)\to(A,a)$. Hence $(R,r)$ is an [initial object](../../../category.md#initial-object).

Conversely, if $(R,r)$ is an [initial object](../../../category.md#initial-object), then

$$
\boxed{\theta_A:\mathcal C(R,A)\longrightarrow G(A),\qquad f\longmapsto G(f)(r)}
$$

is a [bijection](../../../function.md#bijection) for each $A$: existence and uniqueness are precisely initiality applied to every $(A,a)$. For $h:A\to B$, $G(h)\theta_A(f)=G(hf)(r)=\theta_B(hf)$, proving [naturality](../../../category.md#naturality). Thus $r$ is a [universal element](../../../category.md#universal-element-of-a-set-valued-functor) and $\theta$ is a [representation of a functor](../../../category.md#representation-of-a-functor). **Being [representable](../../../category.md#representable-functor) is equivalent to the singleton [comma category](../../../category.md#comma-category) having an [initial object](../../../category.md#initial-object).**

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

A [weakly initial set](../../../category.md#weakly-initial-set) is a set of objects $(W_i)_{i\in I}$ such that every object receives at least one map from some $W_i$. An [initial object](../../../category.md#initial-object) is itself a singleton [weakly initial set](../../../category.md#weakly-initial-set). We prove the converse without replacing uniqueness by weak initiality.

Let $\mathcal E$ be a [complete category](../../../category.md#complete-category) that is [locally small](../../../category.md#locally-small-category). Form $W=\prod_i W_i$. For every object $A$, choose $W_i\to A$ and compose with the projection $W\to W_i$, so $W$ is weakly initial. Completeness supplies a [terminal object](../../../category.md#terminal-object), so the given [weakly initial set](../../../category.md#weakly-initial-set) cannot be empty.

The [endomorphisms](../../../algebra.md#endomorphism) of $W$ form a [set](../../../set.md). Take a simultaneous [equalizer](../../../category.md#equaliser) $e:I\to W$ of all of them with $1_W$; equivalently, equalize the two maps from $W$ into $\prod_{s\in\mathcal E(W,W)}W$ with components $s$ and $1_W$. Thus $se=e$ for every endomorphism $s$. The object $I$ is weakly initial, since $I\xrightarrow eW\to A$ exists for every $A$. Weak initiality of $W$ gives a map $u:W\to I$. Applying the equalizing identity to $eu$ yields $eue=e$, so monicity of $e$ gives $ue=1_I$.

For any [endomorphism](../../../algebra.md#endomorphism) $v:I\to I$, the map $evu$ is an [endomorphism](../../../algebra.md#endomorphism) of $W$. Therefore $evue=e$. Since $ue=1_I$, this becomes $ev=e$, giving $v=1_I$. Now let $f,g:I\rightrightarrows A$ and form their [equalizer](../../../category.md#equaliser) $j:E\to I$. Weak initiality of $I$ gives $h:I\to E$. The composite $jh$ is an [endomorphism](../../../algebra.md#endomorphism) of $I$, hence the identity. Consequently $f=fjh=gjh=g$.

There is at least one map from $I$ to every object, and the argument proves that there is at most one. **The object $I$ is an [initial object](../../../category.md#initial-object).** This establishes the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set) using only small [products in a category](../../../category.md#product-category-theory) and [equalizers](../../../category.md#equaliser).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

If $G$ is a [representable functor](../../../category.md#representable-functor), it preserves small [categorical limits](../../../category.md#categorical-limit). Part (b) makes $(1\downarrow G)$ have an [initial object](../../../category.md#initial-object), which gives a [weakly initial set](../../../category.md#weakly-initial-set).

Conversely, assume limit preservation and a [weakly initial set](../../../category.md#weakly-initial-set) in $(1\downarrow G)$. The needed comma-limit fact is explicit: for a small [diagram in a category](../../../category.md#diagram-category-theory) $(A_j,a_j)$, form $L=\lim_j A_j$ in $\mathcal C$. The elements $a_j\in G(A_j)$ form a compatible family, hence determine a unique $a\in G(L)$ under $G(L)\cong\lim_jG(A_j)$. The projections from $(L,a)$ are a [categorical limit](../../../category.md#categorical-limit) in the [comma category](../../../category.md#comma-category). This includes the empty diagram, since $G$ carries the [terminal object](../../../category.md#terminal-object) to a singleton. Each comma [hom-set](../../../category.md#hom-set) is a subset of a [hom-set](../../../category.md#hom-set) in $\mathcal C$, so the [comma category](../../../category.md#comma-category) is also [locally small](../../../category.md#locally-small-category).

Part (c) now gives an [initial object](../../../category.md#initial-object) of $(1\downarrow G)$, and part (b) supplies a [representation of a functor](../../../category.md#representation-of-a-functor). Therefore

$$
\boxed{G\text{ is representable}\iff G\text{ preserves small limits and }(1\downarrow G)\text{ has a weakly initial set}.}
$$

The size requirement is a genuine [solution-set condition](../../../category.md#solution-set-condition); limit preservation alone does not produce it in an arbitrary [complete category](../../../category.md#complete-category).

## 6

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [monad](../../../category-theory.md#monad) $\mathbb T=(T,\eta,\mu)$ consists of an [endofunctor](../../../category.md#endofunctor) $T:\mathcal C\to\mathcal C$ and [natural transformations](../../../category.md#natural-transformation) $\eta:1_{\mathcal C}\Rightarrow T$ and $\mu:T^2\Rightarrow T$ satisfying

$$
\mu_A\eta_{TA}=1_{TA}=\mu_A T\eta_A,\qquad \mu_A\mu_{TA}=\mu_A T\mu_A.
$$

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is $(A,a)$ with $a:TA\to A$ satisfying $a\eta_A=1_A$ and $a\mu_A=aT(a)$. A [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad) $h:(A,a)\to(B,b)$ obeys $ha=bT(h)$. The [functor](../../../category.md#functor) laws show that identities and composites obey this equation, giving the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^{\mathbb T}$.

For an [adjunction](../../../category.md#adjoint-functors) $F\dashv G$, let $\eta$ be its [adjunction unit](../../../category.md#unit-of-an-adjunction) and $\varepsilon$ its [adjunction counit](../../../category.md#counit-of-an-adjunction). The [monad induced by an adjunction](../../../category-theory.md#monad-induced-by-an-adjunction) is

$$
\boxed{T=GF,\qquad \eta:1\Rightarrow GF,\qquad \mu_A=G(\varepsilon_{FA}).}
$$

The two unit laws are $G\varepsilon_{FA}\eta_{GFA}=1_{GFA}$ and $G(\varepsilon_{FA}F\eta_A)=1_{GFA}$, respectively the two [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction).

For associativity, [naturality](../../../category.md#naturality) of the [adjunction counit](../../../category.md#counit-of-an-adjunction) at $\varepsilon_{FA}:FGFA\to FA$ says

$$
\varepsilon_{FA}\,\varepsilon_{FGFA}=\varepsilon_{FA}\,FG(\varepsilon_{FA}).
$$

Apply $G$ to obtain $\mu_A\mu_{TA}=\mu_AT\mu_A$. The composites defining $\eta$ and $\mu$ are [natural transformations](../../../category.md#natural-transformation), so all [monad](../../../category-theory.md#monad) axioms have been checked, not only their underlying objectwise types.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Define the [forgetful functor](../../../category.md#forgetful-functor) $G^{\mathbb T}(A,a)=A$, acting as the identity on underlying [morphisms](../../../algebra.md#morphism). Define the [free algebra functor](../../../category-theory.md#free-algebra-functor) by

$$
F^{\mathbb T}(X)=(TX,\mu_X),\qquad F^{\mathbb T}(h)=T(h).
$$

The [monad](../../../category-theory.md#monad) laws make $\mu_X$ an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) structure, and [naturality](../../../category.md#naturality) of $\mu$ makes $T(h)$ an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad).

For $(A,a)$, define the transpose maps

$$
\Phi(h)=h\eta_X,\qquad \Psi(k)=aT(k),\qquad
\Phi:\mathcal C^{\mathbb T}(F^{\mathbb T}X,(A,a))\longrightarrow\mathcal C(X,A).
$$

The map $\Psi(k)$ is an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad), because [naturality](../../../category.md#naturality) of $\mu$ and the algebra associativity law give

$$
aT(k)\mu_X=a\mu_A T^2(k)=aT(a)T^2(k)=aT(aT(k)).
$$

For $k:X\to A$, [naturality](../../../category.md#naturality) of $\eta$ gives $\Phi\Psi(k)=aT(k)\eta_X=a\eta_A k=k$. Conversely, if $h$ is an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad), then

$$
\Psi\Phi(h)=aT(h)T\eta_X=h\mu_X T\eta_X=h.
$$

Precomposing by a map into $X$ or postcomposing by an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) respects both formulas. Thus the [bijection](../../../function.md#bijection) is natural and **$F^{\mathbb T}\dashv G^{\mathbb T}$**. This is the [free-forgetful Eilenberg-Moore adjunction](../../../category-theory.md#free-forgetful-eilenberg-moore-adjunction).

Its [adjunction unit](../../../category.md#unit-of-an-adjunction) is the given $\eta_X$; its [adjunction counit](../../../category.md#counit-of-an-adjunction) at $(A,a)$ is the [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) $a:(TA,\mu_A)\to(A,a)$. Hence $G^{\mathbb T}F^{\mathbb T}=T$, and the induced multiplication is the underlying counit at $(TX,\mu_X)$, namely $\mu_X$. Therefore **this [adjunction](../../../category.md#adjoint-functors) induces exactly the original [monad](../../../category-theory.md#monad), including its [unit and multiplication of a monad](../../../category-theory.md#unit-and-multiplication-of-a-monad)**.

## 7

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

A [semi-additive category](../../../category-theory.md#semi-additive-category) has [commutative-monoid enrichment](../../../category-theory.md#commutative-monoid-enrichment): each [hom-set](../../../category.md#hom-set) is a [commutative monoid](../../../algebra.md#commutative-monoid), and [composition in a category](../../../category.md#composition-in-a-category) preserves addition and zero in each variable. In the finite-biproduct convention, which we use here, it also has finite [products in a category](../../../category.md#product-category-theory) and [coproducts in a category](../../../category.md#coproduct). A [preadditive category](../../../category.md#preadditive-category) has [abelian groups](../../../group.md#abelian-group) as its [hom-sets](../../../category.md#hom-set), with composition additive in each variable; this definition alone does not require finite [products in a category](../../../category.md#product-category-theory) or a [zero object](../../../category.md#zero-object).

Let $P=\prod_{i=1}^n A_i$ with projections $p_i$. Define $i_j:A_j\to P$ by $p_i i_j=1_{A_j}$ for $i=j$ and $p_i i_j=0$ otherwise. Bilinearity gives

$$
p_k\left(\sum_j i_jp_j\right)=p_k,
$$

so product uniqueness gives $\sum_j i_jp_j=1_P$. For a family $f_j:A_j\to X$, set $f=\sum_j f_jp_j$. Then $fi_j=f_j$. If $h:P\to X$ has the same restrictions, $h=h\sum_j i_jp_j=\sum_j f_jp_j=f$. Thus the [product in a category](../../../category.md#product-category-theory) is also the [coproduct in a category](../../../category.md#coproduct), with its canonical injections. Conversely, the analogous construction from a finite [coproduct in a category](../../../category.md#coproduct) gives projections and the same identities, proving that it is a [product in a category](../../../category.md#product-category-theory).

For the empty family, a [terminal object](../../../category.md#terminal-object) $T$ has a singleton endomorphism monoid, so $1_T=0$. Every map $T\to X$ equals its composite with $1_T=0$, hence equals the zero map; this map exists by enrichment. Therefore $T$ is also an [initial object](../../../category.md#initial-object), a [zero object](../../../category.md#zero-object). The dual argument applies to an [initial object](../../../category.md#initial-object). Consequently **finite [products in a category](../../../category.md#product-category-theory) and [coproducts in a category](../../../category.md#coproduct) coincide canonically as [biproducts](../../../category-theory.md#biproduct)**, including the nullary case.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Fix an object $C$. For $x:C\to B$, use $rx:C\to A$ as its identity arrow. For $a:C\to A$, its source is $fa$ and target is $ga$. If $ga=fb$, define the composite of $a$ followed by $b$ by

$$
\boxed{b\circ a=a+b-rga,\qquad a^{-1}=rfa+rga-a.}
$$

These expressions use addition and subtraction in the [hom-set](../../../category.md#hom-set) of the [preadditive category](../../../category.md#preadditive-category). The [reflexive pair](../../../category-theory.md#reflexive-pair) identities $fr=gr=1_B$ give

$$
f(b\circ a)=fa+fb-ga=fa,\qquad g(b\circ a)=ga+gb-ga=gb,
$$

so the composite has the required endpoints. Also $f(a^{-1})=ga$ and $g(a^{-1})=fa$.

The unit identities follow directly: $a\circ rfa=rfa+a-rfa=a$ and $rga\circ a=a+rga-rga=a$. If $ga=fb$ and $gb=fc$, either parenthesization of three arrows equals $a+b+c-rga-rgb$, so composition is associative. The inverse identities are

$$
a^{-1}\circ a=a+a^{-1}-rga=rfa,\qquad a\circ a^{-1}=a^{-1}+a-rfa=rga.
$$

Therefore these operations define a [groupoid](../../../category.md#groupoid) on the specified object and arrow [sets](../../../set.md). Precomposing by $k:C'\to C$ respects each expression, by additivity of composition, so the [groupoids](../../../category.md#groupoid) are natural in $C$.

**Every [reflexive pair](../../../category-theory.md#reflexive-pair) therefore has the required [groupoid](../../../category.md#groupoid) structure on generalized points.** This is the [reflexive-pair groupoid formula in a preadditive category](../../../category-theory.md#reflexive-pair-groupoid-formula-in-a-preadditive-category). If the composable-arrow [pullback in a category](../../../category.md#pullback-category-theory) $A\times_{g,B,f}A$ exists, its projections $p,q$ give the actual internal composition map $p+q-rgp$. The printed generalized-point definition does not assume that this pullback exists, and preadditivity alone would not ensure it.

## 8

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

Take any [morphism](../../../algebra.md#morphism) $h:A\to B$ and let $c:B\to C$ be its [categorical cokernel](../../../category.md#cokernel-in-a-category). Let $i:I\to B$ be the [categorical kernel](../../../category.md#kernel-in-a-category) of $c$. Since $ch=0$, kernel universality gives $e:A\to I$ with $h=ie$. The map $i$ is a [monomorphism](../../../category.md#monomorphism). We must establish the [pseudo-epimorphism](../../../category.md#pseudo-epimorphism) property of $e$, rather than merely name $I$ an image.

Suppose $t:I\to Z$ satisfies $te=0$. Let $k:K\to I$ be its [categorical kernel](../../../category.md#kernel-in-a-category). Then $e=ka$ for some $a:A\to K$. The composite $ik$ is a [monomorphism](../../../category.md#monomorphism), so the hypothesis that every [monomorphism](../../../category.md#monomorphism) is normal provides a map $q:B\to D$ of which $ik$ is a [categorical kernel](../../../category.md#kernel-in-a-category), up to its unique compatible isomorphism. Now $qh=qika=0$. The [categorical cokernel](../../../category.md#cokernel-in-a-category) property of $c$ gives $q=\bar q c$, and therefore $qi=\bar q ci=0$.

Since $ik$ is the [categorical kernel](../../../category.md#kernel-in-a-category) of $q$, the map $i$ factors through it: $i=ik\ell$ for some $\ell:I\to K$. Cancel the [monomorphism](../../../category.md#monomorphism) $i$ to get $k\ell=1_I$. As $k$ is also a [monomorphism](../../../category.md#monomorphism), $\ell k=1_K$, so $k$ is an [isomorphism](../../../algebra.md#isomorphism). Finally $t=tk\ell=0$, proving that $e$ is a [pseudo-epimorphism](../../../category.md#pseudo-epimorphism).

Thus

$$
\boxed{h=ie,\qquad i=\ker(\operatorname{coker}h),\qquad e\text{ pseudo-epic},\quad i\text{ monic}.}
$$

The [pseudo-epimorphism factorization through the kernel of a cokernel](../../../category.md#pseudo-epimorphism-factorization-through-the-kernel-of-a-cokernel) proof uses a [pointed category](../../../category.md#pointed-category), existence of [categorical kernels](../../../category.md#kernel-in-a-category) and [categorical cokernels](../../../category.md#cokernel-in-a-category), and normality of every monic map. It does not silently replace pseudo-epic cancellation against zero by the stronger [epimorphism](../../../category.md#epimorphism) condition.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

In an [abelian category](../../../category-theory.md#abelian-category), for $f:A\to B$ set $\operatorname{coim}f=\operatorname{coker}(\ker f)$ and $\operatorname{im}f=\ker(\operatorname{coker}f)$. The canonical map from coimage to image is an [isomorphism](../../../algebra.md#isomorphism). Thus the [image factorization in an abelian category](../../../category.md#image-factorization-in-an-abelian-category) is

$$
\boxed{A\xrightarrow{e}\operatorname{im}f\xrightarrow{m}B,\qquad f=me,\quad e\text{ epic},\quad m\text{ monic},}
$$

unique up to a unique compatible [isomorphism](../../../algebra.md#isomorphism).

The [short five lemma](../../../module-theory.md#short-five-lemma) states that in a commuting diagram of [short exact sequences](../../../module-theory.md#short-exact-sequence) $0\to L\to M\to R\to0$ and $0\to L'\to M'\to R'\to0$ in an [abelian category](../../../category-theory.md#abelian-category), if the vertical maps $L\to L'$ and $R\to R'$ are [isomorphisms](../../../algebra.md#isomorphism), then so is $M\to M'$.

For the [Five lemma](../../../category-theory.md#five-lemma), consider commuting exact rows

$$
A_1\xrightarrow{d_1}A_2\xrightarrow{d_2}A_3\xrightarrow{d_3}A_4\xrightarrow{d_4}A_5,
\qquad
B_1\xrightarrow{d'_1}B_2\xrightarrow{d'_2}B_3\xrightarrow{d'_3}B_4\xrightarrow{d'_4}B_5,
$$

with vertical maps $v_i:A_i\to B_i$. We prove the usual stronger version: $v_1$ epic, $v_2$ and $v_4$ invertible, and $v_5$ monic imply that $v_3$ is invertible. In particular the conclusion holds if all four outer vertical maps are [isomorphisms](../../../algebra.md#isomorphism).

Put $L=\operatorname{im}d_2$ and $R=\operatorname{im}d_3$, and define $L',R'$ similarly. Exactness gives [short exact sequences](../../../module-theory.md#short-exact-sequence)

$$
0\longrightarrow L\longrightarrow A_3\longrightarrow R\longrightarrow0,
\qquad
0\longrightarrow L'\longrightarrow B_3\longrightarrow R'\longrightarrow0.
$$

The [functoriality of abelian image factorization](../../../category.md#functoriality-of-abelian-image-factorization) supplies their vertical outer maps. We show that both are [isomorphisms](../../../algebra.md#isomorphism).

First, $L\cong\operatorname{coker}d_1$ and $L'\cong\operatorname{coker}d'_1$: exactness at $A_2$ identifies $\operatorname{im}d_1$ with $\ker d_2$, and the image-coimage [isomorphism](../../../algebra.md#isomorphism) for $d_2$ gives the claimed cokernel. Write $q:A_2\to L$ and $q':B_2\to L'$ for these [categorical cokernels](../../../category.md#cokernel-in-a-category). To construct an inverse to the induced map $\ell:L\to L'$, observe

$$
(qv_2^{-1}d'_1)v_1=qv_2^{-1}v_2d_1=0.
$$

Cancellation of the [epimorphism](../../../category.md#epimorphism) $v_1$ gives $qv_2^{-1}d'_1=0$, so $qv_2^{-1}$ factors uniquely as $\bar\ell q'$ with $\bar\ell:L'\to L$. From $\ell q=q'v_2$, composing with the epic $q,q'$ gives $\bar\ell\ell=1_L$ and $\ell\bar\ell=1_{L'}$.

Second, $R\cong\ker d_4$ and $R'\cong\ker d'_4$ by exactness at the fourth objects. Write their inclusions as $j:R\to A_4$ and $j':R'\to B_4$. The equality $d'_4v_4=v_5d_4$ gives the induced map $\rho:R\to R'$. Since

$$
v_5d_4v_4^{-1}j'=d'_4j'=0
$$

and $v_5$ is a [monomorphism](../../../category.md#monomorphism), $d_4v_4^{-1}j'=0$. Kernel universality gives $\bar\rho:R'\to R$ with $j\bar\rho=v_4^{-1}j'$. Cancelling the monic $j,j'$ proves $\bar\rho\rho=1_R$ and $\rho\bar\rho=1_{R'}$.

Apply the [short five lemma](../../../module-theory.md#short-five-lemma) to the two [short exact sequences](../../../module-theory.md#short-exact-sequence): their outer maps $\ell,\rho$ are invertible, so **$v_3$ is an [isomorphism](../../../algebra.md#isomorphism)**. This [five lemma via image factorization](../../../category-theory.md#five-lemma-via-image-factorization) argument uses only universal properties and therefore works in any [abelian category](../../../category-theory.md#abelian-category), without treating its objects as literal sets of elements.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
