<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Work inside a model $V$ of [ZF](../../../../../zermelo-fraenkel-set-theory.md). Let $\pi:V\to V$ be a definable class bijection, with definable inverse, so that its image and inverse image of every set are sets by [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md). Define new membership by

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

This is the [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md) convention used here. Its basic advantage is that every prescribed old set $b$ is the new extension of the object $\pi^{-1}(b)$. We verify the axioms rather than treating a membership permutation as automatically harmless.

The new [axiom of extensionality](../../../../../axiom-of-extensionality.md) follows because equality of the new extensions means $\pi(x)=\pi(y)$, hence $x=y$. The new empty set and unordered pair are $\pi^{-1}(\varnothing)$ and $\pi^{-1}(\{x,y\})$. Union and [power set](../../../../../power-set.md) are represented by

$$
\operatorname{Union}_E(a)=\pi^{-1}\left(\bigcup_{u\in\pi(a)}\pi(u)\right),\qquad \operatorname{Pow}_E(a)=\pi^{-1}\left(\{\pi^{-1}(b):b\subseteq\pi(a)\}\right).
$$

Indeed, the elements of the first object are exactly the new elements of new elements of $a$; the elements of the second are exactly the objects whose new extensions are subsets of $\pi(a)$.

Translate an arbitrary formula recursively by replacing each atomic $xEy$ by $x\in\pi(y)$. This is an ordinary definable formula in the old model. Old [axiom schema of separation](../../../../../axiom-schema-of-specification.md) forms any specified subclass $b$ of $\pi(a)$, and $\pi^{-1}(b)$ supplies the new separated set. Old [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) similarly collects the uniquely specified images of all elements of $\pi(a)$, and applying $\pi^{-1}$ supplies its new representative. This verifies the full schemas, including formulas with unbounded quantifiers.

For [axiom of infinity](../../../../../axiom-of-infinity.md), define $e_0=\pi^{-1}(\varnothing)$ and

$$
e_{n+1}=\pi^{-1}\bigl(\pi(e_n)\cup\{e_n\}\bigr).
$$

Then $\pi(e_n)=\{e_0,\ldots,e_{n-1}\}$. These objects are distinct by induction: equality of $e_n$ with an earlier $e_m$ would equate old sets of respectively $n$ and $m$ distinct members. Old replacement collects $S=\{e_n:n\in\omega\}$, and $\pi^{-1}(S)$ is a new inductive set. Thus the construction satisfies **every axiom of [ZF](../../../../../zermelo-fraenkel-set-theory.md) except possibly [Axiom of foundation](../../../../../axiom-of-regularity.md)**.

Now interchange the old objects $\varnothing$ and $\{\varnothing\}$ and fix everything else. For $q=\varnothing$ we have $\pi(q)=\{q\}$, so its new sole member is itself: $q=\{q\}_E$. This [Quine atom](../../../../../quine-atom.md) contradicts [Axiom of foundation](../../../../../axiom-of-regularity.md). The identity permutation preserves the original model and its foundation. Hence, relative to consistency of [ZF](../../../../../zermelo-fraenkel-set-theory.md), **foundation is independent of the other ZF axioms**.

For the further independence result, a full permutation of a model of choice is insufficient. If the old model satisfies [axiom of choice](../../../../../axiom-of-choice.md), then for any new family $a$ of nonempty new sets, old choice selects $g(x)\in\pi(x)$ for every $x\in\pi(a)$. Encode its graph using the new ordered pairs, and represent that graph by $\pi^{-1}$. This is a new [choice function](../../../../../choice-function.md). We therefore add a hereditary finite-support restriction to a universe with many [Quine atoms](../../../../../quine-atom.md).

Start now with a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). Put $a_n=\omega+n$, and let $\pi$ interchange $a_n$ and $\{a_n\}$ for every $n\in\omega$, fixing other objects. All these transpositions are disjoint: the infinite [ordinals](../../../../../ordinal.md) $a_n$ are distinct and none is a singleton. In the resulting membership structure, $A=\{a_n:n\in\omega\}$ is an infinite family of [Quine atoms](../../../../../quine-atom.md).

Build its universe $W$ by the internal transfinite hierarchy

$$
W_0=A,\qquad W_{\alpha+1}=A\cup\{\pi^{-1}(b):b\subseteq W_\alpha\},\qquad W_\lambda=\bigcup_{\alpha<\lambda}W_\alpha.
$$

Write $W$ for the union over the old [ordinals](../../../../../ordinal.md). Apart from the atomic self-loops, an object's new members have lower construction ranks. Every permutation $\sigma$ of $A$ therefore extends recursively to $W$: on atoms use the prescribed permutation, and on other objects put

$$
\widehat\sigma(x)=\pi^{-1}\bigl(\widehat\sigma\,``\pi(x)\bigr).
$$

This is well defined and preserves $E$. A nonatom cannot be sent to an atom, since an extension consisting solely of one atom already represents that atom. Recursing with $\sigma^{-1}$ gives the inverse, so these maps are genuine automorphisms.

Say that $x$ has finite support $S\subseteq A$ if every such permutation fixing $S$ pointwise fixes $x$. Let $H$ consist of the atoms and the objects with finite support all of whose new members, recursively away from atomic self-loops, belong to $H$. This is the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md). We check why it still has the required set-theoretic axioms.

It is closed under taking new members, so extensionality remains valid. The empty object and the pure finite [ordinals](../../../../../ordinal.md) have empty support. Their internally represented infinite collection also has empty support, giving infinity. Pairs and unions use the finite unions of their constituents' supports; all their members remain hereditary members of $H$.

For a set $a\in H$, take all objects $b\in H$ whose new extensions are subsets of $\pi(a)$. They form an old set, since the unrestricted new [power set](../../../../../power-set.md) is an old set and membership in $H$ is definable. Its representative has support contained in a support of $a$, because an automorphism fixing $a$ permutes precisely these hereditary subsets. All its members belong to $H$. Hence this is the [power set](../../../../../power-set.md) required inside $H$, not a claim that unrestricted external subsets are retained.

For separation, relativize the formula to $H$. A support for $a$ together with supports of the finitely many parameters fixes the resulting subclass; its members are hereditary, so its representative belongs to $H$. For replacement, old replacement applied to this relativized definable functional relation collects the range. Its members have a common bound on their construction ranks, by taking the supremum of the set of ranks, so the range's representative lies in $W$. The same finite union of parameter and domain supports fixes the range by uniqueness of each image. It is therefore hereditary and belongs to $H$. These arguments verify the full schemas. Thus $H\models\mathrm{ZF}-\mathrm{Foundation}$.

Finally $A$ and the family of its two-element subsets belong to $H$ with empty support. Suppose a [choice function](../../../../../choice-function.md) $c$ for this family belongs to $H$, and let $S$ be a finite support for $c$. Choose distinct atoms $u,v\notin S$ and transpose them. This permutation fixes $c$ and fixes the unordered pair $\{u,v\}_E$, but interchanges its two possible selected members. Equivariance would require

$$
c(\{u,v\}_E)=\widehat\sigma\bigl(c(\{u,v\}_E)\bigr),
$$

which is impossible. Hence **choice fails in $H$**. Together with a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), or with its full permuted model satisfying choice and failing foundation, this proves independence of [axiom of choice](../../../../../axiom-of-choice.md) from [ZF](../../../../../zermelo-fraenkel-set-theory.md) minus foundation, relative to consistency of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). All hierarchy and support arguments are internal to the starting model; no transitive-model assumption is needed.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
