# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_20.pdf)

**Table of contents**

- [Section A](#section-a)
  - [1](#1)
    - [i](#1/i)
      - [Solution](#1/i/solution)
    - [ii](#1/ii)
      - [Solution](#1/ii/solution)
    - [iii](#1/iii)
      - [Solution](#1/iii/solution)
  - [2](#2)
    - [Solution](#2/solution)
  - [3](#3)
    - [Solution](#3/solution)
- [Section B](#section-b)
  - [4](#4)
    - [i](#4/i)
      - [Solution](#4/i/solution)
    - [ii](#4/ii)
      - [Solution](#4/ii/solution)
    - [iii](#4/iii)
      - [Solution](#4/iii/solution)
    - [iv](#4/iv)
      - [Solution](#4/iv/solution)
  - [5](#5)
    - [Solution](#5/solution)
  - [6](#6)
    - [i](#6/i)
      - [Solution](#6/i/solution)
    - [ii](#6/ii)
      - [Solution](#6/ii/solution)
    - [iii](#6/iii)
      - [Solution](#6/iii/solution)

## Section A

↑ **Parent:** [Paper 20](paper-20.md)

### 1

↑ **Parent:** [Section A](#section-a)

<h4 id="1/i">i</h4>

↑ **Parent:** [1](#1)

<h5 id="1/i/solution">Solution</h5>

↑ **Parent:** [I](#1/i)

Write the [comonad](../../../category.md#comonad) as $(G,\epsilon,\delta)$ and its [category of coalgebras for a comonad](../../../category.md#category-of-coalgebras-for-a-comonad) as $\mathcal E^G$. A [coalgebra for a comonad](../../../category.md#coalgebra-for-a-comonad) is a map $a:A\to GA$ with $\epsilon_Aa=1_A$ and $\delta_Aa=Ga\,a$. A morphism $f:(A,a)\to(B,b)$ satisfies $bf=Gf\,a$. Let $U:\mathcal E^G\to\mathcal E$ be the [forgetful functor](../../../category.md#forgetful-functor) and let $R(X)=(GX,\delta_X)$ be the [cofree coalgebra](../../../category.md#cofree-coalgebra). The [adjunction](../../../category.md#adjoint-functors) $U\dashv R$ has the explicit correspondence

$$
f:UA\to X\quad\longleftrightarrow\quad Gf\,a:A\to R(X).
$$

We construct the three pieces of the [elementary topos](../../../category-theory.md#elementary-topos) structure.

Because $G$ preserves [finite limits](../../../category.md#finite-limit), each underlying finite limiting cone has a unique coalgebra structure induced by the structures on its vertices. The counit and coassociativity equations can be checked after its jointly monic projections. Thus $U$ creates [finite limits](../../../category.md#finite-limit) and reflects isomorphisms. A morphism of coalgebras is monic exactly when its underlying morphism is monic, by the diagonal criterion using the created [pullback](../../../category.md#pullback-category-theory).

For [exponentials in a coalgebra topos](../../../category.md#exponentials-in-a-coalgebra-topos), fix coalgebras $(A,a)$ and $(B,b)$ and put $E=B^A$ in $\mathcal E$. On the cofree coalgebra $R(E)$ there is an underlying evaluation

$$
e:GE\times A\longrightarrow B,\qquad e=\operatorname{ev}(\epsilon_E\times1_A).
$$

The two maps

$$
b e,\qquad Ge\,(\delta_E\times a):GE\times A\longrightarrow GB
$$

use $G(GE\times A)\cong GGE\times GA$ in the second expression. Transpose them in $\mathcal E$ to maps $r,s:GE\rightrightarrows(GB)^A$, and then transpose across $U\dashv R$ to coalgebra morphisms $\widetilde r,\widetilde s:R(E)\rightrightarrows R((GB)^A)$. Take their [equalizer](../../../category.md#equaliser) $C$ in $\mathcal E^G$.

An underlying map $UX\times A\to B$ corresponds to a coalgebra map $h:X\to R(E)$. The equation saying that the original map is a coalgebra morphism is precisely $rh=sh$, since $\delta_Eh=Gh\,x$ for the structure $x:X\to GX$. By the cofree adjunction, this is equivalent to $\widetilde rh=\widetilde sh$, hence to unique factorization through $C$. Therefore

$$
\mathcal E^G(X,C)\cong\mathcal E^G(X\times A,B),
$$

naturally in $X$. This constructs the required [exponential object](../../../category.md#exponential-object).

For the [subobject classifier of a coalgebra topos](../../../category.md#subobject-classifier-of-a-coalgebra-topos), let $\top:1\hookrightarrow\Omega$ be the underlying [subobject classifier](../../../category-theory.md#subobject-classifier), and let $\kappa:G\Omega\to\Omega$ classify the mono $G\top:G1\cong1\hookrightarrow G\Omega$. Its cofree transpose is the coalgebra endomorphism

$$
k=G\kappa\,\delta_\Omega:R\Omega\longrightarrow R\Omega.
$$

Define $\Omega_G$ as the [equalizer](../../../category.md#equaliser) of $k$ and $1_{R\Omega}$. The transpose of $\top$ factors through this [equalizer](../../../category.md#equaliser) and gives $\top_G:1\to\Omega_G$.

Indeed, for a [subobject](../../../category.md#subobject) $S\hookrightarrow UX$ classified by $\chi:UX\to\Omega$, the [pullback](../../../category.md#pullback-category-theory) $x^{-1}(GS)$ has characteristic map $\kappa G\chi\,x$. It is always contained in $S$, by naturality of the counit. Equality holds exactly when $x$ restricts to a coalgebra structure on $S$; its axioms then follow by composing with the [monomorphisms](../../../category.md#monomorphism) $GS\hookrightarrow GX$ and $GGS\hookrightarrow GGX$. Under $U\dashv R$, the classifying map becomes $h=G\chi\,x:X\to R\Omega$. The equality of [subobjects](../../../category.md#subobject) is $\epsilon_\Omega h=\kappa h$. Transposing this equality gives $h=kh$, so exactly the coalgebra [subobjects](../../../category.md#subobject) correspond to maps $X\to\Omega_G$. Their [pullback](../../../category.md#pullback-category-theory) of $\top_G$ is the desired subcoalgebra, and uniqueness follows from uniqueness of $\chi$.

Thus we have [finite limits](../../../category.md#finite-limit), exponentials and a [subobject classifier](../../../category-theory.md#subobject-classifier):

$$
\boxed{\mathcal E^G\text{ is an elementary topos}.}
$$

The construction does not assume that $G$ preserves the underlying exponentials or underlying [subobject classifier](../../../category-theory.md#subobject-classifier).

<h4 id="1/ii">ii</h4>

↑ **Parent:** [1](#1)

<h5 id="1/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/ii)

A [decidable object in a topos](../../../category-theory.md#decidable-object-in-a-topos) has a decomposition $A\times A=\Delta_A\amalg D_A$, with $D_A$ representing inequality. In the [internal logic of a topos](../../../category-theory.md#internal-logic-of-a-topos), equality on $A$ is decidable. These categorical complements behave well under [pullback](../../../category.md#pullback-category-theory).

For a [subobject](../../../category.md#subobject) $B\hookrightarrow A$, pull back the displayed decomposition along $B\times B\hookrightarrow A\times A$. The diagonal pulls back to $\Delta_B$, while $D_A$ pulls back to its complement. Hence **every [subobject](../../../category.md#subobject) of a decidable object is decidable**; the [subobject](../../../category.md#subobject) itself need not be complemented in $A$.

For two decidable objects, the diagonals of $A$ and $B$ give four disjoint summands of $(A\times B)^2$, according as each coordinate pair is equal or unequal. The both-equal summand is $\Delta_{A\times B}$, and the other three give its complement. The [terminal object](../../../category.md#terminal-object) is decidable, so induction gives **closure under finite products**, including the empty product.

For a family $(A_i)_{i\in I}$ of decidable objects with an existing [coproduct](../../../category.md#coproduct) $A=\coprod_iA_i$, products distribute over this [coproduct](../../../category.md#coproduct), giving

$$
A\times A\cong\coprod_{i,j\in I}(A_i\times A_j).
$$

The [coproduct](../../../category.md#coproduct) injections in a topos are disjoint. The diagonal consists of $\Delta_{A_i}$ in each $i=j$ summand, and has complement

$$
\boxed{\left(\coprod_iD_{A_i}\right)\amalg\left(\coprod_{i\ne j}A_i\times A_j\right).}
$$

Consequently **every existing [coproduct](../../../category.md#coproduct) of decidable objects is decidable**, including the [initial object](../../../category.md#initial-object). In a [Grothendieck topos](../../../category-theory.md#grothendieck-topos) all small [coproducts](../../../category.md#coproduct) exist. No assertion that arbitrary products preserve decidability is used.

<h4 id="1/iii">iii</h4>

↑ **Parent:** [1](#1)

<h5 id="1/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/iii)

Let $\mathcal Q$ be the full subcategory of [quotients of decidable objects](../../../category-theory.md#quotients-of-decidable-objects). It is closed under quotients, by composition of [epimorphisms](../../../category.md#epimorphism), and under small [coproducts](../../../category.md#coproduct), by part (ii). It is also closed under [subobjects](../../../category.md#subobject): pull back a decidable cover $D\twoheadrightarrow B$ along $B'\hookrightarrow B$. The resulting cover of $B'$ has domain a [subobject](../../../category.md#subobject) of $D$, hence a decidable object.

The [terminal object](../../../category.md#terminal-object) lies in $\mathcal Q$. If $D\twoheadrightarrow B$ and $D'\twoheadrightarrow C$ are decidable covers, their product is an [epimorphism](../../../category.md#epimorphism) $D\times D'\twoheadrightarrow B\times C$. Part (ii) makes its domain decidable. Thus products, and then [equalizers](../../../category.md#equaliser) as [subobjects](../../../category.md#subobject) of products, remain in $\mathcal Q$. The inclusion $I:\mathcal Q\hookrightarrow\mathcal E$ preserves [finite limits](../../../category.md#finite-limit).

We construct a [coreflective subcategory](../../../category.md#coreflective-subcategory) rather than claim that every object has a decidable cover. For $X\in\mathcal E$, let $qX\hookrightarrow X$ be the union of all [subobjects](../../../category.md#subobject) of $X$ which lie in $\mathcal Q$. The [Grothendieck topos](../../../category-theory.md#grothendieck-topos) is well-powered, so these [subobjects](../../../category.md#subobject) form a set. Choose a decidable cover of each and take their [coproduct](../../../category.md#coproduct). Its map to $X$ has image $qX$, so $qX$ is itself a quotient of a decidable object. Any map from an object of $\mathcal Q$ to $X$ has image in $\mathcal Q$, and therefore factors uniquely through $qX$. This gives

$$
I\dashv q,\qquad \mathcal E(IB,X)\cong\mathcal Q(B,qX).
$$

The induced [idempotent comonad](../../../category.md#idempotent-comonad) $G=Iq$ on $\mathcal E$ preserves [finite limits](../../../category.md#finite-limit): $q$ is a [right adjoint](../../../category.md#adjoint-functors) and $I$ preserves those limits. Its counit is the inclusion $qX\hookrightarrow X$, and $q(qX)=qX$.

The coalgebras of this comonad are exactly the objects of $\mathcal Q$. A coalgebra structure is a section $X\to qX$ of the monic counit, forcing the counit to be an isomorphism; conversely an object already in $\mathcal Q$ has the unique such structure. Thus $\mathcal Q\simeq\mathcal E^G$. Part (i) now gives

$$
\boxed{\mathcal E_{qd}\text{ is a topos}.}
$$

This argument proves the required elementary-topos conclusion without presuming a small family of decidable generators for $\mathcal E$.

### 2

↑ **Parent:** [Section A](#section-a)

<h4 id="2/solution">Solution</h4>

↑ **Parent:** [2](#2)

A [local operator](../../../category-theory.md#lawvere-tierney-topology), also called a [Lawvere-Tierney topology](../../../category-theory.md#lawvere-tierney-topology), is a map $j:\Omega\to\Omega$ which internally satisfies

$$
p\leq jp,\quad j\top=\top,\quad j(p\wedge q)=jp\wedge jq,\quad jjp=jp.
$$

The [closure operation of a local operator](../../../category-theory.md#closure-operation-of-a-local-operator) sends a mono with characteristic map $\chi$ to the [subobject](../../../category.md#subobject) classified by $j\chi$. It is inflationary, idempotent and [pullback](../../../category.md#pullback-category-theory)-stable. A mono is [j-dense](../../../category-theory.md#j-dense-monomorphism) if its closure is its whole codomain, and [j-closed](../../../category-theory.md#j-closed-monomorphism) if it equals its closure. A [j-sheaf](../../../category-theory.md#j-sheaf) $S$ is an object for which restriction

$$
\mathcal E(B,S)\longrightarrow\mathcal E(A,S)
$$

is a bijection for every j-dense mono $A\hookrightarrow B$; requiring only injectivity defines a [j-separated object](../../../category-theory.md#j-separated-object).

Here is a construction underlying the [sheaf reflector for a local operator](../../../category-theory.md#sheaf-reflector-for-a-local-operator). The [closed-subobject classifier](../../../category-theory.md#closed-subobject-classifier) $\Omega_j=\{p:jp=p\}$ is a j-sheaf: closed [subobjects](../../../category.md#subobject) on a dense [subobject](../../../category.md#subobject) extend uniquely by taking their closure in the larger object. Powers $\Omega_j^X$ are also sheaves, because products of a dense mono with $X$ remain dense. A j-closed [subobject](../../../category.md#subobject) of a sheaf is a sheaf: first extend a map into the ambient sheaf, then use density to force its image into the closed [subobject](../../../category.md#subobject).

Close the diagonal of $X$. Its j-closure is an equivalence relation, using preservation of finite meets and [pullback](../../../category.md#pullback-category-theory)-stability to verify transitivity. The effective quotient $X\twoheadrightarrow X_s$ is the separated reflection: every map from $X$ into a separated object identifies that closed diagonal and factors uniquely. For separated $X_s$, the closed-singleton map

$$
X_s\longrightarrow\Omega_j^{X_s},\qquad x\longmapsto\bigl(z\longmapsto j(z=x)\bigr)
$$

is monic. Its j-closed image closure $a_jX$ is a sheaf, and $X_s\hookrightarrow a_jX$ is dense. Unique extension across that mono, following the separated quotient factorization, proves

$$
\mathcal E(X,S)\cong\mathbf{sh}_j(\mathcal E)(a_jX,S)
$$

for every sheaf $S$. This proves reflectivity. The closure construction is [pullback](../../../category.md#pullback-category-theory)-stable; equivalently, separated quotients and the subsequent dense embeddings commute with the finite limiting comparisons, giving the usual left-exact sheaf reflector.

[Finite limits](../../../category.md#finite-limit) of sheaves are computed in $\mathcal E$, because unique extensions can be taken componentwise. If $S$ is a sheaf, $S^T$ is a sheaf for any $T$, by the same product-with-dense-mono argument. Thus sheaf exponentials are the ambient exponentials. Monos between sheaves have j-closed images: their closure is a sheaf, and the dense inclusion into it splits by the extension property, hence is an isomorphism. Therefore $\Omega_j$ classifies precisely their [subobjects](../../../category.md#subobject). These observations establish **$\mathbf{sh}_j(\mathcal E)$ is a reflective topos**.

Now let $u:1\to\Omega$ classify the given [subterminal object](../../../category.md#subterminal-object). Its [open local operator](../../../category-theory.md#open-local-operator) and [closed local operator](../../../category-theory.md#closed-local-operator) are

$$
\boxed{o(U)(p)=(u\Rightarrow p),\qquad c(U)(p)=u\vee p.}
$$

The [Heyting algebra](../../../mathematical-logic.md#heyting-algebra) identities verify all local-operator axioms: implication by fixed $u$ preserves meets and is idempotent, while adjoining $u$ preserves meets by distributivity and is idempotent.

For a mono in $B$ with characteristic predicate $p$, closedness for $c(U)$ means $u\vee p=p$, or $u\leq p$. Density for $o(U)$ means $(u\Rightarrow p)=\top$, again $u\leq p$. Thus **the c(U)-closed monos are exactly the o(U)-dense monos**.

Both densities together force $u\leq p$ and $u\vee p=\top$, hence $p=\top$: the only jointly dense monos are isomorphisms. More explicitly, the meet of these operators is pointwise and

$$
(u\Rightarrow p)\wedge(u\vee p)=p,
$$

so $o(U)\wedge c(U)=\mathrm{id}_\Omega$.

For their join, every mono $A\hookrightarrow B$ factors through the union with the [pullback](../../../category.md#pullback-category-theory) $U_B=U\times B$:

$$
A\hookrightarrow A\cup U_B\hookrightarrow B.
$$

The first mono is c(U)-dense, because adjoining $U$ fills its codomain; the second is o(U)-dense, because its image contains $U_B$. Any [local operator](../../../category-theory.md#lawvere-tierney-topology) above both must therefore make every mono dense, since its dense monos are closed under composition. It is the largest operator $p\mapsto\top$. Consequently

$$
\boxed{o(U)\wedge c(U)=\mathrm{id}_\Omega,\qquad o(U)\vee c(U)=\top.}
$$

These are the [complementary open and closed local operators](../../../category-theory.md#complementary-open-and-closed-local-operators) in the ordered lattice of [local operators](../../../category-theory.md#lawvere-tierney-topology), with order given by pointwise implication.

### 3

↑ **Parent:** [Section A](#section-a)

<h4 id="3/solution">Solution</h4>

↑ **Parent:** [3](#3)

A [first-order signature](../../../mathematical-logic.md#first-order-signature) specifies sorts, function symbols with specified input and output sorts, and relation symbols with specified input sorts. A [coherent formula](../../../mathematical-logic.md#coherent-formula) is built from atomic relations and equalities using $\top$, $\bot$, finite [logical conjunctions](../../../mathematical-logic.md#logical-conjunction), finite [logical disjunctions](../../../mathematical-logic.md#logical-disjunction), and [existential quantification](../../../mathematical-logic.md#existential-quantification). A [coherent theory](../../../mathematical-logic.md#coherent-theory) is a set of sequents $\phi\vdash_{\vec x}\psi$ between [coherent formulas](../../../mathematical-logic.md#coherent-formula) in a common finite context; its axioms are interpreted as universally closed implications. Neither general negation nor universal quantification is allowed inside [coherent formulas](../../../mathematical-logic.md#coherent-formula).

One complete presentation of [coherent logic](../../../mathematical-logic.md#coherent-logic) consists of the following axiom and rule schemes, together with the theory's sequents. All displayed formulas have compatible sorts and contexts, and bound variables can be renamed.

Identity and cut give $\phi\vdash\phi$ and

$$
\frac{\phi\vdash\psi\quad\psi\vdash\theta}{\phi\vdash\theta}.
$$

Substitution replaces the free variables of any derivable sequent by well-typed terms, avoiding capture. Contexts can be enlarged by unused variables, and permuted or renamed.

The finite-meet rules are $\phi\vdash\top$, $\phi\wedge\psi\vdash\phi$, $\phi\wedge\psi\vdash\psi$, and

$$
\frac{\theta\vdash\phi\quad\theta\vdash\psi}{\theta\vdash\phi\wedge\psi}.
$$

The finite-join rules are $\bot\vdash\phi$, $\phi\vdash\phi\vee\psi$, $\psi\vdash\phi\vee\psi$, and

$$
\frac{\phi\vdash\theta\quad\psi\vdash\theta}{\phi\vee\psi\vdash\theta}.
$$

Include distributivity $\theta\wedge(\phi\vee\psi)\dashv\vdash(\theta\wedge\phi)\vee(\theta\wedge\psi)$.

Existential introduction is $\phi(\vec x,t)\vdash_{\vec x}\exists y\,\phi(\vec x,y)$. Existential elimination is

$$
\frac{\phi(\vec x,y)\vdash_{\vec x,y}\psi(\vec x)}{\exists y\,\phi(\vec x,y)\vdash_{\vec x}\psi(\vec x)},
$$

where $y$ is absent from $\psi$. Equivalently, the quantifier is [left adjoint](../../../category.md#adjoint-functors) to weakening along the context projection. Include the [Frobenius rule in coherent logic](../../../mathematical-logic.md#frobenius-rule-in-coherent-logic)

$$
\theta(\vec x)\wedge\exists y\,\phi(\vec x,y)\dashv\vdash\exists y\,(\theta(\vec x)\wedge\phi(\vec x,y)).
$$

It can also be derived from the usual coherent natural-deduction rules.

Equality has $\top\vdash_x x=x$ and the substitution scheme

$$
x=y\wedge\phi(\vec z,x)\vdash_{\vec z,x,y}\phi(\vec z,y),
$$

including atomic formulas and terms of the signature. Symmetry, transitivity and congruence for all functions and relations follow. These schemes impose no unintended inhabitedness axiom on a sort.

The [coherent syntactic category](../../../mathematical-logic.md#coherent-syntactic-category) $\mathcal C_{\mathbb T}$ has objects formulas in context $[\vec x\mid\phi]$, up to renaming. An arrow from $[\vec x\mid\phi]$ to $[\vec y\mid\psi]$ is an equivalence class, modulo provable equivalence, of formulas $\theta(\vec x,\vec y)$ satisfying

$$
\theta\vdash\phi\wedge\psi,\qquad\phi\vdash_{\vec x}\exists\vec y\,\theta,
$$

and

$$
\theta(\vec x,\vec y)\wedge\theta(\vec x,\vec y')\vdash\bigwedge_i y_i=y_i'.
$$

These are provably total functional relations. The identity is the equality graph restricted by $\phi$. If $\theta$ and $\rho$ are consecutive arrows, their composite is represented by $\exists\vec y\,(\theta\wedge\rho)$. Equality, cut and existential rules give the category laws.

A [coherent category](../../../category-theory.md#coherent-category) has [finite limits](../../../category.md#finite-limit), [pullback](../../../category.md#pullback-category-theory)-stable regular-epi/mono image factorizations, and finite unions of [subobjects](../../../category.md#subobject) stable under [pullback](../../../category.md#pullback-category-theory). We verify these structures syntactically. The [terminal object](../../../category.md#terminal-object) is the empty-context truth formula. Products conjoin formulas in disjoint contexts; [equalizers](../../../category.md#equaliser) add equality of the two output tuples. For a functional relation $\theta$, its image in the target is represented by $\exists\vec x\,\theta$. Its factor onto that image is regular epic: two arrows out of the image agreeing on the source agree by existential elimination, and the same argument with the [kernel pair](../../../category.md#kernel-pair) gives the coequalizer property. Frobenius makes these image factorizations stable under [pullback](../../../category.md#pullback-category-theory).

Every [subobject](../../../category.md#subobject) of $[\vec x\mid\phi]$ is represented by a formula $\eta(\vec x)$ with $\eta\vdash\phi$. Indeed, take the existential image of a monic functional relation; uniqueness makes its map to that image an isomorphism. [Subobject](../../../category.md#subobject) inclusion is exactly provable implication. Finite unions are consequently disjunctions, with bottom as the empty [subobject](../../../category.md#subobject); distributivity and substitution make them [pullback](../../../category.md#pullback-category-theory)-stable. Hence **$\mathcal C_{\mathbb T}$ is coherent**.

The [conservative syntactic model](../../../mathematical-logic.md#conservative-syntactic-model) interprets a sort $S$ by $[x:S\mid\top]$, a function by its term graph, and a relation by its atomic-formula [subobject](../../../category.md#subobject). Induction on [coherent formulas](../../../mathematical-logic.md#coherent-formula) shows that $\phi(\vec x)$ is interpreted by the [subobject](../../../category.md#subobject) $[\vec x\mid\phi]$ of its context object. It satisfies every theory axiom by construction. Conversely, a sequent holds in this model exactly when the corresponding [subobject](../../../category.md#subobject) inclusion holds, which is exactly derivability in $\mathbb T$. Therefore

$$
\boxed{\text{the canonical model in }\mathcal C_{\mathbb T}\text{ is conservative}.}
$$

This is conservativity for [coherent sequents](../../../mathematical-logic.md#coherent-sequent), not a claim about non-[coherent formulas](../../../mathematical-logic.md#coherent-formula).

## Section B

↑ **Parent:** [Paper 20](paper-20.md)

### 4

↑ **Parent:** [Section B](#section-b)

<h4 id="4/i">i</h4>

↑ **Parent:** [4](#4)

<h5 id="4/i/solution">Solution</h5>

↑ **Parent:** [I](#4/i)

Write $\widehat{\mathcal C}=[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ and similarly for $\mathcal D$. The [geometric morphism induced by a functor](../../../category-theory.md#geometric-morphism-induced-by-a-functor) has

$$
\boxed{f^*P=P\circ F^{\mathrm{op}},\qquad f_*Q=\operatorname{Ran}_{F^{\mathrm{op}}}Q.}
$$

Precomposition preserves all pointwise limits and colimits, so in particular it preserves [finite limits](../../../category.md#finite-limit). The [Right Kan extension](../../../category.md#right-kan-extension) exists because the categories are small and sets have all small limits; its universal property gives $f^*\dashv f_*$. Thus these functors define a [geometric morphism](../../../category-theory.md#geometric-morphism) $\widehat{\mathcal C}\to\widehat{\mathcal D}$.

There is also $f_!=\operatorname{Lan}_{F^{\mathrm{op}}}$, a [left Kan extension](../../../category.md#left-kan-extension), with $f_!\dashv f^*$. The [Yoneda lemma](../../../category.md#yoneda-lemma) identifies $f_!(yC)\cong y(FC)$, since for every $P$,

$$
\operatorname{Hom}(f_!yC,P)\cong\operatorname{Hom}(yC,f^*P)\cong P(FC)\cong\operatorname{Hom}(y(FC),P).
$$

This is the [representable](../../../category.md#representable-functor) calculation used in the next parts.

<h4 id="4/ii">ii</h4>

↑ **Parent:** [4](#4)

<h5 id="4/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/ii)

A [representable functor](../../../category.md#representable-functor) $yC$ is an [indecomposable projective object](../../../category.md#indecomposable-projective-object). Given an [epimorphism](../../../category.md#epimorphism) $\coprod_iB_i\twoheadrightarrow yC$, evaluate at $C$. [Epimorphisms](../../../category.md#epimorphism) and [coproducts](../../../category.md#coproduct) in a [presheaf category](../../../category.md#presheaf-category) are pointwise, so $1_C\in yC(C)$ is the image of some element of a particular $B_i(C)$. By the [Yoneda lemma](../../../category.md#yoneda-lemma), that element defines $s:yC\to B_i$, and its composite into $yC$ corresponds to $1_C$, hence is the identity. The selected component is split epic. More generally, evaluation sends any epimorphism to a surjection, so a map from $yC$ lifts through any epimorphism; this also proves its ordinary projectivity.

Conversely, every presheaf $A$ has the canonical [epimorphism](../../../category.md#epimorphism)

$$
\coprod_{(C,x),\ x\in A(C)}yC\twoheadrightarrow A,
$$

whose component is the [natural transformation](../../../category.md#natural-transformation) named by $x$. It is pointwise surjective, since an element at $D$ is reached from its own summand $(D,x)$ at $1_D$. If $A$ is indecomposable projective, one component $r:yC\to A$ has a section $s:A\to yC$. The endomorphism $sr$ of $yC$ is idempotent and therefore corresponds to an [idempotent morphism](../../../category.md#idempotent-morphism) $e:C\to C$.

If idempotents split in $\mathcal C$, choose $C\xrightarrow{p}D\xrightarrow{i}C$ with $ip=e$, $pi=1_D$. Then $A\cong yD$: the mutually inverse maps are $y(p)s:A\to yD$ and $r\,y(i):yD\to A$. Thus

$$
\boxed{\text{indecomposable projectives are exactly representables when idempotents split}.}
$$

Without that hypothesis the argument still proves that every such object is a retract of a [representable](../../../category.md#representable-functor). The initial presheaf is not indecomposable projective, since its identity is the empty-[coproduct](../../../category.md#coproduct) [epimorphism](../../../category.md#epimorphism) and has no component to select.

<h4 id="4/iii">iii</h4>

↑ **Parent:** [4](#4)

<h5 id="4/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/iii)

The key fact is that the extra [left adjoint](../../../category.md#adjoint-functors) $f_!$ sends each [representable](../../../category.md#representable-functor) $yC$ to an [indecomposable projective object](../../../category.md#indecomposable-projective-object). Let $\coprod_iB_i\twoheadrightarrow f_!yC$ be epic. The inverse image $f^*$ preserves [epimorphisms](../../../category.md#epimorphism) and [coproducts](../../../category.md#coproduct), because it is a [left adjoint](../../../category.md#adjoint-functors) between toposes. Apply it and lift the unit $\eta:yC\to f^*f_!yC$ through the resulting [epimorphism](../../../category.md#epimorphism), using projectivity of $yC$. A map from $yC$ to a [coproduct](../../../category.md#coproduct) selects one component, by evaluation at $C$ and the [Yoneda lemma](../../../category.md#yoneda-lemma). Thus for some $i$ we obtain $t:yC\to f^*B_i$ with $f^*(B_i\to f_!yC)t=\eta$.

Transpose $t$ across $f_!\dashv f^*$ to $\bar t:f_!yC\to B_i$. The displayed equality says that its composite back to $f_!yC$ is the identity. This proves the required indecomposable-projective property.

Since idempotents split in $\mathcal D$, part (ii) supplies objects $FC\in\mathcal D$ and isomorphisms $f_!yC\cong y(FC)$. Full faithfulness of the [Yoneda embedding](../../../category.md#yoneda-embedding) transports the action of $f_!$ on [representable](../../../category.md#representable-functor) arrows to a functor $F:\mathcal C\to\mathcal D$. For $P\in\widehat{\mathcal D}$,

$$
(f^*P)(C)\cong\operatorname{Hom}(yC,f^*P)\cong\operatorname{Hom}(f_!yC,P)\cong P(FC).
$$

These identifications are natural in both $C$ and $P$. Hence

$$
\boxed{f^*\cong(-)\circ F^{\mathrm{op}}.}
$$

Its [right adjoint](../../../category.md#adjoint-functors) is consequently the right Kan extension from part (i), uniquely up to natural isomorphism. Thus the entire [geometric morphism](../../../category-theory.md#geometric-morphism) is induced by $F$.

<h4 id="4/iv">iv</h4>

↑ **Parent:** [4](#4)

<h5 id="4/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/iv)

The canonical [geometric morphism](../../../category-theory.md#geometric-morphism) $\widehat{\mathcal C}\to\mathbf{Set}$ has inverse image the constant-presheaf functor $\Delta$ and direct image the [global sections functor](../../../category-theory.md#global-sections-functor)

$$
\Gamma(P)=\operatorname{Hom}(1,P),\qquad\Delta\dashv\Gamma.
$$

If the [presheaf topos](../../../category.md#presheaf-topos) is a [local topos](../../../category-theory.md#local-topos), $\Gamma$ is also the inverse image of a [geometric morphism](../../../category-theory.md#geometric-morphism) $g:\mathbf{Set}\to\widehat{\mathcal C}$. This morphism has an extra [left adjoint](../../../category.md#adjoint-functors) $\Delta$. Apply part (iii) with source category $1$ and target category $\mathcal C$, using its idempotent-splitting hypothesis. Then $g$ is induced by a functor $1\to\mathcal C$, choosing an object $C_0$, and $\Gamma$ is naturally evaluation at $C_0$.

Since evaluation at $C_0$ is $\operatorname{Hom}(yC_0,-)$, this says $\operatorname{Hom}(1,-)\cong\operatorname{Hom}(yC_0,-)$. Uniqueness of representing objects gives $yC_0\cong1$. Thus $\mathcal C(C,C_0)$ is a singleton for every $C$: $C_0$ is terminal.

Conversely, if $C_0$ is terminal, $yC_0=1$ and $\Gamma(P)=P(C_0)$. Evaluation at that object preserves [finite limits](../../../category.md#finite-limit) and has a right Kan extension as [right adjoint](../../../category.md#adjoint-functors), so is an inverse image functor. Therefore, under the permitted idempotent-completeness assumption,

$$
\boxed{\widehat{\mathcal C}\text{ is local if and only if }\mathcal C\text{ has a terminal object}.}
$$

### 5

↑ **Parent:** [Section B](#section-b)

<h4 id="5/solution">Solution</h4>

↑ **Parent:** [5](#5)

The required condition is the [common-refinement condition for nonempty-sieve coverage](../../../category.md#common-refinement-condition-for-nonempty-sieve-coverage): for every pair $f:V\to U$, $g:W\to U$, there are arrows $h:T\to V$, $k:T\to W$ with

$$
\boxed{fh=gk.}
$$

Necessity follows by pulling back the nonempty sieve generated by $f$ along $g$: a member $k$ of the [pullback](../../../category.md#pullback-category-theory) sieve supplies such an $h$. Conversely, this condition makes the [pullback](../../../category.md#pullback-category-theory) of every nonempty [sieve on a category](../../../category.md#sieve-category-theory) nonempty. The maximal sieve is nonempty, and the transitivity axiom holds: if a sieve $S$ is locally covering along every member of a nonempty covering sieve $R$, choose $f\in R$ and then $g\in f^*S$; their composite is in $S$. Hence the nonempty sieves form a [Grothendieck topology](../../../category.md#grothendieck-topology), called the [atomic topology](../../../category.md#atomic-topology).

For all functions between nonempty finite sets, the two maps from a singleton to different points of a two-point set have no common refinement. Every potential domain remains nonempty, so the two constant composites cannot agree. The condition fails.

For surjections it holds: $V\times_UW$ is nonempty and both projections are surjective. Work from now on in a small skeleton $\mathcal D$ of nonempty finite sets and surjections. Every morphism $f:P\twoheadrightarrow U$ is a [regular epimorphism](../../../category.md#regular-epimorphism), with [kernel pair](../../../category.md#kernel-pair) $P\times_UP\rightrightarrows P$, and is the coequalizer of that pair in $\mathcal D$.

A matching family in a [representable](../../../category.md#representable-functor) $yV$ on the sieve generated by $f$ is determined by a surjection $t:P\to V$ equalizing that [kernel pair](../../../category.md#kernel-pair). It factors uniquely through a function $U\to V$, which is surjective because $t$ is. This gives the unique amalgamation. A general nonempty covering sieve contains such an $f$; after amalgamating there, common refinements with any other member force agreement on the entire sieve. Therefore **every [representable](../../../category.md#representable-functor) is a sheaf**, so this atomic site is [subcanonical](../../../category.md#subcanonical-topology).

For any sheaf $F$, every restriction $F(f)$ is injective: equality after a covering arrow forces equality by the separated part of the sheaf condition. We shall also use descent along any surjection $q:n\twoheadrightarrow k$:

$$
F(k)\longrightarrow F(n)\rightrightarrows F(n\times_kn)
$$

is an [equalizer](../../../category.md#equaliser) of sets. These are the [descent identities for the atomic finite-surjection site](../../../category.md#descent-identities-for-the-atomic-finite-surjection-site).

Consider primitive $x\in F(m)$, $y\in F(n)$ with a common restriction along $\alpha:P\twoheadrightarrow m$, $\beta:P\twoheadrightarrow n$. Suppose $a,b\in P$ have $\alpha(a)=\alpha(b)$ but $\beta(a)\ne\beta(b)$. Let $q:n\twoheadrightarrow n-1$ identify just the two points $\beta(a),\beta(b)$. Define the finite nonempty set

$$
T=\{(r,s)\in P^2:\alpha(r)=\alpha(s),\ q\beta(r)=q\beta(s)\}.
$$

Both projections $t_1,t_2:T\twoheadrightarrow P$ are surjective, since $T$ contains every diagonal pair. There is also a surjection

$$
h:T\twoheadrightarrow n\times_{n-1}n,\qquad(r,s)\longmapsto(\beta(r),\beta(s)).
$$

Indeed the target consists of diagonal pairs, which are reached because $\beta$ is surjective, and the two off-diagonal pairs corresponding to $\beta(a),\beta(b)$, reached by $(a,b)$ and $(b,a)$.

Since $\alpha t_1=\alpha t_2$, the common-restriction equality gives $F(\beta t_1)y=F(\beta t_2)y$. If $\pi_1,\pi_2$ are the target kernel-pair projections, this is

$$
F(h)F(\pi_1)y=F(h)F(\pi_2)y.
$$

Injectivity of $F(h)$ gives the kernel-pair matching condition on $y$. Descent along $q$ then writes $y=F(q)y'$, contradicting primitivity. Thus $\ker\alpha\subseteq\ker\beta$; interchange the roles to obtain equality. This is the [primitive-element kernel rigidity lemma](../../../category.md#primitive-element-kernel-rigidity-lemma).

Equal kernels produce a unique bijection $\gamma:m\to n$ with $\beta=\gamma\alpha$. Now $F(\alpha)x=F(\alpha)F(\gamma)y$, and injectivity implies

$$
\boxed{x=F(\gamma)y.}
$$

In particular equivalent primitive elements have the same cardinality and differ only by transport along a bijection.

Every element $z\in F(p)$ descends to a primitive one: whenever it is not primitive, descend along a surjection reducing the cardinality by one; this process terminates at or before cardinality one. Kernel rigidity shows that all primitive ancestors of $z$ lie in one equivalence class. Let $F_C(P)$ be the elements with primitive-ancestor class $C$. Restriction along a surjection preserves this class, so each $F_C$ is a subfunctor and

$$
F(P)=\coprod_CF_C(P)
$$

pointwise. Each $F_C$ is a sheaf. A matching family glues in $F$, and one member along a nonempty covering arrow already determines the primitive class of the glued element; it must be $C$.

Choose a representative primitive $x\in F(m)$ of $C$. The Yoneda map $ym\to F$ named by $x$ has image exactly $F_C$. It reaches all descendants of $x$, and every equivalent primitive ancestor is its transport along a bijection. It is therefore pointwise surjective onto $F_C$ and is epic as a map of sheaves. We obtain the [primitive decomposition of an atomic finite-surjection sheaf](../../../category.md#primitive-decomposition-of-an-atomic-finite-surjection-sheaf)

$$
\boxed{F\cong\coprod_CF_C,\qquad ym\twoheadrightarrow F_C.}
$$

This includes the empty [coproduct](../../../category.md#coproduct) for an empty sheaf.

Each nonempty $F_C$ is an [atom in a topos](../../../category-theory.md#atom-in-a-topos). If a sheaf [subobject](../../../category.md#subobject) $S\hookrightarrow F_C$ has an element $F(\alpha)x$ at some $P$, membership descends along the covering surjection $\alpha:P\to m$, so $x$ belongs to $S$. All its restrictions then belong to $S$, giving $S=F_C$. Thus every [subobject](../../../category.md#subobject) of any $F$ selects entire components of this [coproduct](../../../category.md#coproduct), and its complementary selection is again a sheaf [subobject](../../../category.md#subobject). Its characteristic map sends selected components to $\top$ and all others to $\bot$.

The constant two-element presheaf is a sheaf: a matching family on a nonempty sieve has the same value on all its arrows, since any two have a common refinement. The value extends uniquely. It therefore supplies these characteristic maps, with truth the inclusion of the $\top$ value. Equivalently, a J-closed sieve here is either empty or maximal, because every nonempty sieve covers. Hence

$$
\boxed{\Omega_{\mathbf{Sh}(\mathcal D,J)}=\text{the constant functor }\{\bot,\top\}.}
$$

### 6

↑ **Parent:** [Section B](#section-b)

<h4 id="6/i">i</h4>

↑ **Parent:** [6](#6)

<h5 id="6/i/solution">Solution</h5>

↑ **Parent:** [I](#6/i)

Let $\mathcal A=\mathbb T_{fp}$ be a small skeleton of the [finitely presented models of an algebraic theory](../../../foundations-of-mathematics.md#finitely-presented-models-of-an-algebraic-theory). The [classifying topos](../../../category-theory.md#classifying-topos) assertion means that for every [Grothendieck topos](../../../category-theory.md#grothendieck-topos) $\mathcal F$ there is an equivalence

$$
\boxed{\operatorname{Geom}(\mathcal F,[\mathcal A,\mathbf{Set}])\simeq\mathbb T\text{-}\operatorname{Mod}(\mathcal F),}
$$

natural under inverse image along [geometric morphisms](../../../category-theory.md#geometric-morphism). On the left, morphisms are transformations between inverse image functors, and on the right they are model homomorphisms. A model in $\mathcal F$ interprets the sorts by objects, the operations by arrows, and the equations by equality of the resulting arrows. Finite products suffice for these algebraic operations.

The [generic model of an algebraic theory](../../../category-theory.md#generic-model-of-an-algebraic-theory) is the tautological covariant functor: for each sort $S$ its component is

$$
U_S:\mathcal A\to\mathbf{Set},\qquad A\longmapsto A_S,
$$

with all operations interpreted pointwise. Pulling $U$ back by a [geometric morphism](../../../category-theory.md#geometric-morphism) gives its classified model. For a single-sorted theory, this is simply the underlying-set functor with its pointwise algebraic structure.

The orientation is important: $[\mathcal A,\mathbf{Set}]$ is the presheaf topos on $\mathcal A^{\mathrm{op}}$, and the generic model is covariant on finitely presented algebras. Such an algebra is a finite-generator, finite-relation presentation. In the algebraic syntactic category it corresponds to the formula imposing its relations, with arrows reversed. The finite-presentability/filtered-colimit description of algebraic models gives the above classifying equivalence; a detailed proof is not needed for this part.

<h4 id="6/ii">ii</h4>

↑ **Parent:** [6](#6)

<h5 id="6/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/ii)

Take $\mathcal A$ to be the category of finitely presented [commutative rings](../../../commutative-algebra.md#commutative-ring) with identity, and put $\mathcal C=\mathcal A^{\mathrm{op}}$. In its presheaf topos, the tautological ring $U(A)=A$ is generic. The additional domain axioms are [coherent sequents](../../../mathematical-logic.md#coherent-sequent), so they are imposed by a [quotient-theory coverage](../../../category-theory.md#quotient-theory-coverage) on $\mathcal C$.

Concretely, declare the zero ring covered by the empty family. For every finitely presented $A$ and elements $a,b\in A$ with $ab=0$, declare the two opposite quotient arrows associated with

$$
\boxed{A\longrightarrow A/(a),\qquad A\longrightarrow A/(b)}
$$

to be a covering family at $A$. These [quotient rings](../../../commutative-algebra.md#quotient-ring) are finitely presented. [Pullback](../../../category.md#pullback-category-theory) and transitivity generate a Grothendieck topology $J$ from these families. The empty cover forbids $0=1$; the two quotient covers make every zero product locally have a zero factor. Conversely, any internal integral domain satisfies exactly the continuity conditions prescribed by these generating covers. Thus

$$
\boxed{\mathbf{Sh}(\mathcal A^{\mathrm{op}},J)\text{ classifies integral domains},}
$$

and its generic domain is the associated sheaf $K=a_JU$, with the ring operations transported through the left-exact sheaf reflector.

This coverage is **not standard**, meaning not all [representables](../../../category.md#representable-functor) are sheaves; in modern terminology it is not subcanonical. For an explicit obstruction, use $A=\mathbb Z/4\mathbb Z$ and $a=b=2$. The two quotient arrows are the same map $A\to\mathbb Z/2\mathbb Z$, so their generated sieve is a singleton cover. Consider the [representable](../../../category.md#representable-functor) on $\mathcal C$ corresponding to $R=\mathbb Z[t]$:

$$
yR(A)=\operatorname{Hom}_{\mathrm{Ring}}(R,A).
$$

Its distinct sections $t\mapsto0$ and $t\mapsto2$ become equal after restriction to $\mathbb Z/2\mathbb Z$. Hence this [representable](../../../category.md#representable-functor) is not even separated for $J$. The [nilpotent element](../../../commutative-algebra.md#nilpotent) has to disappear in the generic domain, which explains this failure of standardness.

<h4 id="6/iii">iii</h4>

↑ **Parent:** [6](#6)

<h5 id="6/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/iii)

Work in the domain-classifying site of part (ii), with generic domain $K=a_JU$. For finitely presented rings $A$, the object $a_JyA$ is an available stage. Tuples of sections of $K$ are locally represented by tuples of actual elements of $A$, because $U\to a_JU$ is locally surjective and sheafification preserves finite products. It is therefore enough to prove the requested implication on such representatives.

We first note the [empty-cover criterion for the domain-classifying site](../../../category-theory.md#empty-cover-criterion-for-the-domain-classifying-site): $a_JyB$ is initial if and only if the finitely presented ring $B$ is the zero ring. One direction is the generating empty cover. Conversely, any nonzero ring has a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) and hence a homomorphism to a field. That field is a set-based integral domain and defines a point of the classifying topos. The inverse image of $a_JyB$ at this point is $\operatorname{Hom}_{\mathrm{Ring}}(B,L)$, which is nonempty for the chosen field $L$. It therefore cannot be the inverse image of an [initial object](../../../category.md#initial-object). This uses only the ordinary maximal-ideal existence principle externally, not excluded middle in the internal logic.

Suppose $a_1,\ldots,a_n\in A$ represent a tuple lying in the negation of the all-units [subobject](../../../category.md#subobject). Write $t=a_1\cdots a_n$ and consider the finitely presented [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring)

$$
B=A[1/t]\cong A[z]/(tz-1).
$$

Every $a_i$ is invertible in $B$, since $(\prod_{j\ne i}a_j)z$ is an inverse. But the pulled-back tuple still lies in the negation of the all-units [subobject](../../../category.md#subobject). Thus the whole stage $a_JyB$ maps into both that [subobject](../../../category.md#subobject) and its negation, forcing this stage to be initial. The empty-cover criterion gives $B=0$.

The localization $A[1/t]$ is zero precisely when $t^N=0$ in $A$ for some integer $N\geq1$, by the equality criterion in localization. Repeated use of the generating zero-product covers now gives a covering family

$$
A\longrightarrow A/(a_i)\qquad(1\leq i\leq n).
$$

Indeed, splitting $t^N=t\,t^{N-1}=0$ and inducting first forces $t=0$ locally; splitting the product $a_1\cdots a_n=0$ then forces one $a_i=0$ locally. More formally the two inductions are coherent derivations from the zero-product axiom, so their quotient families belong to the generated topology. The sheaf semantics of disjunction consequently gives

$$
\boxed{\neg\left(\bigwedge_{i=1}^n\exists y_i\,(x_iy_i=1)\right)\ \Longrightarrow\ \bigvee_{i=1}^n(x_i=0).}
$$

This is the [finite-tuple weak-field property of the generic integral domain](../../../category-theory.md#finite-tuple-weak-field-property-of-the-generic-integral-domain). The argument is intuitionistically valid inside the topos, although its description of the site uses ordinary external set theory. There is no appeal to preservation of negation by an arbitrary geometric inverse image.

For the converse assertion, let $R$ be any internally nontrivial commutative unital ring satisfying the $n=2$ implication. Assume $xy=0$. If $x$ and $y$ were both units, multiplying by their two inverses would give $0=1$, contradicting nontriviality. Therefore

$$
xy=0\quad\Longrightarrow\quad\neg\bigl(\operatorname{Unit}(x)\wedge\operatorname{Unit}(y)\bigr).
$$

The assumed two-variable implication then gives $x=0\vee y=0$. Together with nontriviality this is exactly the internal integral-domain axiom. Hence **a nontrivial ring satisfying the two-variable case is an integral domain**.

For example, the ordinary integral domain $\mathbb Z$ fails the one-variable implication at $2$. This does not contradict the generic result: the displayed implication uses negation and is non-coherent, so it need not survive the inverse image that classifies an arbitrary set-based domain.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
