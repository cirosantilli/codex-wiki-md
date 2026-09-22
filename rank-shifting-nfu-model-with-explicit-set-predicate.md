# Rank-shifting NFU model with explicit set predicate

↑ **Parent:** [Rank-shifting automorphism construction of NFU](rank-shifting-automorphism-construction-of-nfu.md)

Let $M$ be a membership structure satisfying [extensionality](axiom-of-extensionality.md) and every pure-membership separation instance, with an external automorphism $j$ and domains $D_i=j^i(D_0)$ represented by objects of $M$. Suppose every $M$-subset of $D_i$ is an element of $D_{i+1}$. Interpret [NFU](new-foundations-with-urelements.md) on the objects of $D_0$ using the displayed [set](set-split.md) predicate and membership, with all [subset](subset.md) statements evaluated in $M$. Atoms have no members, and [extensionality](axiom-of-extensionality.md) applied to $j(y),j(z)\subseteq D_0$ gives [extensionality](axiom-of-extensionality.md) for [sets](set-split.md). A [stratified formula](stratified-formula.md) becomes an ordinary pure-membership formula by sending each variable of type $i$ to $j^i(x)$ and restricting its quantifier to $D_i$. A [set](set-split.md) predicate on sort $i$ means containment in $D_{i-1}$; adjacent-sort membership is guarded by containment in the lower domain. Separation yields the extension $X\subseteq D_i$, the closure hypothesis places it in $D_{i+1}$, and $j^{-(i+1)}(X)\in D_0$ is the required untyped [set](set-split.md). This proves every comprehension instance. The guard is essential: an object not contained in a lower domain can still have some ordinary members there, which must not become members of a typed atom. Internal ranks $V_{j^i(\alpha)}$ with $j(\alpha)>\alpha$ give one instance of these hypotheses; shifted rank objects in an elementary model of an expanded $V_{\omega+\omega}$ give a consistency proof without assuming Con([ZFC](zermelo-fraenkel-set-theory-with-choice.md)).

**Table of contents**

- [Rank-indiscernible construction of an NFU model](rank-indiscernible-construction-of-an-nfu-model.md)

## ↑ Ancestors (9)

1. [Rank-shifting automorphism construction of NFU](rank-shifting-automorphism-construction-of-nfu.md)
2. [Type-shifting automorphism](type-shifting-automorphism.md)
3. [New Foundations with urelements](new-foundations-with-urelements.md)
4. [New Foundations](new-foundations.md)
5. [Set theory](set-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19/6/solution.md)
