<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work in a ground [first-order model](../../../../../model-of-a-first-order-theory.md) of [set theory](../../../../../set-theory-split.md) satisfying [ZF](../../../../../zermelo-fraenkel-set-theory.md), and let $\pi$ be a definable [bijection](../../../../../bijection.md) of its universe, whose inverse is also definable. Write $\psi=\pi^{-1}$ and replace membership by

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

In this [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md), an object having prescribed extension $b$ is represented by $\psi(b)$. The [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) in the ground model guarantees that images of [sets](../../../../../set-split.md) under $\pi$ and $\psi$ are [sets](../../../../../set-split.md). The [axiom of extensionality](../../../../../axiom-of-extensionality.md) follows from injectivity of $\pi$; the new [empty set](../../../../../empty-set.md) is $\psi(\varnothing)$, and the new pair of $x,y$ is $\psi(\{x,y\})$.

For the [Axiom of union](../../../../../axiom-of-union.md) and [Axiom of power set](../../../../../axiom-of-power-set.md), representatives are respectively

$$
\psi\left(\bigcup_{y\in\pi(x)}\pi(y)\right),\qquad
\psi\left(\{\psi(s):s\subseteq\pi(x)\}\right).
$$

Indeed, $z$ is an $E$-subset of $x$ exactly when $\pi(z)\subseteq\pi(x)$. Translate every [first-order formula](../../../../../first-order-formula.md) by replacing membership with membership in $\pi(y)$. Ground [separation](../../../../../axiom-schema-of-specification.md) then forms each desired subextension of $\pi(x)$, and ground [replacement](../../../../../axiom-schema-of-replacement.md) forms each functional image; applying $\psi$ supplies its representative. To verify the [axiom of infinity](../../../../../axiom-of-infinity.md), define by ground recursion

$$
a_0=\psi(\varnothing),\qquad a_{n+1}=\psi(\pi(a_n)\cup\{a_n\}).
$$

Then $\psi(\{a_n:n<\omega\})$ is an $E$-inductive [set](../../../../../set-split.md). Thus every [ZF](../../../../../zermelo-fraenkel-set-theory.md) axiom except possibly the [Axiom of foundation](../../../../../axiom-of-regularity.md) survives.

Interchange two distinct objects $a$ and $\{a\}$, fixing everything else. Then $\pi(a)=\{a\}$, so $a$ is a [Quine atom](../../../../../quine-atom.md): internally $a=\{a\}$. The nonempty [set](../../../../../set-split.md) $a$ has no member disjoint from itself, violating the [Axiom of foundation](../../../../../axiom-of-regularity.md). The original membership model satisfies that axiom. **[Foundation](../../../../../axiom-of-regularity.md) is therefore relatively independent of the other [ZF](../../../../../zermelo-fraenkel-set-theory.md) axioms.**

A full [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md) of a choice model still satisfies the [axiom of choice](../../../../../axiom-of-choice.md): choose an old member of each nonempty extension $\pi(y)$ and encode the resulting choice graph with the new ordered-pair operations. To obtain failure of choice, an additional restriction by symmetries is necessary.

Start instead with [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) and use the definable permutation interchanging every $a_n=\omega+n$ with $\{a_n\}$. These transpositions are disjoint and produce an [infinite set](../../../../../infinite-set.md) $A$ of [Quine atoms](../../../../../quine-atom.md). Inside the resulting membership model build the cumulative universe over $A$, closing at successive stages under [sets](../../../../../set-split.md) of previously constructed objects, represented by $\psi(X)$. Atomic objects are kept as the designated base objects; $\psi(\{a\})=a$ for $a\in A$. Every permutation of $A$ extends recursively to an automorphism of this universe, with the atomic self-loops fixed by the recursive convention.

An object has [finite support](../../../../../finite-support-in-a-permutation-action.md) if every permutation fixing some finite $S\subseteq A$ pointwise fixes it. Retain the objects which have [finite support](../../../../../finite-support-in-a-permutation-action.md) and whose members recursively also have [finite support](../../../../../finite-support-in-a-permutation-action.md), interpreting the atomic self-loops as the base case. This is the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md). It is transitive for the new membership relation. [Extensionality](../../../../../axiom-of-extensionality.md) is inherited. Pairs and [unions](../../../../../set-union.md) have supports contained in the [union](../../../../../set-union.md) of the finitely many relevant supports. For a supported [set](../../../../../set-split.md) $x$, the collection of all retained [subsets](../../../../../subset.md) of $x$ is a ground [set](../../../../../set-split.md), by the full model's [power set](../../../../../power-set.md) axiom, and is fixed by every permutation fixing a support of $x$. Its members are retained, so this collection supplies the internal [power set](../../../../../power-set.md). A [first-order formula](../../../../../first-order-formula.md) with retained parameters is invariant under their common stabilizer. Consequently its definable [subset](../../../../../subset.md) of $x$, and the range of a functional relation on $x$, have that same [finite support](../../../../../finite-support-in-a-permutation-action.md); ground [separation](../../../../../axiom-schema-of-specification.md) and [replacement](../../../../../axiom-schema-of-replacement.md) first ensure that they are [sets](../../../../../set-split.md). The pure natural-number hierarchy supplies [infinity](../../../../../infinity.md). These arguments verify all of [ZF](../../../../../zermelo-fraenkel-set-theory.md) except [Axiom of foundation](../../../../../axiom-of-regularity.md), which fails at the [Quine atoms](../../../../../quine-atom.md).

The family $[A]^2$ of all two-element [subsets](../../../../../subset.md) is retained and has empty support. If it had a retained choice [function](../../../../../function-split.md) $f$, choose two distinct [Quine atoms](../../../../../quine-atom.md) $a,b$ outside a [finite support](../../../../../finite-support-in-a-permutation-action.md) of $f$. The transposition of $a,b$ fixes $f$ and fixes the unordered pair $\{a,b\}$, but moves either possible value $f(\{a,b\})$. This is impossible. Thus **[ZF](../../../../../zermelo-fraenkel-set-theory.md) without [Foundation](../../../../../axiom-of-regularity.md) has both choice models and models in which Choice fails**, relative to the usual consistency assumption. The construction also explains why twisting membership alone was insufficient.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
