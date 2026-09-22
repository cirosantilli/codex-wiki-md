<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md) changes membership, not the underlying domain. In a model $M$ of [ZF](../../../../../zermelo-fraenkel-set-theory.md), let $\pi$ be a definable class bijection, with parameters allowed, and define

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

Every old set $b$ is the new extension of precisely the object $\pi^{-1}(b)$. Translation of formulas replaces each membership assertion by this definable relation. Both images and inverse images of old sets under $\pi$ are sets by [replacement](../../../../../axiom-schema-of-replacement.md).

Here are the axiom checks. [Extensionality](../../../../../axiom-of-extensionality.md) follows because equal new extensions mean $\pi(x)=\pi(y)$ and hence $x=y$. The new empty set is $\pi^{-1}(\varnothing)$ and the new pair is $\pi^{-1}(\{x,y\})$. For an object $a$, new union and [power set](../../../../../power-set.md) have representatives

$$
\pi^{-1}\left(\bigcup_{z\in\pi(a)}\pi(z)\right),\qquad
\pi^{-1}\left(\{\pi^{-1}(b):b\subseteq\pi(a)\}\right).
$$

These formulas verify the actual new membership conditions. A definable subset of the new extension $\pi(a)$ is an old set by [separation](../../../../../axiom-schema-of-specification.md) after translation, and its representative gives new [separation](../../../../../axiom-schema-of-specification.md). Similarly, a functional new formula on that extension has an old set as range by [replacement](../../../../../axiom-schema-of-replacement.md); apply $\pi^{-1}$ to its range. For infinity, iterate the new successor operation

$$
s_E(x)=\pi^{-1}\bigl(\pi(x)\cup\{x\}\bigr)
$$

starting from the new empty set. Old recursion and [replacement](../../../../../axiom-schema-of-replacement.md) collect its finite iterates into a set $B$, and $\pi^{-1}(B)$ is a new inductive set. Thus all axioms of [ZF](../../../../../zermelo-fraenkel-set-theory.md) except possibly foundation hold.

Now swap the old objects $0=\varnothing$ and $1=\{0\}$ and fix everything else. The old object $0$ then satisfies $0\mathrel E0$, and its entire new extension is $\{0\}$. It is a [Quine atom](../../../../../quine-atom.md), so foundation fails. Taking $\pi$ to be the identity gives the original model where foundation holds. **Foundation is independent of the other [ZF](../../../../../zermelo-fraenkel-set-theory.md) axioms**, relative to consistency of [ZF](../../../../../zermelo-fraenkel-set-theory.md).

A full permutation of a model of choice does not destroy choice. Given a new family of nonempty new sets, old choice selects an element of each old extension $\pi(y)$; [replacement](../../../../../axiom-schema-of-replacement.md) converts its graph into new ordered-pair coding. Thus simply repeating the preceding unrestricted permutation construction would not prove independence of choice. The extension needed is the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md).

Start with a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) and simultaneously swap $a_n=\omega+n$ with $\{a_n\}$ for all $n<\omega$. These transpositions have disjoint supports: none of these infinite [ordinals](../../../../../ordinal.md) is a singleton, and the [ordinals](../../../../../ordinal.md) and their singletons are separately distinct. Put $A=\{a_n:n<\omega\}$, whose members now have new extensions $\{a_n\}$. Build the universe over these [Quine atoms](../../../../../quine-atom.md) by allowing arbitrary new sets of previously constructed objects at each successor stage, and taking unions at limit stages. More explicitly, begin with $U_0=A$, put

$$
U_{\alpha+1}=A\cup\{\pi^{-1}(b):b\subseteq U_\alpha\},
\qquad U_\lambda=\bigcup_{\alpha<\lambda}U_\alpha,
$$

and take the union over all [ordinals](../../../../../ordinal.md). The singleton with sole member $a_n$ is already $a_n$, as [extensionality](../../../../../axiom-of-extensionality.md) requires; it is not added as a different atom or set. Every other object's membership has a well-founded construction rank once these designated atomic self-loops are treated as rank-zero leaves.

Every permutation $g$ of $A$ extends to an automorphism of this universe: on atoms use $g$, and on every non-atomic object recurse by

$$
\widehat g(x)=\pi^{-1}\{\widehat g(y):y\mathrel E x\}.
$$

The inverse permutation gives its inverse, and the formula preserves $E$. Call an object supported by a finite $S\subseteq A$ when every permutation fixing $S$ pointwise fixes that object. Retain only objects which are supported and all of whose members are hereditarily supported; the recursion here again stops at atoms, whose support is their singleton. Denote this class by $H$.

We verify that $(H,E)$ is a model of [ZF](../../../../../zermelo-fraenkel-set-theory.md) without foundation. It is membership-closed and hence retains [extensionality](../../../../../axiom-of-extensionality.md). Pairing uses the union of the two parameter supports, and union uses the support of its input. For [separation](../../../../../axiom-schema-of-specification.md), use the finite union of the supports of the domain and all parameters: permutations fixing them preserve satisfaction in $H$, so they fix the defined subset. Every member remains hereditary. For [replacement](../../../../../axiom-schema-of-replacement.md), the same support fixes the image of a definable functional relation; its elements already lie in $H$ by the internal range condition, and old [replacement](../../../../../axiom-schema-of-replacement.md) supplies the underlying set of them. These assertions are legitimate class translations because construction ranks, supports and hereditary support are definable in the starting model.

For [power set](../../../../../power-set.md), start with the set of all new subsets of a supported set and retain exactly those lying in $H$. The resulting collection is fixed by every permutation fixing the original set's support: the action preserves hereditary support and permutes its subsets. Every retained member is hereditary, so this is the internal [power set](../../../../../power-set.md). The empty set and the pure finite and infinite natural-number hierarchy have empty support, yielding infinity. The new pairing, union and comprehension representatives discussed above therefore remain inside $H$. Foundation still fails because all the [Quine atoms](../../../../../quine-atom.md) are in $H$.

The set $A$ itself has empty support and hereditary members. So does the family of its two-element subsets, each of which has a [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md). If this family had a choice function $f\in H$, let $S$ be a [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md) of $f$, and choose distinct $a,b\in A\setminus S$. The transposition of $a,b$ fixes $S$ and the unordered pair $\{a,b\}$, but interchanges either possible chosen value $f(\{a,b\})$. It cannot fix the function graph, contradicting its support. Thus **choice fails in $(H,E)$**.

The unrestricted permutation model over the same initial [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) model satisfies choice and fails foundation, whereas its hereditarily supported submodel fails both. Hence **choice is independent of [ZF](../../../../../zermelo-fraenkel-set-theory.md) with foundation omitted**. These are relative-consistency constructions, not an assertion that [ZF](../../../../../zermelo-fraenkel-set-theory.md) proves its own consistency. Starting with [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) is harmless for the usual consistency comparison with [ZF](../../../../../zermelo-fraenkel-set-theory.md), by the constructible-universe relative-consistency theorem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
