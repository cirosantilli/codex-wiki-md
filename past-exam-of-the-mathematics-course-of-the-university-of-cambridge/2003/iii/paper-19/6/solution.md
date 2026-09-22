<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [complete type](../../../../../complete-type.md) over $A\subseteq M$ is a maximal consistent [set](../../../../../set-split.md) of [first-order formulas](../../../../../first-order-formula.md) in a fixed finite tuple of variables with parameters from $A$, consistent with the theory of that parameter expansion. A [first-order model](../../../../../model-of-a-first-order-theory.md) $M$ is a [saturated model](../../../../../saturated-model.md) of degree $\kappa$ if every such type with $|A|<\kappa$ is realized in $M$. It suffices to require this for one-variable types and realize a finite tuple successively. Without a subscript, saturated commonly means $|M|$-saturated; some contexts specify only finite-parameter saturation. We state the degree explicitly.

The [saturated elementary extension theorem](../../../../../saturated-elementary-extension-theorem.md) says that **every [first-order structure](../../../../../first-order-structure.md) has a $\kappa$-saturated [elementary extension](../../../../../elementary-extension.md) for any specified infinite $\kappa$**. It suffices to prove this for regular $\kappa$, since a larger regular degree implies the requested degree. At a single stage $M$, list all complete one-variable types over all [subsets](../../../../../subset.md) of $M$ of size below $\kappa$. This collection is a [set](../../../../../set-split.md). Adjoin a witness constant for each type to the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md) of $M$ and require that constant to satisfy its type. Every finite [subset](../../../../../subset.md) is satisfiable in $M$: each type's finite conjunction has a witness there, and the finitely many new constants have no cross-constraints. The [compactness theorem](../../../../../compactness-theorem.md) gives an [elementary extension](../../../../../elementary-extension.md) realizing all these types simultaneously.

Repeat this step along an elementary chain $(M_\alpha)_{\alpha<\kappa}$, taking [unions](../../../../../set-union.md) at limit stages, and let $N$ be its [union](../../../../../set-union.md). The [elementary chain theorem](../../../../../elementary-chain-theorem.md) follows here by induction on [first-order formulas](../../../../../first-order-formula.md): an existential statement true in the [union](../../../../../set-union.md) has a witness in a later stage; elementarity brings an existential witness back to the earlier stage containing its parameters. Thus each stage is elementary in $N$.

If $A\subseteq N$ has size below regular $\kappa$, all its elements lie in a single $M_\alpha$, by taking the [supremum](../../../../../supremum.md) of their fewer-than-$\kappa$ stage indices. Any [complete type](../../../../../complete-type.md) over $A$ consistent with $N$ is already consistent over $M_\alpha$, since these structures have the same parameter theory. It was therefore realized in $M_{\alpha+1}$. This proves $\kappa$-saturation of $N$.

A corresponding theorem about full saturation is available with a stated cardinal-size hypothesis: if $\lambda$ is uncountable regular, $|\mathcal L|<\lambda$, and $\lambda^{<\lambda}=\lambda$, then every infinite [first-order model](../../../../../model-of-a-first-order-theory.md) of size at most $\lambda$ has an [elementary extension](../../../../../elementary-extension.md) of size $\lambda$ which is $\lambda$-saturated. First adjoin $\lambda$ pairwise distinct constants to the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md); every finite fragment is satisfiable because the original [first-order model](../../../../../model-of-a-first-order-theory.md) is infinite. A [Skolem hull](../../../../../skolem-hull.md) of their realizations and the original domain has size $\lambda$. There are at most $\lambda$ small parameter [sets](../../../../../set-split.md) and at most $2^{|\mathcal L|+|A|+\aleph_0}\le\lambda$ types over each of them. Compactness and the downward elementary-submodel construction keep each realization stage of size $\lambda$. Taking a [Skolem hull](../../../../../skolem-hull.md) of the preceding stage and the chosen witnesses closes under at most $\lambda$ finite terms and proves this size bound and elementarity. The same length-$\lambda$ chain is consequently a fully [saturated model](../../../../../saturated-model.md) of size $\lambda$. The [cardinal](../../../../../cardinal-number.md) hypothesis is not silently asserted to hold for every [cardinal](../../../../../cardinal-number.md).

We now prove consistency of [NFU](../../../../../new-foundations-with-urelements.md) by the permitted alternative method of indiscernibles and a domain-shifting [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md). This can start from an explicit [set](../../../../../set-split.md) structure available in [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), so we need not assume that there is a [first-order model](../../../../../model-of-a-first-order-theory.md) of all [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). Let

$$
H=V_{\omega+\omega},\qquad F(n)=V_{\omega+n}\quad(n\in\omega),
$$

and give $F$ the value $\varnothing$ off the [natural numbers](../../../../../natural-number.md). Regard $(H,\in,F,\omega)$ as a [first-order structure](../../../../../first-order-structure.md), with a named object $\omega$. The graph of $F$ is an external [set](../../../../../set-split.md) in the metatheory; it need not be a member of $H$. This structure is extensional and satisfies every [separation](../../../../../axiom-schema-of-specification.md) instance in the pure membership language: any [subset](../../../../../subset.md) of $x\in H$ has rank below $\omega+\omega$ and belongs to $H$. It also satisfies, for natural $m<n$,

