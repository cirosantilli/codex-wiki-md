<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The assertions are relative independence results. We construct countermodels in a background model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md); if [ZF](../../../../../zermelo-fraenkel-set-theory.md) is consistent, its [constructible universe](../../../../../constructible-universe.md) gives a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) as well. The original model satisfies [foundation](../../../../../axiom-of-regularity.md) and [choice](../../../../../axiom-of-choice.md), supplying the positive sides.

For failure of [foundation](../../../../../axiom-of-regularity.md), use a [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md). Let $\pi$ interchange the old $\varnothing$ and $\{\varnothing\}$ and fix every other object, and put $x\mathrel E y$ iff $x\in\pi(y)$. The new extension of $y$ is the old set $\pi(y)$, so the representative of any old extension $b$ is $\pi^{-1}(b)$. Bijectivity gives [extensionality](../../../../../axiom-of-extensionality.md). Translate formulas recursively by this definition of $E$. Old [separation](../../../../../axiom-schema-of-specification.md) gives each new definable subset, and old [replacement](../../../../../axiom-schema-of-replacement.md) gives each new functional range; apply $\pi^{-1}$ to the resulting extension to obtain its new representative.

Explicitly, a new pair is represented by $\pi^{-1}(\{x,y\})$; the new union of $a$ is represented by $\pi^{-1}(\bigcup_{x\in\pi(a)}\pi(x))$; and the new [power set](../../../../../power-set.md) of $a$ is represented by

$$
\pi^{-1}\bigl(\{\pi^{-1}(b):b\subseteq\pi(a)\}\bigr).
$$

Starting from the new empty set, iterate the new successor and collect these iterates by old [replacement](../../../../../axiom-schema-of-replacement.md), obtaining an [inductive set](../../../../../inductive-set.md). The old [axiom of choice](../../../../../axiom-of-choice.md) selects a member from each nonempty extension and thereby gives new choice functions. However the old object $q=\varnothing$ now satisfies $q\mathrel E q$ and has exactly itself as its member: it is a [Quine atom](../../../../../quine-atom.md). Its new singleton has no $E$-minimal member, so [foundation](../../../../../axiom-of-regularity.md) fails.

To make [choice](../../../../../axiom-of-choice.md) fail, retain infinitely many [Quine atoms](../../../../../quine-atom.md) $A=\{a_n:n<\omega\}$ and impose a finite-support symmetry restriction. A precise background construction uses tagged set codes. Each atom $a$ has extension $\{a\}$. For every other set of available objects $S$, introduce a unique ordinary set code with extension $S$, except that $S=\{a\}$ is already represented by $a$ itself. Iterate this construction through the [ordinals](../../../../../ordinal.md). Omitting the duplicate singleton codes makes the resulting relation extensional. Every permutation of $A$ extends to an [automorphism](../../../../../automorphism.md) of this universe by recursion through its ordinary codes.

An object has [finite support](../../../../../finite-support-in-a-permutation-action.md) if some finite $S\subseteq A$ has the property that every permutation fixing $S$ pointwise fixes that object. Retain the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md): the object and every object reached through its membership relation must have finite support. The atomic self-loops are permitted. The atom set $A$ and all pure sets are retained.

The union of supports for a domain and finitely many parameters supports any definable subset or functional image: every permutation fixing those supports preserves the defining formula. Members of the subset or image are already hereditary, so this verifies [separation](../../../../../axiom-schema-of-specification.md) and [replacement](../../../../../axiom-schema-of-replacement.md). The collection of all retained subsets of a retained set is invariant under any permutation fixing that set's support, and each of its members is hereditary; this verifies the [Axiom of power set](../../../../../axiom-of-power-set.md). Pairs and unions have the union of the requisite finite supports, and the pure natural-number hierarchy verifies [infinity](../../../../../infinity.md). The coding still verifies [extensionality](../../../../../axiom-of-extensionality.md).

If a choice function on all two-element subsets of $A$ had finite support $S$, choose distinct $a,b\notin S$. The transposition of $a,b$ fixes $S$ and the unordered pair $\{a,b\}$, but moves either possible chosen value. This contradicts invariance of the function. Hence [choice](../../../../../axiom-of-choice.md) fails, while a [Quine atom](../../../../../quine-atom.md) witnesses failure of [foundation](../../../../../axiom-of-regularity.md). We have a model of $\mathrm{ZF}-\mathrm{Foundation}+\neg\mathrm{Choice}$. Together with the original model this proves the required independence of [choice](../../../../../axiom-of-choice.md) over $\mathrm{ZF}-\mathrm{Foundation}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
