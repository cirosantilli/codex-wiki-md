<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A sufficient condition is that $T$ be [first-order consistent](../../../../../first-order-consistency.md), complete, and full in its own [first-order language](../../../../../first-order-language.md). Work in the allowed function-free setting. Since $T$ proves the logically valid [first-order sentence](../../../../../first-order-sentence.md) $\exists x(x=x)$, fullness guarantees at least one constant and a nonempty collection of names.

Form the carrier from [equivalence classes](../../../../../equivalence-class.md) $[c]$ of [constant symbols](../../../../../constant-symbol.md) under

$$
c\sim d\quad\Longleftrightarrow\quad T\vdash c=d.
$$

[Logical equality](../../../../../logical-equality.md) logic makes this an [equivalence relation](../../../../../equivalence-relation.md). Interpret a constant by its class and interpret each relation symbol by

$$
R([c_1],\ldots,[c_n])\quad\Longleftrightarrow\quad
T\vdash R(c_1,\ldots,c_n).
$$

Substitution of equals makes this independent of representatives. This defines a [canonical first-order structure](../../../../../canonical-first-order-structure.md) because every carrier element is named by a constant.

The truth lemma, proved by [induction](../../../../../mathematical-induction.md) on [logical formulas](../../../../../logical-formula.md) with constants substituted for their [free variables](../../../../../free-variable.md), says

$$
\mathcal M\models\phi([\vec c])\quad\Longleftrightarrow\quad T\vdash\phi(\vec c).
$$

[Atomic formulas](../../../../../atomic-formula.md) hold by construction; completeness and [first-order consistency](../../../../../first-order-consistency.md) give the Boolean steps. For the existential step, a witness in the [first-order structure](../../../../../first-order-structure.md) is a named class, so its truth gives a proved instance and hence a proved [existential sentence](../../../../../existential-sentence.md). Conversely a proved [existential sentence](../../../../../existential-sentence.md) has a constant witness by fullness, and the [induction](../../../../../mathematical-induction.md) hypothesis realizes that instance in the [first-order structure](../../../../../first-order-structure.md). The universal case follows by [negation](../../../../../negation.md). Thus $\mathcal M\models T$, proving

$$
\boxed{\text{Consistent complete full theories have canonical first-order structures}.}
$$

The witness condition is needed in the original [first-order language](../../../../../first-order-language.md); adding new constants produces a [canonical first-order structure](../../../../../canonical-first-order-structure.md) in an expanded [first-order language](../../../../../first-order-language.md), which is a different assertion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
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
