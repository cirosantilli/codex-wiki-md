# Paper 23

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper23.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper23.pdf)

**Table of contents**

- [Section A](#section-a)
  - [1](#1)
    - [Solution](#1/solution)
  - [2](#2)
    - [Solution](#2/solution)
- [Section B](#section-b)
  - [3](#3)
    - [i](#3/i)
      - [Solution](#3/i/solution)
    - [ii](#3/ii)
      - [Solution](#3/ii/solution)
    - [iii](#3/iii)
      - [Solution](#3/iii/solution)
  - [4](#4)
    - [Solution](#4/solution)
  - [5](#5)
    - [Solution](#5/solution)
    - [i](#5/i)
      - [Solution](#5/i/solution)
    - [ii](#5/ii)
      - [Solution](#5/ii/solution)
    - [iii](#5/iii)
      - [Solution](#5/iii/solution)
    - [iv](#5/iv)
      - [Solution](#5/iv/solution)
  - [6](#6)
    - [Solution](#6/solution)

## Section A

↑ **Parent:** [Paper 23](paper-23.md)

### 1

↑ **Parent:** [Section A](#section-a)

<h4 id="1/solution">Solution</h4>

↑ **Parent:** [1](#1)

Use the [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem): a [functor](../../../category.md#functor) $U:\mathcal A\to\mathcal B$, with $\mathcal A$ [complete](../../../topological-analysis.md#completeness) and both categories [locally small](../../../category.md#locally-small-category), has a [left adjoint](../../../category.md#adjoint-functors) precisely when it preserves small [categorical limits](../../../category.md#categorical-limit) and satisfies the [solution-set condition](../../../category.md#solution-set-condition). The latter means that every [comma category](../../../category.md#comma-category) $(b\downarrow U)$ has a small [weakly initial set](../../../category.md#weakly-initial-set).

Here is the proof. First prove the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set). In a complete locally small [category](../../../category.md) $\mathcal E$, take the [product in a category](../../../category.md#product-category-theory) $W$ of a small weakly initial family. It is weakly initial: project to whichever member admits a [morphism](../../../algebra.md#morphism) into the required object. Form the simultaneous [equalizer](../../../category.md#equaliser) $i:I\to W$ of every [endomorphism](../../../algebra.md#endomorphism) of $W$ and $1_W$; local smallness makes this a small limit.

For parallel $f,g:I\to X$, let $j:Y\to I$ be their [equalizer](../../../category.md#equaliser). Weak initiality supplies $t:W\to Y$. Since $ijt$ is an endomorphism of $W$, the defining equalities give $ijti=i$. Cancel the [monomorphism](../../../category.md#monomorphism) $i$ to get $jti=1_I$. Thus $j$ is a split epimorphism as well as a monomorphism, hence invertible, and $f=g$. Existence of a [morphism](../../../algebra.md#morphism) $I\to X$ follows by composing $i$ with a map $W\to X$. Therefore $I$ is an [initial object](../../../category.md#initial-object).

Now, if $U$ preserves small [categorical limits](../../../category.md#categorical-limit), each $(b\downarrow U)$ has them: take the limit of the underlying $\mathcal A$-diagram and use preservation to assemble its maps out of $b$. It is locally small and has a weakly initial solution set, so the lemma produces an [initial object](../../../category.md#initial-object) $(Lb,\eta_b)$. Its [universal property](../../../category-theory.md#universal-property) gives natural [bijections](../../../function.md#bijection)

$$
\mathcal A(Lb,a)\cong\mathcal B(b,Ua).
$$

The universal arrows define $L$ on [morphisms](../../../algebra.md#morphism), proving $L\dashv U$. Conversely, a [right adjoint](../../../category.md#adjoint-functors) preserves [categorical limits](../../../category.md#categorical-limit), and its unit supplies a singleton solution set in each comma category.

Apply this to $U=F^*$. The [functor category](../../../category.md#functor-category) $[\mathcal D,\mathbf{Set}]$ is complete and locally small because $\mathcal D$ is small; [pointwise limits in a functor category](../../../category.md#pointwise-limits-in-a-functor-category) show $F^*$ preserves all small limits. For $Q:\mathcal C\to\mathbf{Set}$, verify the [bounded subfunctor solution set for precomposition](../../../category.md#bounded-subfunctor-solution-set-for-precomposition). Choose an infinite [cardinal number](../../../set-theory.md#cardinal-number) $\kappa$ at least as large as the number of $\mathcal D$-[morphisms](../../../algebra.md#morphism) and $\sum_{c\in\mathcal C}|Q(c)|$. Given $\eta:Q\to GF$, set

$$
G'(d)=\{G(u)\eta_c(x):c\in\mathcal C,\ x\in Q(c),\ u:Fc\to d\}.
$$

Postcomposition makes $G'$ a subfunctor, each value has cardinality at most $\kappa$, and $\eta$ factors through $G'F$. After labelling its values by subsets of $\kappa$, only a set of possibilities for $G'$ and $Q\to G'F$ exists. Their maps into $G$ give the required weakly initial set. Thus **$F^*$ has a left adjoint**.

It is the [left Kan extension](../../../category.md#left-kan-extension). The [left Kan extension as a comma-category colimit](../../../category.md#left-kan-extension-as-a-comma-category-colimit) makes it concrete:

$$
\boxed{(\operatorname{Lan}_FQ)(d)=\operatorname{colim}_{(c,u:Fc\to d)\in(F\downarrow d)}Q(c).}
$$

Every representative $(c,u,x)$ maps under $\eta:Q\to GF$ to $G(u)\eta_c(x)$. The colimit identifications and naturality make this well-defined, giving exactly $\operatorname{Nat}(\operatorname{Lan}_FQ,G)\cong\operatorname{Nat}(Q,GF)$.

### 2

↑ **Parent:** [Section A](#section-a)

<h4 id="2/solution">Solution</h4>

↑ **Parent:** [2](#2)

**Broadly in favour, if “trivial” means transparent once the correct structure has been identified.** The value of [category theory](../../../category-theory.md) is often to isolate a [universal property](../../../category-theory.md#universal-property) that makes a repeated argument automatic.

For example, two objects with the same universal property have unique connecting maps in each direction. Their composites and the identities satisfy the same defining conditions, so uniqueness makes those composites identities. This one argument explains the uniqueness of [categorical products](../../../category.md#product-category-theory), [categorical limits](../../../category.md#categorical-limit), [adjoint functors](../../../category.md#adjoint-functors) and many other constructions. It also specifies which isomorphism is canonical, a point that an arbitrary objectwise choice would miss.

The [Yoneda lemma](../../../category.md#yoneda-lemma) makes this perspective systematic. A [natural transformation](../../../category.md#natural-transformation) out of $\mathcal C(c,-)$ is determined by its value at $1_c$. Once that evaluation principle is recognized, questions about representable [functors](../../../category.md#functor) reduce to compositions in the original [category](../../../category.md). Similarly, the [Beck monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) organizes many free-and-forgetful constructions around [monad algebras](../../../category-theory.md#algebra-for-a-monad), reflection of [isomorphisms](../../../algebra.md#isomorphism) and specified [coequalizers](../../../category.md#coequalizer). The proof supplies a reusable explanation of why the algebraic structure can be reconstructed from the forgetful [functor](../../../category.md#functor).

The substantial work lies in finding suitable definitions and verifying their hypotheses. The [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem), for instance, needs completeness, local smallness and a solution set; none follows merely from calling a construction natural. The partial-operation tower below even has a [monadic length](../../../category-theory.md#monadic-length) that records how many distinct reconstruction steps are needed. These examples support the view that abstraction clarifies the source of an argument's simplicity. They also show why that simplicity is an achievement requiring proof.

## Section B

↑ **Parent:** [Paper 23](paper-23.md)

### 3

↑ **Parent:** [Section B](#section-b)

<h4 id="3/i">i</h4>

↑ **Parent:** [3](#3)

<h5 id="3/i/solution">Solution</h5>

↑ **Parent:** [I](#3/i)

We prove the [orthogonality of final functors and discrete fibrations](../../../category.md#orthogonality-of-final-functors-and-discrete-fibrations). For $b\in\mathcal B$, [finality](../../../category.md#finality-of-a-functor) supplies an object $(a,u:b\to Fa)$ of $(b\downarrow F)$. Lift $Ku:Kb\to GHa$ through the [discrete fibration](../../../category.md#discrete-fibration) $G$, obtaining

$$
j_{a,u}:c_{a,u}\longrightarrow Ha,\qquad Gj_{a,u}=Ku,\qquad Gc_{a,u}=Kb.
$$

If $v:(a,u)\to(a',u')$ in the [comma category](../../../category.md#comma-category), then $Fv\,u=u'$, and $Hv\,j_{a,u}$ is a lift of $Ku'$ with codomain $Ha'$. Uniqueness of that lift makes its domain equal to $c_{a',u'}$. Thus $c_{a,u}=c_{a',u'}$; since the comma category is a [connected category](../../../category.md#connected-category), equality propagates along every zigzag. Define $Lb$ to be this common object.

For $w:b\to b'$, choose $(a,u:b'\to Fa)$. Lift $Kw$ into $Lb'$, obtaining $\ell:c\to Lb'$. Then $j_{a,u}\ell$ lifts $K(uw)$ into $Ha$, so its domain is $Lb$ by the preceding construction. Define $Lw=\ell$. The [unique lifting property of a discrete fibration](../../../category.md#unique-lifting-property-of-a-discrete-fibration) proves $L(1_b)=1_{Lb}$ and $L(w'w)=L(w')L(w)$, and gives $GL=K$.

At $b=Fa$, use $(a,1_{Fa})$; its lift is $1_{Ha}$, so $LFa=Ha$. Both $L(Fv)$ and $Hv$ are lifts of $GHv$ with the same codomain, hence agree. Therefore $LF=H$.

If $L'$ is another filling [functor](../../../category.md#functor), its arrow $L'u:L'b\to Ha$ is the same unique lift of $Ku$, forcing $L'b=Lb$. Its arrows are likewise forced by their codomains and images under $G$. **The diagonal functor exists and is unique.**

<h4 id="3/ii">ii</h4>

↑ **Parent:** [3](#3)

<h5 id="3/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/ii)

Use the [connected-component presheaf of a functor](../../../category.md#connected-component-presheaf-of-a-functor). For $F:\mathcal C\to\mathcal D$, define $\mathcal E$ to have objects $(b,z)$, where $z$ is a [categorical connected component](../../../category.md#connected-component-of-a-category) of $(b\downarrow F)$. An arrow $(b,z)\to(b',z')$ is an arrow $u:b\to b'$ such that $u^*z'=z$, where precomposition induces $u^*:\pi_0(b'\downarrow F)\to\pi_0(b\downarrow F)$. Identity and composition follow from precomposition, so this is a [category](../../../category.md).

The projection $G:\mathcal E\to\mathcal D$ is a [discrete fibration](../../../category.md#discrete-fibration): the unique lift of $u:b\to b'$ with codomain $(b',z')$ has domain $(b,u^*z')$.

Define $J:\mathcal C\to\mathcal E$ by

$$
Ja=(Fa,[(a,1_{Fa})]),\qquad Jv=Fv.
$$

For $v:a\to a'$, the objects $(a,1_{Fa})$ and $(a',Fv)$ lie in the same component of $(Fa\downarrow F)$, proving this is well-defined. Clearly $GJ=F$.

For $(b,z)\in\mathcal E$, the objects and arrows of $((b,z)\downarrow J)$ are exactly the objects and arrows of the component $z$ of $(b\downarrow F)$. Indeed, an arrow $(b,z)\to Ja$ is $u:b\to Fa$ with $[(a,u)]=z$, and its commuting triangles are precisely those in the original comma category. This category is nonempty and connected. Hence $J$ is a [final functor](../../../category.md#final-functor), proving the [final-discrete-fibration factorization](../../../category.md#final-discrete-fibration-factorization)

$$
\boxed{\mathcal C\xrightarrow{J}\mathcal E\xrightarrow{G}\mathcal D.}
$$

<h4 id="3/iii">iii</h4>

↑ **Parent:** [3](#3)

<h5 id="3/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/iii)

Suppose $F=GJ=G'J'$ are two [final-discrete-fibration factorizations](../../../category.md#final-discrete-fibration-factorization). Apply the [orthogonality of final functors and discrete fibrations](../../../category.md#orthogonality-of-final-functors-and-discrete-fibrations) to the square with left side $J$, top $J'$, bottom $G$ and right side $G'$. It gives a unique $S:\mathcal E\to\mathcal E'$ satisfying $SJ=J'$ and $G'S=G$. Reversing the roles gives $T:\mathcal E'\to\mathcal E$.

Both $TS$ and $1_{\mathcal E}$ fill the same square for $J,G$, so uniqueness gives $TS=1_{\mathcal E}$; similarly $ST=1_{\mathcal E'}$. This proves the [uniqueness of a final-discrete-fibration factorization](../../../category.md#uniqueness-of-a-final-discrete-fibration-factorization): **the connecting functor is a canonical isomorphism**, not just a noncanonical equivalence.

### 4

↑ **Parent:** [Section B](#section-b)

<h4 id="4/solution">Solution</h4>

↑ **Parent:** [4](#4)

An [adjunction](../../../category.md#adjoint-functors) $L\dashv U$ induces the [monad](../../../category-theory.md#monad) $T=UL$ with unit $\eta$ and multiplication $U\varepsilon L$. The [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) sends $B$ to $(UB,U\varepsilon_B)$. A [monadic adjunction](../../../category-theory.md#monadic-adjunction) is one for which that comparison is an [equivalence of categories](../../../category.md#equivalence-of-categories). Iterating comparisons, when their [left adjoints](../../../category.md#adjoint-functors) exist, gives a tower; its [monadic length](../../../category-theory.md#monadic-length) is the number of steps until equivalence, with length zero for an equivalence and length one for a monadic adjunction that is not already an equivalence.

The [precise monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) says that a [right adjoint](../../../category.md#adjoint-functors) is monadic exactly when it reflects [isomorphisms](../../../algebra.md#isomorphism) and creates [coequalizers](../../../category.md#coequalizer) of pairs whose images admit [split coequalizers](../../../category.md#split-coequalizer).

Write $U_r:\mathcal C_r\to\mathcal C_{r-1}$ for one-step forgetting. For $r=1$, the [free extension of nested partial unary operations](../../../category.md#free-extension-of-nested-partial-unary-operations) is the familiar set $A\times\mathbb N$, with $\alpha_1(a,j)=(a,j+1)$ and unit $a\mapsto(a,0)$. A map into a set with endomorphism $\beta_1$ extends uniquely by $(a,j)\mapsto\beta_1^j f(a)$.

For $r\geq2$, let

$$
S(A)=\{a\in A:\alpha_{r-1}(a)\text{ is defined and equals }a\}.
$$

Keep $A$ and all its old operations, and adjoin the disjoint set $S(A)\times\mathbb N$. On the new points define $\alpha_1(a,j)=(a,j+1)$; every old operation $\alpha_i$ with $i\geq2$ is undefined there. Define the new top operation only at the old eligible points, by $\alpha_r(a)=(a,0)$ for $a\in S(A)$.

These domains satisfy the defining rules of the [nested partial unary operation category](../../../category.md#nested-partial-unary-operation-category): the new points have no $\alpha_1$-[fixed points](../../../function.md#fixed-point), so none has any higher operation defined. Given $f:A\to U_rB$, extend it by

$$
\overline f(a,j)=\beta_1^j\beta_r(f(a)).
$$

The expression is defined because $f$ sends eligible points to eligible points and $\beta_1$ is total. It preserves every defined operation; preservation of $\alpha_r$ at old points determines $j=0$, and preservation of $\alpha_1$ determines the whole chain. Thus it is the unique extension, proving $L_r\dashv U_r$.

<a id="4/image-the-free-new-operation-sends-each-eligible-point-to-a-new-value-with-a-free-chain-under-the-first-operation"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-23-free-extension.png)

**[Figure 1](#4/image-the-free-new-operation-sends-each-eligible-point-to-a-new-value-with-a-free-chain-under-the-first-operation). The free new operation sends each eligible point to a new value with a free chain under the first operation**.

For monadicity, $U_r$ reflects [isomorphisms](../../../algebra.md#isomorphism): an isomorphism of the lower structures takes $S(A)$ bijectively to $S(B)$, so the inverse of a map preserving the new operation preserves it too.

Next prove the [split-coequalizer lifting for a fixed-point-domain operation](../../../category.md#split-coequalizer-lifting-for-a-fixed-point-domain-operation). Let $f,g:A\rightrightarrows B$ be $\mathcal C_r$-morphisms and suppose their lower images have a split coequalizer $q:U_rB\to Q$, with $s:Q\to U_rB$, $t:U_rB\to U_rA$ satisfying

$$
qf=qg,\qquad qs=1,\qquad ft=1,\qquad gt=sq.
$$

Equip $Q$ with $\beta_Q(z)=q\beta_B(sz)$ on its required eligible domain. The lower-structure maps $s,t$ preserve eligibility. For eligible $x\in B$,

$$
q\beta_B(x)=qf\beta_A(tx)=qg\beta_A(tx)=q\beta_B(sqx),
$$

so $q$ preserves the top operation. If $h:B\to D$ coequalizes $f,g$, its lower factor $\overline h:Q\to U_rD$ satisfies

$$
\overline h\beta_Q(z)=h\beta_B(sz)=\beta_D(hsz)=\beta_D(\overline hz).
$$

Thus it is a morphism of the full structures. Uniqueness of the lifted operation follows from the eligible section $s$ and surjectivity of $q$. This creates the specified coequalizer, so the [Beck monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) proves **each one-step adjunction is monadic**.

Finally, every free top operation just constructed has no fixed points: for $r=1$ it shifts the free chain, while for $r\geq2$ it sends old eligible points to new distinct points and is undefined on the new points. Freely adjoining any further operation therefore changes nothing, since its required domain is empty. For $n>m$, the monad induced on $\mathcal C_m$ by the long free-and-forgetful adjunction is consequently the same monad, including unit and multiplication, as that for $\mathcal C_{m+1}\to\mathcal C_m$.

The first comparison category is thus equivalent to $\mathcal C_{m+1}$. Its algebra action evaluates the new formal value by $\alpha_{m+1}$, so the comparison from $\mathcal C_n$ retains precisely that next operation and is the remaining forgetful functor. Iteration recovers one additional operation at each step. These remaining comparisons are not equivalences while an operation is still forgotten: take a two-element set with all retained operations equal to the identity, and choose the next operation to be the identity in one extension and the transposition in another. Higher operations can be identities in the first case and undefined in the second. The identity on the retained structure is not a morphism between these extensions, so the forgetful functor is not full. This includes $\mathcal C_1\to\mathbf{Set}$.

The [monadic tower for nested partial unary operations](../../../category-theory.md#monadic-tower-for-nested-partial-unary-operations) therefore has exactly the claimed length:

$$
\boxed{\operatorname{length}(\mathcal C_n\rightleftarrows\mathbf{Set})=n.}
$$

### 5

↑ **Parent:** [Section B](#section-b)

<h4 id="5/solution">Solution</h4>

↑ **Parent:** [5](#5)

A [filtered category](../../../category.md#filtered-category) is nonempty, every pair of objects maps to a common object, and every parallel pair becomes equal after postcomposition. Equivalently every finite [diagram in a category](../../../category.md#diagram-category-theory) has a [cocone](../../../category.md#cocone-under-a-diagram).

For a filtered set diagram $D:I\to\mathbf{Set}$, the [finite-stage equality in a filtered set colimit](../../../category.md#finite-stage-equality-in-a-filtered-set-colimit) says that representatives $x\in D(i)$ and $y\in D(j)$ define the same element exactly when their images agree at some common stage. Indeed, equality in the ordinary disjoint-union-and-quotient construction is witnessed by a finite zigzag; filteredness moves its objects to a common stage and equalizes the finitely many competing arrows.

For a finite [categorical product](../../../category.md#product-category-theory), choose a common stage for all coordinate representatives to obtain surjectivity of the colimit-to-product comparison. Finitely many coordinate equalities can then be realized together at one later stage, proving injectivity. The empty product is preserved because a nonempty filtered category is connected. For an [equalizer](../../../category.md#equaliser), an element whose two images agree in the colimit reaches a stage where they agree, so it is represented by an element of the stagewise equalizer; the same equality criterion proves injectivity. Finite products and equalizers construct every [finite limit](../../../category.md#finite-limit). Hence [filtered colimits commute with finite limits in sets](../../../category.md#filtered-colimits-commute-with-finite-limits-in-sets).

We prove the equivalence by the cycle [solution](#5/i/solution), [solution](#5/ii/solution), [solution](#5/iii/solution), [solution](#5/iv/solution), then back to [solution](#5/i/solution).

<h4 id="5/i">i</h4>

↑ **Parent:** [5](#5)

<h5 id="5/i/solution">Solution</h5>

↑ **Parent:** [I](#5/i)

Assume $F$ preserves [finite limits](../../../category.md#finite-limit). Given any finite diagram in the [comma category](../../../category.md#comma-category) $(A\downarrow F)$, first take its underlying limit $c$ in $\mathcal C$. Its structure maps $A\to Fc_j$ form a cone, and preservation gives a unique map $A\to Fc$. This object and the underlying projections satisfy the limiting [universal property](../../../category-theory.md#universal-property) in the comma category. The construction also includes the empty diagram, since $F$ sends a [terminal object](../../../category.md#terminal-object) to a singleton. Thus $(A\downarrow F)$ has finite limits for every set $A$, proving (ii).

<h4 id="5/ii">ii</h4>

↑ **Parent:** [5](#5)

<h5 id="5/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/ii)

Take $A=1$. The [category of elements](../../../category.md#category-of-elements) $\int F=(1\downarrow F)$ has [finite limits](../../../category.md#finite-limit). Reversing its limiting cones gives [cocones](../../../category.md#cocone-under-a-diagram) over every finite diagram in $(\int F)^{\mathrm{op}}$; a terminal object before reversal ensures nonemptiness. Its [opposite category](../../../category.md#opposite-category) is therefore a [filtered category](../../../category.md#filtered-category), proving (iii).

<h4 id="5/iii">iii</h4>

↑ **Parent:** [5](#5)

<h5 id="5/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/iii)

Use the [covariant density presentation](../../../category.md#covariant-density-presentation). An object of $\int F$ is $(c,x)$ with $x\in Fc$; an arrow $(c,x)\to(d,y)$ is $u:c\to d$ with $F(u)x=y$. For each such object the [Yoneda lemma](../../../category.md#yoneda-lemma) gives a [natural transformation](../../../category.md#natural-transformation) $\mathcal C(c,-)\to F$. An arrow $u$ induces $\mathcal C(d,-)\to\mathcal C(c,-)$ by precomposition, so these transformations form a cocone indexed by $(\int F)^{\mathrm{op}}$.

At $a$, send a representative $(c,x,v:c\to a)$ to $F(v)x$. Every $z\in Fa$ comes from $(a,z,1_a)$. If two representatives have the same value $z$, their arrows to $(a,z)$ in $\int F$ identify both with that same representative in the opposite-indexed colimit. Thus the map is bijective and natural, proving

$$
\boxed{F\cong\operatorname{colim}_{(c,x)\in(\int F)^{\mathrm{op}}}\mathcal C(c,-).}
$$

The index is small because $\mathcal C$ is small and every $Fc$ is a set. By (iii) it is a [filtered category](../../../category.md#filtered-category). This proves (iv).

<h4 id="5/iv">iv</h4>

↑ **Parent:** [5](#5)

<h5 id="5/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/iv)

Every covariant [representable functor](../../../category.md#representable-functor) $\mathcal C(c,-)$ preserves [categorical limits](../../../category.md#categorical-limit), since a morphism out of $c$ into a limit is precisely a compatible cone. A filtered colimit of these functors is computed pointwise, and [filtered colimits commute with finite limits in sets](../../../category.md#filtered-colimits-commute-with-finite-limits-in-sets). Interchanging the finite limit and filtered colimit therefore proves that $F$ preserves finite limits, which is (i). This completes the cycle. It is also the [flat functor and finite-limit preservation](../../../category.md#flat-functor-and-finite-limit-preservation) criterion for a finitely complete small category.

### 6

↑ **Parent:** [Section B](#section-b)

<h4 id="6/solution">Solution</h4>

↑ **Parent:** [6](#6)

Work in ordinary set theory with the [axiom of choice](../../../set-theory.md#axiom-of-choice). A [regular category](../../../category.md#regular-category) has [finite limits](../../../category.md#finite-limit), image factorizations as [regular epimorphisms](../../../category.md#regular-epimorphism) followed by [monomorphisms](../../../category.md#monomorphism), and pullback-stable regular epimorphisms. A [regular functor](../../../category.md#regular-functor) preserves finite limits and regular epimorphisms.

A [capital regular category](../../../category.md#capital-regular-category) is one whose [well-supported objects](../../../category.md#well-supported-object) are [well-pointed objects in a category](../../../category.md#well-pointed-object-in-a-category). Here well-supported means $A\to1$ is a regular epimorphism; well-pointed means a subobject of $A$ containing every point $1\to A$ must be the whole object. This is the convention of [Definition 1.3](https://www2.math.ethz.ch/EMIS/journals/TAC/volumes/16/31/16-31.pdf). It permits objects of proper support with no points. Replacing this condition by global points detecting every isomorphism would change the assertion: a three-element chain is regular but cannot admit a conservative finite-limit-preserving functor to such a category.

Here is a regular-logic proof sketch of [capitalization of a small regular category](../../../category.md#capitalization-of-a-small-regular-category). Use a sort for every object of $\mathcal C$, a function symbol for every morphism, and [regular theory](../../../mathematical-logic.md#regular-theory) axioms for composition, finite limiting diagrams and regular-epimorphism lifting. Its set models are precisely regular functors $\mathcal C\to\mathbf{Set}$. Empty sorts must be allowed.

The key separation lemma is the [regular-logic separation of a proper subobject](../../../category.md#regular-logic-separation-of-a-proper-subobject). For $m:S\hookrightarrow A$ proper, the sequent

$$
\top\ \vdash_{x:A}\ \exists y:S\ (m(y)=x)
$$

is not derivable: interpreting a derivation in $\mathcal C$ would make the monomorphism $m$ a regular epimorphism, hence an isomorphism. The [chase completeness for regular logic](../../../mathematical-logic.md#chase-completeness-for-regular-logic) supplies a set model in which it fails. Briefly, start with a named antecedent element, adjoin witnesses for the existential axioms, and quotient by required equalities. Every consequent about the original parameter arising at a finite stage has a finite proof; thus a nonderivable consequent remains false. The filtered union is the desired model. This witness construction, rather than an assumption that every sort is inhabited, is what keeps proper supports distinguishable.

Since $\mathcal C$ is small, choose a set-indexed family $(M_i)_{i\in I}$ of regular functors, one detecting each proper monomorphism, and form

$$
P:\mathcal C\longrightarrow\mathbf{Set}^{I},\qquad
P(A)=(M_iA)_{i\in I}.
$$

It is regular by coordinatewise finite limits and surjections. It reflects invertibility of monomorphisms. If $P(f)$ is invertible, apply this fact to the image inclusion of $f$ and to the diagonal of its [kernel pair](../../../category.md#kernel-pair). They are invertible, so $f$ is both a regular epimorphism and a monomorphism, hence invertible. Thus $P$ is a [conservative functor](../../../category.md#conservative-functor).

The target is a [power of sets as a capital regular category](../../../category.md#power-of-sets-as-a-capital-regular-category). A well-supported family has every coordinate nonempty, and choice extends any coordinate element to a global tuple. A subobject containing every tuple must consequently contain every coordinate element. Therefore it is capital, giving the required isomorphism-reflecting regular functor. This is the separation aspect of the regular representation results originating in [Barr's embedding work](https://math.mcgill.ca/barr/papers/embed.pdf); full faithfulness is unnecessary here.

The stronger target of a single set category has a precise restriction: **$\mathcal C$ admits a conservative regular functor to the [Category of sets](../../../category.md#category-of-sets) exactly when it is an [almost totally supported regular category](../../../category.md#almost-total-support-for-a-regular-category).** This means every object is well-supported or a [strict initial object](../../../category.md#strict-initial-object). Here are necessity and sufficiency.

Suppose $V:\mathcal C\to\mathbf{Set}$ is regular and conservative. If $VA$ is nonempty, its support in sets is $1$. Since $V$ preserves images, it sends the support inclusion $\sigma(A)\hookrightarrow1$ to an isomorphism; conservativity makes $\sigma(A)=1$, so $A$ is well-supported.

If $VA$ is empty, every projection $A\times X\to A$ is sent to the unique bijection between empty sets, hence is invertible. This supplies a morphism $A\to X$ for every $X$. The equalizer of any two such morphisms is also sent to a bijection, hence is invertible, proving uniqueness. Thus $A$ is initial. Every arrow $Y\to A$ forces $VY$ to be empty and is then sent to a bijection; conservativity makes it invertible. So $A$ is strict initial.

Conversely suppose this support condition holds. Use $P$ above and take

$$
V(A)=\prod_{i\in I}M_i(A).
$$

Products preserve finite limits and, by choice, coordinatewise surjections, so $V$ is regular. A well-supported object has all coordinates nonempty. A proper strict initial object has a subterminal image in every coordinate, with at least one empty coordinate: otherwise its arrow to $1$ would be sent by $P$ to an isomorphism, contradicting conservativity.

If $Vf$ is a bijection between well-supported objects, the [conservativity of set products on totally supported families](../../../category.md#conservativity-of-set-products-on-totally-supported-families) makes each $M_i(f)$ bijective: a missing coordinate preimage or a pair of equal-image coordinate elements extends to a tuple witnessing failure of surjectivity or injectivity. Hence $P(f)$ is invertible and so is $f$. An arrow between strict initial objects is already invertible; an arrow from a strict initial object to a well-supported object cannot become a bijection between empty and nonempty sets. An arrow into a strict initial object is invertible by definition. These cases prove conservativity and the [conservative regular representation in sets](../../../category.md#conservative-regular-representation-in-sets) criterion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
