<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work in a background model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). Each structure below satisfies every axiom of [ZF](../../../../../zermelo-fraenkel-set-theory.md) except the indicated one and falsifies that axiom; the background model supplies the other consistency direction.

For the [Axiom of union](../../../../../axiom-of-union.md), put $\lambda=\beth_\omega$ and use the [hereditarily locally small membership model](../../../../../hereditarily-locally-small-membership-model.md)

$$
B_\lambda=\{x:(\forall y\in\operatorname{TC}(\{x\}))\ |y|<\lambda\}.
$$

The [transitive class](../../../../../transitive-class.md) $B_\lambda$ inherits [extensionality](../../../../../axiom-of-extensionality.md) and [foundation](../../../../../axiom-of-regularity.md). Definable subsets of its sets remain in it. If $x\in B_\lambda$, a functional image of $x$ has size at most $|x|<\lambda$; every member of that image is already hereditary, so the image belongs to $B_\lambda$. This verifies [replacement](../../../../../axiom-schema-of-replacement.md), even though its values can have unbounded ranks. Also $|\mathcal P(x)|=2^{|x|}<\lambda$ by the [strong limit cardinal](../../../../../strong-limit-cardinal.md) property, and each subset of $x$ is locally small. This verifies the [Axiom of power set](../../../../../axiom-of-power-set.md). Pairing and [infinity](../../../../../infinity.md) follow similarly. But

$$
A=\{V_{\omega+n}:n<\omega\}\in B_\lambda,\qquad
\bigcup A=V_{\omega+\omega}\notin B_\lambda,
$$

since $|V_{\omega+n}|=\beth_n<\lambda$ while $|V_{\omega+\omega}|=\lambda$. This is failure of sumset without failure of [replacement](../../../../../axiom-schema-of-replacement.md) or [power set](../../../../../power-set.md).

For the [Axiom of power set](../../../../../axiom-of-power-set.md), use the [hereditarily countable sets](../../../../../hereditarily-countable-set.md) $H_{\omega_1}$. This is a [transitive class](../../../../../transitive-class.md). A countable union of countable [transitive closures](../../../../../transitive-closure.md) is countable, so it is closed under pairs, unions and functional images of its countable domains; these facts verify [pairing](../../../../../axiom-of-pairing.md), [union](../../../../../set-union.md) and [replacement](../../../../../axiom-schema-of-replacement.md). [Separation](../../../../../axiom-schema-of-specification.md), [foundation](../../../../../axiom-of-regularity.md) and [infinity](../../../../../infinity.md) also hold. Every subset of $\omega$ is hereditarily countable, but the full [power set](../../../../../power-set.md) $\mathcal P(\omega)$ is uncountable by [Cantor's theorem](../../../../../cantor-s-theorem.md) and cannot be a member of $H_{\omega_1}$. Since every candidate internal power set would have to contain all those subsets, the power-set axiom fails.

For [replacement](../../../../../axiom-schema-of-replacement.md), take the rank-initial [transitive set](../../../../../transitive-set.md) $V_{\omega+\omega}$. A limit rank contains the empty set and is closed under pairs, unions, subsets and power sets; it contains $\omega$, and [foundation](../../../../../axiom-of-regularity.md) and [extensionality](../../../../../axiom-of-extensionality.md) are inherited. Fix the parameter $V_\omega$. The definable map

$$
n\longmapsto\mathcal P^n(V_\omega)=V_{\omega+n}
$$

is internally described by a finite sequence of power-set iterations. Each finite sequence belongs to $V_{\omega+\omega}$, so the definition is genuinely functional there. Its range has rank $\omega+\omega$ and is not in the structure. Thus this instance of [replacement](../../../../../axiom-schema-of-replacement.md) fails.

For [extensionality](../../../../../axiom-of-extensionality.md), use the [non-extensional membership model with one atom](../../../../../non-extensional-membership-model-with-one-atom.md). Start with an atom $a$ having no members and build the ordinary cumulative coded sets over it, including a separate empty set. Interpret membership by the contents of a set code and give $a$ no members. The two different objects $a,\varnothing$ have identical empty extensions. [Foundation](../../../../../axiom-of-regularity.md) holds by the code ranks; pure finite ordinals give [infinity](../../../../../infinity.md); pairs, unions, definable subsets and functional ranges have their usual set codes. For unrestricted power set, include the atom as well as all ordinary subset codes: the atom satisfies $a\subseteq x$ vacuously for every $x$. This detail is necessary because the formulas here are the unmodified [ZF](../../../../../zermelo-fraenkel-set-theory.md) formulas, without a set predicate. The collection still has a set code, so the [Axiom of power set](../../../../../axiom-of-power-set.md) holds. All axioms except [extensionality](../../../../../axiom-of-extensionality.md) are satisfied.

Finally, $V_\omega$, the [hereditarily finite sets](../../../../../hereditarily-finite-set.md), satisfies every axiom except [infinity](../../../../../infinity.md). Pairs, unions, power sets and subsets of finite sets are finite, and every functional image of a finite domain is finite, so the full [replacement](../../../../../axiom-schema-of-replacement.md) schema holds. An [inductive set](../../../../../inductive-set.md) would contain every finite von Neumann ordinal and would be infinite, whereas every member of $V_\omega$ is finite. Hence [infinity](../../../../../infinity.md) fails.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