$$
\forall X\ (X\subseteq F(m)\Rightarrow X\in F(n)),
$$

since a [subset](../../../../../subset.md) of $V_{\omega+m}$ has rank at most $\omega+m$ and hence belongs to $V_{\omega+n}$.

Apply the indiscernible construction proved in question 7(i) to a [Skolem expansion](../../../../../skolem-expansion.md) of this [set](../../../../../set-split.md) structure, requiring $(c_i)_{i\in\mathbb Z}$ to be increasing members of its named natural-number object. For every finite fragment use an increasing [sequence](../../../../../sequence.md) of ordinary [natural numbers](../../../../../natural-number.md) in the initial structure in the Ramsey argument. The resulting generated elementary hull $M$ has an external [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) $j$ with $j(c_i)=c_{i+1}$, preserving $F$ and the named $\omega$. Put $D_i=F^M(c_i)$ and $D=D_0$. Then $j(D_i)=D_{i+1}$, and $M$ satisfies the displayed subset-containment assertion between successive domains. No claim that $M$ satisfies [replacement](../../../../../axiom-schema-of-replacement.md) is required.

All membership and [subset](../../../../../subset.md) statements about these objects are interpreted inside $M$. The hull is necessarily externally nonstandard: the natural-number objects $\ldots,c_{-2},c_{-1},c_0$ give an external descending chain. The external [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) is not an object that must be definable within that [first-order model](../../../../../model-of-a-first-order-theory.md).

On the external domain $D$ define

$$
\boxed{S(y)\iff M\models j(y)\subseteq D,\qquad
x\mathrel E y\iff S(y)\ \text{and}\ M\models x\in j(y).}
$$

This is the [rank-shifting NFU model with explicit set predicate](../../../../../rank-shifting-nfu-model-with-explicit-set-predicate.md). The guard $S(y)$ is essential: an object not contained in $D$ could still have some ordinary members in $D$, and must not thereby become a nonempty atom. The objects failing $S$ have no $E$-members. If two objects satisfying $S$ have the same $E$-members, their images under $j$ are [subsets](../../../../../subset.md) of $D$ with the same members, so [extensionality](../../../../../axiom-of-extensionality.md) in $M$ and injectivity of $j$ make the original objects equal. Thus set-extensionality and the atom condition hold.

It remains to prove every comprehension instance. Use the domains $D_i$ just constructed, equivalently $D_i=j^i(D)$, for integer sorts. The map $j$ is a [bijection](../../../../../bijection.md) from the objects of $D_i$ to the objects of $D_{i+1}$, and every [subset](../../../../../subset.md) of $D_i$ that exists in $M$ is an element of $D_{i+1}$. In sort $i$ define the [set](../../../../../set-split.md) predicate by $y\subseteq D_{i-1}$; from sort $i$ to $i+1$ define membership by ordinary membership guarded by $y\subseteq D_i$.

For a [stratified formula](../../../../../stratified-formula.md), assign integer types to its variables with equal types for equality and adjacent types for membership. Shift all types uniformly if necessary so the finitely many used types are nonnegative. Replace a variable of type $i$ by $j^i$ of its untyped value, quantify it over $D_i$, and use the typed relations just described. Applying $j^i$ to the untyped definition shows that each atomic [first-order formula](../../../../../first-order-formula.md) has the same truth value under this translation; induction on connectives and quantifiers proves the same for the whole [first-order formula](../../../../../first-order-formula.md). Importantly the translated [first-order formula](../../../../../first-order-formula.md) is an ordinary [first-order formula](../../../../../first-order-formula.md) of $M$ with finitely many domain and transformed-parameter constants, not a [first-order formula](../../../../../first-order-formula.md) containing the external [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) as a predicate.

If the comprehension variable has type $i$, [separation](../../../../../axiom-schema-of-specification.md) in $M$ produces its extension $X\subseteq D_i$. The subset-containment assertion gives $X\in D_{i+1}$. Put $y=j^{-(i+1)}(X)\in D$. Then $j(y)=j^{-i}(X)\subseteq D$, hence $S(y)$, and for every $x\in D$,

$$
x\mathrel E y\quad\Longleftrightarrow\quad j^i(x)\in X
\quad\Longleftrightarrow\quad\varphi(x).
$$

This verifies stratified comprehension with arbitrary parameters. The empty extension gives a distinguished [empty set](../../../../../empty-set.md); the always-true [first-order formula](../../../../../first-order-formula.md) gives a universal [set](../../../../../set-split.md). The unstratified Russell predicate is not an allowed comprehension instance. Thus

$$
\boxed{\mathsf{ZFC}\vdash\operatorname{Con}(\mathsf{NFU}).}
$$

Starting from the actual [set](../../../../../set-split.md) structure $H$ and applying compactness constructs a [set](../../../../../set-split.md) [first-order model](../../../../../model-of-a-first-order-theory.md), so this is a consistency proof in [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), not merely an assumption of Con([ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md)). It proves the requested consistency with an explicit interpretation; it does not depend on treating the much stronger full [extensionality](../../../../../axiom-of-extensionality.md) of NF as already consistent. The external $j$ is a tool of the construction, not an extra symbol permitted in [NFU](../../../../../new-foundations-with-urelements.md)'s comprehension scheme.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
