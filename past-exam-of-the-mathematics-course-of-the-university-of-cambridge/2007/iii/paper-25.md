# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper25.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
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
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Both alternatives can be proved using the same smallness mechanism. We first establish the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set), then obtain the two [adjoint functor](../../../category.md#adjoint-functors) existence theorems and their applications.

Let $\mathcal E$ be a [locally small category](../../../category.md#locally-small-category) with all small [categorical limits](../../../category.md#categorical-limit) and a [weakly initial set](../../../category.md#weakly-initial-set) $(W_i)_{i\in I}$. Its [product in a category](../../../category.md#product-category-theory) $W=\prod_iW_i$ is weakly initial: given any object, choose a map from some $W_i$ and compose with the corresponding projection. Take the simultaneous [equalizer](../../../category.md#equaliser) $e:E\to W$ of every endomorphism of $W$ and its identity; local smallness makes this a small [categorical limit](../../../category.md#categorical-limit). Then $E$ is also weakly initial. If $a,b:E\to X$, form their [equalizer](../../../category.md#equaliser) $j:Y\to E$ and choose $t:W\to Y$. Since $ejt$ is an endomorphism of $W$, the construction of $e$ gives $ejte=e$. Cancelling the [monomorphism](../../../category.md#monomorphism) $e$ yields $jte=1_E$. Thus $j$ is both a [monomorphism](../../../category.md#monomorphism) and a [split epimorphism](../../../category.md#split-epimorphism), hence invertible, and $a=b$. There is therefore exactly one arrow from $E$ to every object: $E$ is initial.

The [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) says that for a [functor](../../../category.md#functor) $U:\mathcal A\to\mathcal B$ between [locally small categories](../../../category.md#locally-small-category), with $\mathcal A$ complete, a [left adjoint](../../../category.md#adjoint-functors) exists exactly when $U$ preserves all small [categorical limits](../../../category.md#categorical-limit) and satisfies the [solution-set condition](../../../category.md#solution-set-condition). That condition requires, for each $B$, a set of arrows $u_i:B\to UA_i$ such that every $u:B\to UA$ factors as $U(f)u_i$ for some $i$ and $f:A_i\to A$.

For sufficiency, the [comma category](../../../category.md#comma-category) $(B\downarrow U)$ is locally small and complete: form a diagram's [categorical limit](../../../category.md#categorical-limit) in $\mathcal A$, and use [categorical limit](../../../category.md#categorical-limit) preservation to obtain its arrow from $B$. The solution set is a [weakly initial set](../../../category.md#weakly-initial-set) in this [comma category](../../../category.md#comma-category). The lemma provides an [initial object](../../../category.md#initial-object) $(LB,\eta_B:B\to ULB)$. Its [universal property](../../../category-theory.md#universal-property) gives

$$
\mathcal A(LB,A)\cong\mathcal B(B,UA),\qquad f\longmapsto U(f)\eta_B.
$$

For $h:B\to B'$, define $Lh$ by $U(Lh)\eta_B=\eta_{B'}h$. Uniqueness proves the identity and composition laws and [naturality](../../../category.md#naturality) of the displayed bijections, hence $L\dashv U$. Conversely, an [adjunction](../../../category.md#adjoint-functors) makes $U$ preserve [categorical limits](../../../category.md#categorical-limit), since the corresponding [hom-set](../../../category.md#hom-set) [functors](../../../category.md#functor) turn a [categorical limit](../../../category.md#categorical-limit) cone into a [categorical limit](../../../category.md#categorical-limit) of sets. The single arrow $\eta_B$ is a solution set. This proves both directions of the theorem.

Now let $F:\mathcal C\to\mathcal D$ have small domain and codomain. The [functor categories](../../../category.md#functor-category) $[\mathcal D,\mathbf{Set}]$ and $[\mathcal C,\mathbf{Set}]$ are locally small, and their [categorical limits](../../../category.md#categorical-limit) are pointwise. Thus the precomposition [functor](../../../category.md#functor) $F^*$ preserves [categorical limits](../../../category.md#categorical-limit) and its domain is complete. To verify its [solution-set condition](../../../category.md#solution-set-condition), fix $X:\mathcal C\to\mathbf{Set}$ and an arrow $x:X\to F^*Y$. Let $Y_0\subseteq Y$ be the subfunctor generated by all elements $x_c(a)$, where $c\in\mathcal C$ and $a\in X(c)$. Explicitly,

$$
Y_0(d)=\{Y(g)(x_c(a)):g:Fc\to d,\ a\in X(c)\}.
$$

These sets are stable under every $Y(h)$. If $\kappa$ is an infinite cardinal bounding $|\operatorname{Mor}\mathcal D|$ and $\left|\coprod_cX(c)\right|$, every $Y_0(d)$ has cardinal at most $\kappa$. Replace each such set by a subset of a fixed set of size $\kappa$. There is only a set of choices of these subsets, of their action maps for the set of arrows of $\mathcal D$, and of maps from $X$ to their restrictions. These coded pairs form a solution set: $x$ factors through $F^*Y_0$ and then the inclusion $Y_0\hookrightarrow Y$. The general theorem now yields

$$
\boxed{\operatorname{Lan}_F\dashv F^*.}
$$

Its values may also be written $\operatorname{Lan}_FX(d)=\operatorname{colim}_{(Fc\to d)}X(c)$, the usual [left Kan extension](../../../category.md#left-kan-extension) formula.

For the other alternative, the [categorical limit](../../../category.md#categorical-limit) form of the [Special adjoint functor theorem](../../../category.md#special-adjoint-functor-theorem) says that a limit-preserving [functor](../../../category.md#functor) $U:\mathcal A\to\mathcal B$ has a left adjoint if $\mathcal A$ is locally small, complete and [well-powered](../../../category.md#well-powered-category), has a [cogenerating set](../../../category.md#cogenerating-set) $(Q_i)_{i\in I}$, and $\mathcal B$ is locally small. A cogenerating set means that maps into its members distinguish any two parallel arrows. The dual theorem says that a colimit-preserving [functor](../../../category.md#functor) from a locally small, cocomplete, [well-copowered category](../../../category.md#well-copowered-category) with a [small generating family](../../../category.md#generating-set-in-a-category) has a right adjoint. These conclusions are also necessary in their preservation clauses.

Here is a proof of the special theorem rather than an invocation of the general theorem without its required solution set. Given $(A,x:B\to UA)$, intersect all subobjects $m:M\hookrightarrow A$ through which $x$ factors after application of $U$. There are only a set of them by well-poweredness. Their intersection is a wide pullback, preserved by $U$, so gives a smallest supporting pair $(A_0,x_0)$. If $p,q:A_0\to Q_i$ satisfy $U(p)x_0=U(q)x_0$, their [equalizer](../../../category.md#equaliser) is a supporting subobject. Minimality makes that [equalizer](../../../category.md#equaliser) invertible, whence $p=q$. Consequently

$$
\mathcal A(A_0,Q_i)\longrightarrow\mathcal B(B,UQ_i),\qquad p\longmapsto U(p)x_0,
$$

is injective. The cogenerating property makes the evaluation arrow from $A_0$ into the [product in a category](../../../category.md#product-category-theory) of the $Q_i$, one factor for each map $A_0\to Q_i$, a [monic arrow](../../../category.md#monomorphism). Its indexing set at each $i$ is identified with a subset of the fixed set $\mathcal B(B,UQ_i)$. Only a set of such [products in a category](../../../category.md#product-category-theory) can occur. Each has only a set of subobjects, and each possible subobject has only a set of arrows from $B$ into its image under $U$. These pairs give a [weakly initial set](../../../category.md#weakly-initial-set) in $(B\downarrow U)$, since every original pair receives the arrow from its minimal supporting pair. The complete-category lemma now gives the adjoint. Reversing all arrows proves the [colimit](../../../category.md#colimit) form of the special theorem.

Apply that dual form to $F^*:[\mathcal D,\mathbf{Set}]\to[\mathcal C,\mathbf{Set}]$. Its domain is cocomplete and locally small, and $F^*$ preserves pointwise [colimits](../../../category.md#colimit). The set of covariant [representable functors](../../../category.md#representable-functor) $\mathcal D(d,-)$ generates the domain: by the [Yoneda lemma](../../../category.md#yoneda-lemma), maps from these representables probe every element at every object and hence distinguish distinct [natural transformations](../../../category.md#natural-transformation). Finally, [epimorphisms](../../../category.md#epimorphism) in this [functor category](../../../category.md#functor-category) are pointwise surjective. Indeed, their pointwise images form subfunctors; if an image is proper, the two inclusions into the pointwise pushout of two copies of the target over that image distinguish the original map, contradicting epicity. Quotients of a fixed [functor](../../../category.md#functor) are therefore specified by compatible equivalence relations on its sets of values, and form a set. Thus the domain is a [well-copowered category](../../../category.md#well-copowered-category). All special-theorem hypotheses hold, giving

$$
\boxed{F^*\dashv\operatorname{Ran}_F.}
$$

Here the [Right Kan extension](../../../category.md#right-kan-extension) can be written $\operatorname{Ran}_FX(d)=\operatorname{Nat}(\mathcal D(d,F-),X)$. In particular both requested adjoints exist, although the two proofs use different smallness hypotheses.

## 2

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**Definitions organize [category theory](../../../category-theory.md), but theorems give that organization mathematical force.** I would therefore argue against treating the subject as an exception in which definitions are intrinsically more important than theorems. The distinction is especially misleading here because good categorical definitions are designed to expose hypotheses from which substantial theorems follow.

A [category](../../../category.md) records objects, composable arrows, identities and associative composition. A [functor](../../../category.md#functor) preserves that structure. This language allows one to compare otherwise different mathematical settings, but it does not itself say which constructions exist. For example, the definition of a [product in a category](../../../category.md#product-category-theory) is not a recipe for forming a [Cartesian product](../../../set-theory.md#cartesian-product) of underlying sets: it requires a universal factorization of pairs of arrows. If two [products in a category](../../../category.md#product-category-theory) $(P,p_1,p_2)$ and $(Q,q_1,q_2)$ exist, the universal properties give unique arrows $f:P\to Q$ and $g:Q\to P$ respecting projections. The composites $gf$ and $fg$ respect the same projections as the identities, so uniqueness forces them to be identities. Thus a definition yields a genuine theorem: [products in a category](../../../category.md#product-category-theory) are unique up to unique compatible isomorphism. The proof matters because it licenses replacing a construction by any other realization of the same property.

The [Yoneda lemma](../../../category.md#yoneda-lemma) is a more substantial example. For a covariant [representable functor](../../../category.md#representable-functor) $\mathcal C(A,-)$ and $X:\mathcal C\to\mathbf{Set}$, a [natural transformation](../../../category.md#natural-transformation) $t:\mathcal C(A,-)\to X$ is determined by $a=t_A(1_A)$. [Naturality](../../../category.md#naturality) forces

$$
t_B(f)=X(f)(a).
$$

Conversely this formula defines a [natural transformation](../../../category.md#natural-transformation) for every $a\in X(A)$. Hence $\operatorname{Nat}(\mathcal C(A,-),X)\cong X(A)$. The definition of [naturality](../../../category.md#naturality) is indispensable, but the theorem identifies every possible transformation, proves representables detect arrows, and explains why universal objects can be studied through [hom-sets](../../../category.md#hom-set). Merely knowing the definition does not supply this conclusion.

Similarly, an [adjunction](../../../category.md#adjoint-functors) is defined by natural [hom-set](../../../category.md#hom-set) bijections. The construction of a [free abelian group](../../../group-theory.md#free-abelian-group) gives $\mathbf{Ab}(\mathbb Z^{(S)},A)\cong\mathbf{Set}(S,UA)$, because a [group homomorphism](../../../group-theory.md#group-homomorphism) is determined uniquely by its values on the basis. This makes a universal extension problem transparent. But the [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) goes further: it turns [categorical limit](../../../category.md#categorical-limit) preservation and a solution set into an actual adjoint. Its smallness hypotheses cannot be discarded as bookkeeping. For instance, the underlying-set [functor](../../../category.md#functor) from finite groups to finite sets has no left adjoint at a singleton. A putative universal finite [group](../../../group.md) with universal element of order $m$ could not map that element to a generator of a finite cyclic group of order greater than $m$. The theorem's hypotheses separate existence from attractive notation.

The [monoidal coherence theorem](../../../category-theory.md#monoidal-coherence-theorem) offers another example. A [monoidal category](../../../category-theory.md#monoidal-category) has associativity and unit isomorphisms satisfying the [pentagon identity for a monoidal category](../../../category-theory.md#pentagon-identity-for-a-monoidal-category) and [triangle identity for a monoidal category](../../../category-theory.md#triangle-identity-for-a-monoidal-category). Coherence proves that every formal reassociation and unit insertion produces the same structural map. This is what justifies calculating without displaying all parentheses; it is not true merely because one has named an [associator](../../../category-theory.md#associator). Nor does it identify arbitrary additional maps, such as distinct braidings.

Finally, the [opposite category](../../../category.md#opposite-category) construction shows how a definition can economize on proofs: reversing arrows takes [products in a category](../../../category.md#product-category-theory) to [coproducts in a category](../../../category.md#coproduct), [initial objects](../../../category.md#initial-object) to [terminal objects](../../../category.md#terminal-object) and [monads](../../../category-theory.md#monad) to comonads. Yet this economy works because theorems and their proofs are invariant under the reversal. The subject is powerful precisely when definitions isolate reusable structure and theorems establish its consequences. Separating their importance obscures that partnership.

## 3

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Write the square as $GH=KF$, with $F:\mathcal A\to\mathcal B$ final and $G:\mathcal C\to\mathcal D$ a [discrete fibration](../../../category.md#discrete-fibration). For $b\in\mathcal B$, choose an object $(a,h:b\to Fa)$ of the nonempty [comma category](../../../category.md#comma-category) $(b\downarrow F)$. Lift $K(h):Kb\to GHa$ uniquely to an arrow

$$
\ell_h:c_h\longrightarrow Ha
$$

over $K(h)$, and tentatively put $L(b)=c_h$.

A morphism $(a,h)\to(a',h')$ in this [comma category](../../../category.md#comma-category) is an arrow $j:a\to a'$ with $F(j)h=h'$. The composite $H(j)\ell_h$ is a lift of $K(h')$ with codomain $Ha'$. Uniqueness of lifts gives $H(j)\ell_h=\ell_{h'}$, including equality of their source objects. Since the [comma category](../../../category.md#comma-category) is connected by zigzags, $c_h$ is independent of the choice. Thus $L(b)$ is well defined and $GL(b)=Kb$.

For $f:b\to b'$, take $(a',h':b'\to Fa')$. Lift $K(f)$ into $L(b')$, obtaining $t:c\to L(b')$. Composing with $\ell_{h'}$ gives a lift of $K(h'f)$ into $Ha'$, whose source must be $L(b)$. Hence $t:L(b)\to L(b')$. Set $L(f)=t$. Uniqueness of this lift makes the definition independent of the chosen comma object and proves $L(1_b)=1_{L(b)}$ and $L(gf)=L(g)L(f)$.

At $b=Fa$, choose $(a,1_{Fa})$. Its lift is $1_{Ha}$, so $L(Fa)=Ha$. For $j:a\to a'$, $Hj$ is the unique lift of $K(Fj)$ into $Ha'$, so $L(Fj)=Hj$. We have constructed the required [functor](../../../category.md#functor) with $LF=H$ and $GL=K$.

If $L'$ is another filler, $L'(h):L'b\to Ha$ must equal $\ell_h$ by unique lifting. Thus $L'b=L(b)$ for every object. Its arrows are then forced by unique lifting into those objects. Therefore

$$
\boxed{L\text{ exists and is unique}.}
$$

This proves the [orthogonality of final functors and discrete fibrations](../../../category.md#orthogonality-of-final-functors-and-discrete-fibrations).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For each $d\in\mathcal D$, let $P(d)=\pi_0(d\downarrow F)$, the collection of connected components, where connectedness means connection by a zigzag of arrows. Precomposition with $u:d\to d'$ gives a function $P(u):P(d')\to P(d)$. Identity and composition are inherited from precomposition.

Construct a [category](../../../category.md) $\mathcal E$ whose objects are pairs $(d,c)$ with $c\in P(d)$. An arrow $(d,c)\to(d',c')$ is an arrow $u:d\to d'$ satisfying $c=P(u)c'$. Composition is that of $\mathcal D$, and the component equation is preserved by composition. The projection $p:\mathcal E\to\mathcal D$ is a [discrete fibration](../../../category.md#discrete-fibration): an arrow $u:d\to d'$ has precisely one lift into $(d',c')$, namely the arrow from $(d,P(u)c')$ represented by $u$.

Define $J:\mathcal C\to\mathcal E$ by

$$
J(a)=(Fa,[(a,1_{Fa})]),\qquad J(j)=F(j).
$$

This is well defined because $(a,1_{Fa})$ and $(a',Fj)$ lie in the same component of $(Fa\downarrow F)$ whenever $j:a\to a'$. Clearly $pJ=F$.

For an object $(d,c)$ of $\mathcal E$, an object of $((d,c)\downarrow J)$ is exactly a pair $(a,u:d\to Fa)$ representing the component $c$. Its morphisms are exactly the arrows in $(d\downarrow F)$ between such objects. Thus this [comma category](../../../category.md#comma-category) is the component $c$ itself, which is nonempty and connected. This proves that $J$ is a [final functor](../../../category.md#final-functor), and hence

$$
\boxed{F=pJ,\qquad J\text{ final},\quad p\text{ a discrete fibration}.}
$$

This is the [final-discrete-fibration factorization](../../../category.md#final-discrete-fibration-factorization). For small [categories](../../../category.md) the collections $P(d)$ are sets and this construction is the [category of elements](../../../category.md#category-of-elements) of the presheaf $P$. For [categories](../../../category.md) of a larger size, the construction is interpreted in the same chosen ambient size framework.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Suppose $F=pJ=p'J'$ are two such factorizations, with $J,J'$ final and $p,p'$ [discrete fibrations](../../../category.md#discrete-fibration). Apply the unique diagonal construction to the square with left side $J$, top $J'$, bottom $p$ and right side $p'$. It gives a unique [functor](../../../category.md#functor) $L:\mathcal E\to\mathcal E'$ such that $LJ=J'$ and $p'L=p$. Reversing the two factorizations gives $M:\mathcal E'\to\mathcal E$ with $MJ'=J$ and $pM=p'$.

Both $ML$ and $1_{\mathcal E}$ fill the square with left side $J$, top $J$, bottom $p$ and right side $p$. Uniqueness from part (i) gives $ML=1_{\mathcal E}$. Similarly $LM=1_{\mathcal E'}$. Thus

$$
\boxed{L:\mathcal E\xrightarrow{\sim}\mathcal E'\text{ is the unique compatible isomorphism}.}
$$

In particular the conclusion is a canonical isomorphism of intermediate [categories](../../../category.md), not just an unspecified equivalence.

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write the [monad](../../../category-theory.md#monad) identities as

$$
\mu_A\eta_{TA}=1_{TA}=\mu_AT\eta_A,\qquad
\mu_AT\mu_A=\mu_A\mu_{TA}.
$$

If $\mu_A$ is invertible, its two right inverses agree, so $\eta_{TA}=T\eta_A$. Conversely, suppose $\eta_T=T\eta$. [Naturality](../../../category.md#naturality) of $\eta$ at $\mu_A$, followed by that equality at $TA$, gives

$$
\eta_{TA}\mu_A=T\mu_A\eta_{TTA}=T\mu_AT\eta_{TA}=T(\mu_A\eta_{TA})=1_{TTA}.
$$

Together with $\mu_A\eta_{TA}=1_{TA}$ this proves

$$
\boxed{\mu\text{ is invertible}\ \Longleftrightarrow\ \eta_T=T\eta,\qquad\mu^{-1}=\eta_T=T\eta.}
$$

This is the equivalence defining an [idempotent monad](../../../category-theory.md#idempotent-monad).

For the [equalizer submonad of a monad](../../../category-theory.md#equalizer-submonad-of-a-monad), let $\beta_A:RA\to TA$ equalize $\eta_{TA}$ and $T\eta_A$. If $f:A\to B$, [naturality](../../../category.md#naturality) of these two transformations shows that $Tf\beta_A$ equalizes the corresponding pair at $B$. There is therefore a unique $Rf$ satisfying

$$
\beta_BRf=Tf\beta_A.
$$

Uniqueness gives $R1=1$ and $R(gf)=Rg\,Rf$, so $R$ is a [functor](../../../category.md#functor) and $\beta:R\Rightarrow T$ is a [natural transformation](../../../category.md#natural-transformation).

Take the stipulated factorizations $\alpha_A$ and $\theta_A$. [Naturality](../../../category.md#naturality) of $\beta$ at $\beta_A$ rewrites their defining equations as

$$
\beta_A\alpha_A=\eta_A,\qquad
\beta_A\theta_A=\mu_A\beta_{TA}R\beta_A=\mu_AT\beta_A\beta_{RA}.
$$

The composites on the right are natural in $A$; cancellation of the [monic arrow](../../../category.md#monomorphism) $\beta_A$ therefore makes $\alpha$ and $\theta$ natural. We now verify every [monad](../../../category-theory.md#monad) law, rather than assuming that restricting the structure automatically preserves them.

For the two unit laws, [naturality](../../../category.md#naturality) and the unit laws of $T$ give

$$
\begin{aligned}
\beta_A\theta_A\alpha_{RA}
&=\mu_AT\beta_A\eta_{RA}
=\mu_A\eta_{TA}\beta_A=\beta_A,\\
\beta_A\theta_AR\alpha_A
&=\mu_AT\beta_AT\alpha_A\beta_A
=\mu_AT\eta_A\beta_A=\beta_A.
\end{aligned}
$$

Cancelling $\beta_A$ proves $\theta_A\alpha_{RA}=1_{RA}=\theta_AR\alpha_A$. For associativity, the same [naturality](../../../category.md#naturality) equations give

$$
\begin{aligned}
\beta_A\theta_AR\theta_A
&=\mu_AT\mu_A\,TT\beta_A\,T\beta_{RA}\,\beta_{RRA},\\
\beta_A\theta_A\theta_{RA}
&=\mu_A\mu_{TA}\,TT\beta_A\,T\beta_{RA}\,\beta_{RRA}.
\end{aligned}
$$

These are equal by associativity of $\mu$; cancelling $\beta_A$ proves associativity of $\theta$. Thus

$$
\boxed{(R,\alpha,\theta)\text{ is a monad, and }\beta:R\Rightarrow T\text{ is a monad morphism}.}
$$

The remaining claims use two [split equalizers associated with a monad](../../../category.md#split-equalizers-associated-with-a-monad). First, $\eta_{TA}:TA\to TTA$ is a [split equalizer](../../../category.md#split-equalizer) of $\eta_{TTA},T\eta_{TA}$. Its retraction is $\mu_A$, and the splitting of the parallel pair is $T\mu_A$, since

$$
\mu_A\eta_{TA}=1,\qquad
T\mu_A\eta_{TTA}=\eta_{TA}\mu_A,\qquad
T\mu_AT\eta_{TA}=1.
$$

The equalizing equation follows from [naturality](../../../category.md#naturality) of $\eta$. In general, identities $re=1$, $sf=er$, $sg=1$ and $fe=ge$ prove that $e$ is an [equalizer](../../../category.md#equaliser): if $fh=gh$, then $h=erh$, with unique factorization $rh$. Hence $\eta_{TA}$ and $\beta_{TA}$ are two [equalizers](../../../category.md#equaliser) of the same pair. Their comparison is $\alpha_{TA}$, and its inverse is $\mu_A\beta_{TA}$. In particular

$$
\boxed{\alpha_{TA}\text{ is invertible},\qquad \alpha_{TA}^{-1}=\mu_A\beta_{TA}.}
$$

Second, $e_A=T\eta_A:TA\to TTA$ is a [split equalizer](../../../category.md#split-equalizer) of $TT\eta_A,T\eta_{TA}$, with retraction $\mu_A$ and splitting $\mu_{TA}$. Indeed,

$$
\mu_AT\eta_A=1,\qquad
\mu_{TA}TT\eta_A=T\eta_A\mu_A,\qquad
\mu_{TA}T\eta_{TA}=1.
$$

This is precisely the parallel pair in the PDF's diagram after $T\beta_A$. The map $T\beta_A$ equalizes that pair, because applying $T$ to the defining [equalizer](../../../category.md#equaliser) equation gives their equality on $T\beta_A$. Put

$$
h_A=\mu_AT\beta_A:TRA\to TA.
$$

The split-equalizer factorization and $\beta_A\alpha_A=\eta_A$ give

$$
e_Ah_A=T\beta_A,\qquad h_AT\alpha_A=1_{TA}.
$$

If $T\alpha_A$ is invertible, then $T\beta_A=e_A(T\alpha_A)^{-1}$ is a [monic arrow](../../../category.md#monomorphism). Conversely, if $T\beta_A$ is a [monic arrow](../../../category.md#monomorphism), the equation

$$
T\beta_A(T\alpha_Ah_A)=e_Ah_A=T\beta_A
$$

forces $T\alpha_Ah_A=1_{TRA}$, so $h_A$ is the inverse of $T\alpha_A$. Therefore

$$
\boxed{T\alpha_A\text{ invertible}\ \Longleftrightarrow\ T\beta_A\text{ monic}.}
$$

Notice that, under either condition, $T\beta_A$ is actually a [split monomorphism](../../../category.md#split-monomorphism), with retraction $T\alpha_A\mu_A$. Thus $TT\beta_A$ is a [monic arrow](../../../category.md#monomorphism) too, since a [functor](../../../category.md#functor) preserves [split monomorphisms](../../../category.md#split-monomorphism). We have not assumed that $T$ preserves arbitrary [monomorphisms](../../../category.md#monomorphism).

Now prove the specified [naturality](../../../category.md#naturality) square is a [pullback in a category](../../../category.md#pullback-category-theory). Let $x:X\to TRA$ and $y:X\to RTA$ satisfy $T\beta_Ax=\beta_{TA}y$. [Naturality](../../../category.md#naturality) of $\eta$, followed by the [equalizer](../../../category.md#equaliser) equation for $\beta_{TA}$, gives

$$
\begin{aligned}
TT\beta_A\eta_{TRA}x
&=\eta_{TTA}T\beta_Ax
=\eta_{TTA}\beta_{TA}y\\
&=T\eta_{TA}\beta_{TA}y
=T\eta_{TA}T\beta_Ax
=TT\beta_AT\eta_{RA}x.
\end{aligned}
$$

Cancel the [monic arrow](../../../category.md#monomorphism) $TT\beta_A$. Thus $x$ equalizes $\eta_{TRA},T\eta_{RA}$ and factors uniquely as $x=\beta_{RA}z$ with $z:X\to RRA$. [Naturality](../../../category.md#naturality) of $\beta$ then gives

$$
\beta_{TA}R\beta_Az=T\beta_A\beta_{RA}z=T\beta_Ax=\beta_{TA}y.
$$

Cancel $\beta_{TA}$ to obtain $R\beta_Az=y$. This is exactly existence and uniqueness in the pullback [universal property](../../../category-theory.md#universal-property).

Because the square is a pullback and $T\beta_A$ is a [monic arrow](../../../category.md#monomorphism), $R\beta_A$ is a [monic arrow](../../../category.md#monomorphism). [Naturality](../../../category.md#naturality) of $\alpha$ and the formula for $\theta$ now give

$$
R\beta_A\alpha_{RA}\theta_A
=\alpha_{TA}\beta_A\theta_A
=\alpha_{TA}\mu_A\beta_{TA}R\beta_A
=R\beta_A.
$$

Cancelling $R\beta_A$ proves $\alpha_{RA}\theta_A=1_{RRA}$. The other composite is already one of the unit laws. Hence $\theta_A$ is invertible. If the equivalent monicity conditions hold for every $A$, we conclude

$$
\boxed{(R,\alpha,\theta)\text{ is idempotent},\qquad \theta^{-1}=\alpha_R=R\alpha.}
$$

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [preadditive category](../../../category.md#preadditive-category) has an abelian-group structure on every [hom-set](../../../category.md#hom-set) and bilinear composition. One equivalent definition of an [additive category](../../../category-theory.md#additive-category) is a [preadditive category](../../../category.md#preadditive-category) with a [zero object](../../../category.md#zero-object) and finite [products in a category](../../../category.md#product-category-theory); the following argument proves that these [products in a category](../../../category.md#product-category-theory) are automatically [coproducts in a category](../../../category.md#coproduct). An [abelian category](../../../category-theory.md#abelian-category) is an [additive category](../../../category-theory.md#additive-category) with kernels and cokernels in which every [monomorphism](../../../category.md#monomorphism) is a kernel and every [epimorphism](../../../category.md#epimorphism) is a cokernel. Equivalently, for every arrow the canonical map from its coimage to its image is invertible.

Let $P=\prod_{i=1}^nA_i$, with projections $p_i$. Define $\iota_i:A_i\to P$ by $p_j\iota_i=\delta_{ji}$, where the diagonal entry is the identity and the others are zero. Since its composites with all projections are identities,

$$
\sum_i\iota_ip_i=1_P.
$$

Given $f_i:A_i\to B$, the map $f=\sum_if_ip_i$ satisfies $f\iota_i=f_i$. If another map has those composites, multiplying the displayed identity by that map forces it to equal $f$. Thus $P$ is also a [coproduct in a category](../../../category.md#coproduct). The empty case is the [zero object](../../../category.md#zero-object). Reversing arrows proves that a finite [coproduct in a category](../../../category.md#coproduct) is likewise a [product in a category](../../../category.md#product-category-theory). Hence **finite [products in a category](../../../category.md#product-category-theory) and [coproducts in a category](../../../category.md#coproduct) are canonically [biproducts](../../../category-theory.md#biproduct)** in an [additive category](../../../category-theory.md#additive-category).

For the [category of abelian groups](../../../category-theory.md#category-of-abelian-groups), let $(A_i,D_{ij})$ be a directed diagram, with no injectivity assumption on its transition maps. Its set [colimit](../../../category.md#colimit) consists of classes $[i,a]$, with

$$
[i,a]=[j,b]\quad\Longleftrightarrow\quad D_{ik}a=D_{jk}b\text{ for some }k\geq i,j.
$$

Directedness proves transitivity of this relation. Define addition by moving representatives to a common upper index:

$$
[i,a]+[j,b]=[k,D_{ik}a+D_{jk}b].
$$

Moving all indices involved to one further upper bound proves independence of representatives and of $k$. Define $-[i,a]=[i,-a]$ and use the common class of the zeros as zero. The abelian-group laws hold at a common index, so descend to the quotient. Every canonical map $A_i\to C$ is a homomorphism, and a compatible cocone induces the homomorphism $[i,a]\mapsto f_i(a)$. This is the unique extension. Moreover the formula for addition is forced by those canonical homomorphisms, proving that the underlying-set [functor](../../../category.md#functor) creates directed [colimits](../../../category.md#colimit). This establishes [directed colimits created by the abelian-group forgetful functor](../../../category.md#directed-colimits-created-by-the-abelian-group-forgetful-functor) explicitly.

If a cocone $\nu_i:A_i\to B$ has injective legs, the induced map $C\to B$ is injective. Indeed, equal images of $[i,a]$ and $[j,b]$ give, at a common index $k$,

$$
\nu_k(D_{ik}a)=\nu_i(a)=\nu_j(b)=\nu_k(D_{jk}b).
$$

Injectivity of $\nu_k$ gives equal representatives at $k$. Since [monomorphisms](../../../category.md#monomorphism) of [abelian groups](../../../group.md#abelian-group) are exactly injective homomorphisms, we have proved that **the [category of abelian groups](../../../category-theory.md#category-of-abelian-groups) is a finitary [abelian category](../../../category-theory.md#abelian-category)** in the directed-union sense of the question.

Now let $\mathcal A$ be complete, cocomplete and finitary. Index by finite subsets $J\subseteq I$ and put $S_J=\bigoplus_{j\in J}A_j$. For $J\subseteq K$, insert the additional zero coordinates. A compatible cocone on these finite [biproducts](../../../category-theory.md#biproduct) is exactly a family of maps from every $A_i$, so their directed [colimit](../../../category.md#colimit) is $S=\coprod_{i\in I}A_i$.

Each finite [biproduct](../../../category-theory.md#biproduct) has a map $k_J:S_J\to P=\prod_{i\in I}A_i$ using its coordinates in $J$ and zeros outside $J$. Projection to the finite set of coordinates in $J$ is a retraction, so $k_J$ is a [split monomorphism](../../../category.md#split-monomorphism). These maps form a cocone of [monomorphisms](../../../category.md#monomorphism). The finitary property makes its induced map a [monic arrow](../../../category.md#monomorphism), and that induced map is exactly the canonical infinite identity matrix:

$$
\boxed{j:\coprod_{i\in I}A_i\longrightarrow\prod_{i\in I}A_i\text{ is monic}.}
$$

This proves the [coproduct-to-product comparison in a finitary abelian category](../../../category-theory.md#coproduct-to-product-comparison-in-a-finitary-abelian-category). The PDF's use of finite [products in a category](../../../category.md#product-category-theory) in the hint is valid because these are the same finite [biproducts](../../../category-theory.md#biproduct).

If $\mathcal A$ is also a [cofinitary abelian category](../../../category-theory.md#cofinitary-abelian-category), apply this argument in its opposite [category](../../../category.md). The same canonical comparison $j$ is then an [epic arrow](../../../category.md#epimorphism) in $\mathcal A$. In an [abelian category](../../../category-theory.md#abelian-category) an arrow that is both a [monomorphism](../../../category.md#monomorphism) and an [epimorphism](../../../category.md#epimorphism) is invertible, so $j$ is an isomorphism.

For countably many copies of $A$, put $S=\coprod_{n\geq0}A$ and let $q=j^{-1}\Delta:A\to S$, where $\Delta$ is the [product in a category](../../../category.md#product-category-theory) diagonal. Let $\iota_n$ denote the [coproduct in a category](../../../category.md#coproduct) injections, let $s:S\to S$ shift them by $s\iota_n=\iota_{n+1}$, and let $\nabla:S\to A$ be the codiagonal. Comparing every [product in a category](../../../category.md#product-category-theory) coordinate gives

$$
jq=j\iota_0+jsq.
$$

Since $j$ is a [monic arrow](../../../category.md#monomorphism), $q=\iota_0+sq$. Also $\nabla\iota_0=1_A$ and $\nabla s=\nabla$. Therefore, for $z=\nabla q$,

$$
z=1_A+z.
$$

[Hom-sets](../../../category.md#hom-set) are [abelian groups](../../../group.md#abelian-group), so cancellation gives $1_A=0$. Any arrow to or from $A$ is consequently zero by composition with its identity. Thus every object is both initial and terminal, and

$$
\boxed{\mathcal A\text{ is degenerate: every object is a zero object}.}
$$

This is the countable shift-and-fold argument behind [countable biproducts in an additive category force triviality](../../../category-theory.md#countable-biproducts-in-an-additive-category-force-triviality).

## 6

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [monoidal category](../../../category-theory.md#monoidal-category) consists of a [category](../../../category.md) $\mathcal C$, a bifunctor $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a unit object $I$, and [natural isomorphisms](../../../category.md#natural-isomorphism)

$$
a_{X,Y,Z}:(X\otimes Y)\otimes Z\to X\otimes(Y\otimes Z),\quad
\lambda_X:I\otimes X\to X,\quad
\rho_X:X\otimes I\to X.
$$

The [associator](../../../category-theory.md#associator) and [unitors](../../../category-theory.md#unitor) satisfy the [pentagon identity for a monoidal category](../../../category-theory.md#pentagon-identity-for-a-monoidal-category) and [triangle identity for a monoidal category](../../../category-theory.md#triangle-identity-for-a-monoidal-category)

$$
\begin{aligned}
a_{W,X,Y\otimes Z}\,a_{W\otimes X,Y,Z}
&=(1_W\otimes a_{X,Y,Z})\,a_{W,X\otimes Y,Z}\,(a_{W,X,Y}\otimes1_Z),\\
(1_X\otimes\lambda_Y)a_{X,I,Y}&=\rho_X\otimes1_Y.
\end{aligned}
$$

All compositions here have the displayed parenthesized sources and targets; no strictness assumption is being made.

The [monoidal coherence theorem](../../../category-theory.md#monoidal-coherence-theorem) says that between two formal tensor expressions having the same ordered list of letters after deletion of formal units, every map made from [associators](../../../category-theory.md#associator), [unitors](../../../category-theory.md#unitor), their inverses, identities, tensor [products in a category](../../../category.md#product-category-theory) and compositions is the same. Thus every diagram of such structural maps commutes. It does not permit permutation of letters or identify different additional maps such as braidings.

We prove this by canonical normalization. We first derive three necessary unit identities from the axioms, avoiding a circular appeal to coherence:

$$
\rho_{X\otimes Y}=(1_X\otimes\rho_Y)a_{X,Y,I},\qquad
\lambda_{X\otimes Y}a_{I,X,Y}=\lambda_X\otimes1_Y,\qquad
\lambda_I=\rho_I.
$$

For the first identity, take the pentagon on $X,Y,I,Z$ and postcompose by $1_X\otimes(1_Y\otimes\lambda_Z)$. [Naturality](../../../category.md#naturality) of $a$ and the triangle identify its left-hand path as $a_{X,Y,Z}(\rho_{X\otimes Y}\otimes1_Z)$; they identify its right-hand path as

$$
a_{X,Y,Z}\bigl(((1_X\otimes\rho_Y)a_{X,Y,I})\otimes1_Z\bigr).
$$

Cancel $a_{X,Y,Z}$. Taking $Z=I$ permits cancellation of the operation $-\otimes I$, since the [natural isomorphism](../../../category.md#natural-isomorphism) $\rho$ makes that [functor](../../../category.md#functor) faithful. This proves the first identity. The identical argument with tensor order reversed, [associator](../../../category-theory.md#associator) reversed and left and right [unitors](../../../category-theory.md#unitor) exchanged proves the second. Finally, [naturality](../../../category.md#naturality) of $\lambda$ at the map $\lambda_X:I\otimes X\to X$ gives $\lambda_{I\otimes X}=1_I\otimes\lambda_X$, after cancellation of $\lambda_X$. Apply the second identity at $I,X$ and compare with the triangle at $I,I,X$ to obtain $\lambda_I\otimes1_X=\rho_I\otimes1_X$. Set $X=I$ and use the same faithfulness to conclude $\lambda_I=\rho_I$. This establishes the [unit identities derived from the monoidal pentagon and triangle](../../../category-theory.md#unit-identities-derived-from-the-monoidal-pentagon-and-triangle).

For an ordered word $u$, define a right-associated normal tensor, including a terminal unit, by

$$
N(\varnothing)=I,\qquad N(Au)=A\otimes N(u).
$$

Define canonical concatenation maps $c_{u,v}:N(u)\otimes N(v)\to N(uv)$ recursively:

$$
c_{\varnothing,v}=\lambda_{N(v)},\qquad
c_{Au,v}=(1_A\otimes c_{u,v})a_{A,N(u),N(v)}.
$$

All these maps are invertible. The derived unit identities give, by induction on $u$,

$$
c_{u,\varnothing}=\rho_{N(u)}.
$$

The empty base case is $\lambda_I=\rho_I$; the induction step is exactly the right-unitor identity above.

A second induction, again on $u$, proves the concatenation identity

$$
c_{uv,w}(c_{u,v}\otimes1_{N(w)})
=c_{u,vw}(1_{N(u)}\otimes c_{v,w})a_{N(u),N(v),N(w)}.
$$

For $u=\varnothing$, [naturality](../../../category.md#naturality) of $\lambda$ and $\lambda_{X\otimes Y}a_{I,X,Y}=\lambda_X\otimes1_Y$ give the equality. For $u=Au'$, expand each occurrence with first word beginning in $A$ by the recursive formula. [Naturality](../../../category.md#naturality) moves the maps $c_{u',v}$ and $c_{v,w}$ through the [associators](../../../category-theory.md#associator). The two paths of [associators](../../../category-theory.md#associator) on $A,N(u'),N(v),N(w)$ agree by the pentagon; the remaining maps inside the factor $A\otimes-$ agree by the induction hypothesis for $u'$. This proves the concatenation identity for every triple of words, including empty words.

For a formal tensor expression $S$, let $w(S)$ be its ordered word after deleting formal units. Define an isomorphism $\nu_S:S\to N(w(S))$ recursively by

$$
\nu_A=\rho_A^{-1},\qquad \nu_I=1_I,\qquad
\nu_{S\otimes T}=c_{w(S),w(T)}(\nu_S\otimes\nu_T).
$$

Here the first case means a formal letter $A$, and the second means the distinguished formal unit. Applying the concatenation identity and [naturality](../../../category.md#naturality) of $a$ gives

$$
\nu_{S\otimes(T\otimes U)}a_{S,T,U}=\nu_{(S\otimes T)\otimes U}.
$$

Similarly, [naturality](../../../category.md#naturality) of the [unitors](../../../category-theory.md#unitor) and the two empty-word concatenation identities give

$$
\nu_S\lambda_S=\nu_{I\otimes S},\qquad
\nu_S\rho_S=\nu_{S\otimes I}.
$$

Thus normalization commutes with each generating [associator](../../../category-theory.md#associator) or [unitor](../../../category-theory.md#unitor). It also commutes with their inverses. The recursive tensor formula shows the same for a generating map applied inside any larger tensor expression, and composition preserves the property. Consequently every structural map $g:S\to T$ satisfies $\nu_Tg=\nu_S$, whence

$$
\boxed{g=\nu_T^{-1}\nu_S.}
$$

This depends only on the source and target expressions, so any two structural paths agree. That proves coherence, including all insertions and removals of units, by the [word normalization proof of monoidal coherence](../../../category-theory.md#word-normalization-proof-of-monoidal-coherence).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
