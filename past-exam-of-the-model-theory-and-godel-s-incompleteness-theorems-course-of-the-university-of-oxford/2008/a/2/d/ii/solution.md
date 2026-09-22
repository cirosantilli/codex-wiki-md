<h1 id="a/2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [arithmetical proof relation](../../../../../../arithmetical-proof-relation.md) and coding just constructed. A [formal proof](../../../../../../formal-proof.md) of $C$ cannot have code $0$, since that code was reserved for $\neg C$. Every candidate code $v$ for a [formal proof](../../../../../../formal-proof.md) of $C$ is therefore positive. But code $0\le v$ is already a [formal proof](../../../../../../formal-proof.md) of $\neg C$, so the no-earlier-negation condition fails for every candidate. Hence

$$
\boxed{\mathbb N\models\neg\operatorname{Pr}_S^*(\ulcorner C\urcorner).}
$$

PA proves $C$ by [induction](../../../../../../mathematical-induction.md), while $S$ has $\neg C$ as an added axiom. Thus $S$ is inconsistent and its ordinary [arithmetical provability predicate](../../../../../../arithmetical-provability-predicate.md) is true of every [first-order sentence](../../../../../../first-order-sentence.md), including $C$. The displayed negative Rosser assertion can nevertheless be true, because the Rosser condition compares the order of opposite [formal proofs](../../../../../../formal-proof.md) rather than asking for their mere existence.

There is an important coding qualification. The PDF refers to a course [formal proof](../../../../../../formal-proof.md) coding but does not specify its numerical ordering. The truth of this Rosser assertion for an inconsistent [first-order theory](../../../../../../first-order-theory.md) is not coding-invariant, so [formal proof](../../../../../../formal-proof.md) length alone cannot establish it for an unspecified fixed coding. For example, a different legitimate numbering could reserve code $0$ for a known PA [formal proof](../../../../../../formal-proof.md) of $C$, code $1$ for the new axiom $\neg C$, and higher codes for all other derivations. Then code $0$ would witness $\operatorname{Pr}_S^*(\ulcorner C\urcorner)$ instead. The explicit allowed construction in part (i) supplies a convention under which the requested assertion holds; interpreting it as a claim about some externally fixed course numbering requires that numbering's corresponding [order property](../../../../../../order-property.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
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
