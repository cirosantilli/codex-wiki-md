<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

All consistency assertions here are relative: begin with a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), obtainable from a model of [ZF](../../../../../zermelo-fraenkel-set-theory.md) by its [constructible universe](../../../../../constructible-universe.md) as proved below. First use the [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md). Let $\pi$ exchange the old empty [set](../../../../../set-split.md) with its old singleton and fix every other object, and define

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

An old [set](../../../../../set-split.md) $b$ is the extension, in the new relation, of $\pi^{-1}(b)$. This immediately verifies extensionality and gives explicit representatives for the new empty [set](../../../../../set-split.md), pairs, unions and power [sets](../../../../../set-split.md): the old extensions required are respectively $\varnothing$, $\{a,b\}$, $\bigcup_{u\in\pi(a)}\pi(u)$, and $\{\pi^{-1}(c):c\subseteq\pi(a)\}$. Translate any formula by replacing membership by $E$; old separation and replacement then give the desired new subsets and functional ranges, whose representatives are obtained by $\pi^{-1}$.

For infinity, recursively form the new empty object $e=\pi^{-1}(\varnothing)$ and successors $s(x)=\pi^{-1}(\pi(x)\cup\{x\})$. The old replacement axiom collects the sequence $e,s(e),s^2(e),\ldots$; the representative of its range is a new inductive [set](../../../../../set-split.md). The old object $q=\varnothing$ has new extension $\pi(q)=\{q\}$, so $qEq$ and its singleton witnesses failure of the [Axiom of foundation](../../../../../axiom-of-regularity.md). Choice survives this full permutation construction: old choice applied to a family of nonempty new extensions selects its members, and new ordered pairs and a representative of their old [set](../../../../../set-split.md) give the new [choice function](../../../../../choice-function.md). Thus **$\mathsf{ZF}-\mathsf{Foundation}+\mathsf{AC}+\neg\mathsf{Foundation}$ is relatively consistent**. A well-founded starting model gives the opposite possibility for foundation.

To make choice fail, a symmetry restriction is essential. Here is an explicit pure-set construction with many [Quine atoms](../../../../../quine-atom.md). Take a countably infinite [set](../../../../../set-split.md) $A$ of distinct tagged objects $a_n$. Give $a_n$ the extension $\{a_n\}$. For every subset $S$ of objects already constructed, introduce an object $c(S)$ with extension $S$, except that $c(\{a_n\})$ is defined to be $a_n$ itself. Use a disjoint tag for all other codes $c(S)$, so identical extensions have identical codes and distinct extensions have distinct codes. Iterate this operation transfinitely, taking unions at limits. Each level is an old [set](../../../../../set-split.md), and its subsets are an old [set](../../../../../set-split.md), so this is a definable class construction. Every non-atomic membership edge decreases construction rank. Atomic edges are just the prescribed self-loops. Consequently the resulting structure is extensional, has the required pairs, unions and power [sets](../../../../../set-split.md), and the old replacement axiom bounds ranks of definable functional ranges. Its pure finite ranks supply infinity.

Every permutation of $A$ extends recursively by $c(S)\mapsto c(\sigma S)$. An object is finitely supported if some finite $F\subset A$ has the property that every permutation fixing $F$ pointwise fixes that object. Retain objects all of whose members, and members' members, are finitely supported, with recursion stopping at the atomic self-loops. Call this class $N$, the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md).

We must verify its [set](../../../../../set-split.md) axioms, not merely declare it a symmetric model. Empty [set](../../../../../set-split.md), pairs and unions have supports given by finite unions of the supports of their arguments. For separation, a formula with finitely supported parameters and domain $a$ is invariant under permutations fixing the union of those supports; its selected extension is therefore supported, and all its elements already lie in $N$. For power [set](../../../../../set-split.md), take all codes $c(S)$ with $S\subseteq\operatorname{ext}(a)$ and $c(S)\in N$. They form an old [set](../../../../../set-split.md), by separation from the bounded code level. Permutations fixing a support of $a$ permute this entire collection, so its code is supported and belongs to $N$. For replacement, translate the relativized formula to the original universe and use old replacement to collect its unique values. Equivariance gives this range a support from the parameters and domain, and every range element lies in $N$. Infinity uses the pure natural-number construction, fixed by every atom permutation. This proves $N\models\mathsf{ZF}-\mathsf{Foundation}$.

The [set](../../../../../set-split.md) $A$ and the collection of its two-element subsets have empty support and belong to $N$. Suppose the latter had a [choice function](../../../../../choice-function.md) $f\in N$, with finite support $F$. Choose distinct $a,b\in A\setminus F$. The transposition of $a,b$ fixes $F$, hence $f$, and fixes the unordered pair $\{a,b\}$. But it swaps whichever member $f(\{a,b\})$ selects, a contradiction. Therefore

$$
\boxed{N\models\neg\mathsf{AC}.}
$$

Together with the full permutation model satisfying choice, this proves **independence of choice from [ZF](../../../../../zermelo-fraenkel-set-theory.md) without foundation**, using the same replacement of atoms by self-membered pure [sets](../../../../../set-split.md). The negated-choice model also fails foundation; this suffices for independence over the foundation-free base.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
