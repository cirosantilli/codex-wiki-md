<h1 id="a/2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $C$ denote the addition-commutativity [first-order sentence](../../../../../../first-order-sentence.md) and put $d=\ulcorner\neg C\urcorner$. In the ordinary checker for PA derivations, replace the axiom test $\operatorname{Ax}_{PA}(u)$ by

$$
\operatorname{Ax}_S(u)\equiv\operatorname{Ax}_{PA}(u)\vee u=\bar d.
$$

Keep all tests for sequence formation, earlier lines, logical axiom schemes and [inference rules](../../../../../../inference-rule.md) unchanged. This gives a [formal proof](../../../../../../formal-proof.md) checker $Q_S(u,w)$ which recognizes exactly ordinary $S$-derivations. The finite syntactic modification is arithmetizable by the same bounded coding apparatus as the original checker.

For the proof-order comparison in the next part, make the choice of coding explicit. Reserve code $0$ for the one-line derivation of the newly added axiom $\neg C$, and give an ordinary derivation with code $w$ the new code $w+1$. A corresponding bounded relation is

$$
\boxed{\operatorname{Prov}_S(u,v)\equiv
(v=0\wedge u=\bar d)\vee(\exists w\le v)(v=w+1\wedge Q_S(u,w)).}
$$

Every code has a specified decoding, every genuine [formal proof](../../../../../../formal-proof.md) is represented, and no false [formal proof](../../../../../../formal-proof.md) is admitted. The reserved code duplicates one genuine derivation, which is harmless. This is one explicit arithmetized [arithmetical proof relation](../../../../../../arithmetical-proof-relation.md) obtainable from the PA checker by the requested axiom change and a simple renumbering. Stating the proof-order convention matters because a Rosser [predicate symbol](../../../../../../predicate-symbol.md) uses code order, not merely the existence of [formal proofs](../../../../../../formal-proof.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../split.md)
7. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
