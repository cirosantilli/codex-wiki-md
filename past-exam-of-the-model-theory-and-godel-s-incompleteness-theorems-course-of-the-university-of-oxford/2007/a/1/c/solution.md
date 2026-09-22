<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Omega-consistency](../../../../../omega-consistency-of-an-arithmetic-theory.md) forbids a [logical formula](../../../../../logical-formula.md) $B(x)$ of any complexity for which $S\vdash\exists xB(x)$ and $S\vdash\neg B(\bar n)$ for every standard $n$. The difference from [one-consistency](../../../../../one-consistency.md) is that the matrix is unrestricted. It implies [first-order consistency](../../../../../first-order-consistency.md).

For a complete [first-order consistent](../../../../../first-order-consistency.md) classical [first-order theory](../../../../../first-order-theory.md), theorem membership obeys the ordinary Boolean [truth tables](../../../../../truth-table.md). For example, it proves a [conjunction](../../../../../conjunction-astronomy.md) exactly when it proves both conjuncts; completeness and [first-order consistency](../../../../../first-order-consistency.md) also make theoremhood of a [negation](../../../../../negation.md) the complement of theoremhood of the [first-order sentence](../../../../../first-order-sentence.md). [Omega-consistency](../../../../../omega-consistency-of-an-arithmetic-theory.md) additionally gives the witness property

$$
S\vdash\exists xB(x)\quad\Longleftrightarrow\quad
S\vdash B(\bar n)\text{ for some standard }n.
$$

The reverse implication is existential introduction. For the forward implication, if no standard instance were provable, completeness would give a [formal proof](../../../../../formal-proof.md) of each negated instance, violating [omega-consistency](../../../../../omega-consistency-of-an-arithmetic-theory.md). This works also after replacing additional [free variables](../../../../../free-variable.md) by numerals.

Now induct on [logical formulas](../../../../../logical-formula.md) with their remaining [free variables](../../../../../free-variable.md) replaced by standard numerals. At the atomic level, the equivalence between theoremhood and standard truth follows from [bounded completeness of an arithmetic theory](../../../../../bounded-completeness-of-an-arithmetic-theory.md) and bounded [soundness of an arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) from (b). The Boolean steps use the truth-table facts just proved. The existential step uses the witness property and the [induction](../../../../../mathematical-induction.md) hypothesis on its matrix; [universal quantification](../../../../../universal-quantification.md) follows by [negation](../../../../../negation.md). Hence

$$
\boxed{S\vdash X\quad\Longleftrightarrow\quad\mathbb N\models X}
$$

for every [first-order sentence](../../../../../first-order-sentence.md) $X$. Completeness ensures it decides each [first-order sentence](../../../../../first-order-sentence.md), and this equivalence ensures every decision is correct.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
