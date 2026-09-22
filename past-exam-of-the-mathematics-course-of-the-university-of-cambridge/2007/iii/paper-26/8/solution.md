<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Write $\mathsf{ZF}^-$ for [ZF](../../../../../zermelo-fraenkel-set-theory.md) with the [Axiom of foundation](../../../../../axiom-of-regularity.md) omitted. Independence is a relative-consistency assertion: from a model of ZFC we construct models of $\mathsf{ZF}^-+\neg\mathsf{Foundation}$, both with and without [axiom of choice](../../../../../axiom-of-choice.md). A model of ZFC itself supplies the positive cases.

First use a [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md). Inside the starting model choose a definable class bijection $\pi$ and put $xEy$ exactly when $x\in\pi(y)$. The new extension of $y$ is the old set $\pi(y)$, so any prescribed set of new members $b$ has representative $\pi^{-1}(b)$. We verify the axioms rather than treating the change of membership as automatically harmless.

The [axiom of extensionality](../../../../../axiom-of-extensionality.md) follows from injectivity of $\pi$. The new empty set is $\pi^{-1}(\varnothing)$ and a pair with members $a,b$ is $\pi^{-1}(\{a,b\})$. The union of a new set $x$ is represented by

$$
\pi^{-1}\left(\bigcup_{z\in\pi(x)}\pi(z)\right).
$$

A new subset $z$ of $x$ means $\pi(z)\subseteq\pi(x)$. Hence the new power set of $x$ is represented by

$$
\pi^{-1}\bigl(\{\pi^{-1}(b):b\subseteq\pi(x)\}\bigr).
$$

These are sets by the original power-set and replacement axioms. Translate each formula by replacing membership with $E$. The original [separation](../../../../../axiom-schema-of-specification.md) axiom extracts the required subset of $\pi(x)$, and replacement collects the range of a definable functional relation on $\pi(x)$; applying $\pi^{-1}$ gives their new representatives. Thus the full [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) and [separation](../../../../../axiom-schema-of-specification.md) schemes survive.

For [axiom of infinity](../../../../../axiom-of-infinity.md), start at $e=\pi^{-1}(\varnothing)$, iterate the new successor $s_E(x)=\pi^{-1}(\pi(x)\cup\{x\})$ along the old $\omega$, and take a new set representing this range. It contains the new empty set and is closed under the new successor. Finally, the old axiom of choice well-orders each old extension $\pi(x)$. Encode that relation using new ordered pairs and its new set representative. All subsets of the extension are represented in the new model, so this is genuinely a new well-order. Thus choice survives the full membership permutation.

Now transpose the old $\varnothing$ and $\{\varnothing\}$ and fix every other object. The old empty set $q=\varnothing$ satisfies $\pi(q)=\{q\}$, so its sole new member is itself: it is a [Quine atom](../../../../../quine-atom.md). The nonempty new set $q$ has no member disjoint from it, violating foundation. This gives $\boxed{\operatorname{Con}(\mathsf{ZFC})\Longrightarrow\operatorname{Con}(\mathsf{ZF}^-+\mathsf{AC}+\neg\mathsf{Foundation})}$. Together with the starting model, this proves independence of foundation.

For failure of choice, a membership permutation alone is insufficient, as the verification above shows. Add a symmetry restriction. Choose distinct old objects $a_n=\{\omega,n\}$ for $n<\omega$ and let $\pi$ simultaneously swap $a_n$ with $\{a_n\}$, fixing all other objects. The two families are disjoint, so this is a class bijection. Each $a_n$ is now a [Quine atom](../../../../../quine-atom.md). Write $A$ for the new set having precisely these atoms as members.

Every permutation of the atoms extends to an automorphism of the new universe, fixing its pure well-founded part. To construct it, send the atoms according to the prescribed permutation and, for any other object $x$, take the unique object whose new members are the images of its new members. This recursion is well founded away from the atomic self-loops: every other membership step decreases old rank, including the steps from the transposed singletons to their old extensions. Thus all the required automorphisms exist.

An object is supported by a finite set $F\subseteq A$ if every atom permutation fixing $F$ pointwise fixes it. Let $H$ consist of objects that have [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md) and all of whose new membership descendants also have [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md). This is the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md). The atoms belong to $H$, as does $A$ itself. We check that restricting $E$ to $H$ preserves $\mathsf{ZF}^-$.

Extensionality is inherited because every member of an object of $H$ is again in $H$. Empty sets, pairs and unions have supports obtained by taking finite unions of the supports of their parameters, and their descendants are already supported. The pure natural numbers and their set are fixed by every atom permutation, giving infinity. For [separation](../../../../../axiom-schema-of-specification.md), permutations fixing the domain and formula parameters preserve the defined subset, which therefore has their common [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md). For replacement, translate the relativized formula into the original universe and use original replacement to collect its unique values. Every value lies in $H$, and the range is invariant under the same [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md). Finally, the collection of all $H$-subsets of an object $x\in H$ is a subcollection of its full new power set, hence is a set in the original universe. Every permutation fixing a support of $x$ permutes these supported subsets, so this collection is supported; its members and their descendants lie in $H$. This verifies the internal power-set axiom. These arguments handle the full schemes with arbitrary finite tuples of parameters.

There is no choice function on the two-element subsets of $A$ in $H$. Suppose $f$ were one and had [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md) $F$. Choose distinct atoms $a,b\notin F$. The transposition exchanging them fixes $f$ and the unordered pair $\{a,b\}$, but exchanges its two possible selected values. Thus

$$
f(\{a,b\})=\tau(f(\{a,b\}))
$$

is impossible. The family of all such pairs belongs to $H$: it is invariant under every atom permutation and each pair has [finite support in a permutation action](../../../../../finite-support-in-a-permutation-action.md). Therefore $H\models\neg\mathsf{AC}$; it still contains the self-membered atoms, so it also fails foundation. We have proved

$$
\boxed{\operatorname{Con}(\mathsf{ZFC})\Longrightarrow\operatorname{Con}(\mathsf{ZF}^-+\neg\mathsf{AC}+\neg\mathsf{Foundation}).}
$$

The positive-choice permutation model and this negative-choice symmetry model establish independence of choice from $\mathsf{ZF}^-$. These constructions can be carried out internally in any starting model; no assumption of a transitive set model is needed.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
