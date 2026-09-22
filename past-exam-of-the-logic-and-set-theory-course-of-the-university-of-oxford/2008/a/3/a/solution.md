<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An $L$-structure consists of a nonempty domain $A$, an element $c^{\mathcal A}\in A$ for each [constant symbol](../../../../../constant-symbol.md), a [function](../../../../../function-split.md) $f^{\mathcal A}:A^n\to A$ for each $n$-ary [function symbol](../../../../../function-symbol.md), and a relation $R^{\mathcal A}\subseteq A^n$ for each $n$-ary [predicate symbol](../../../../../predicate-symbol.md). When [equality](../../../../../equality-mathematics.md) is part of the logic it is interpreted as actual identity on $A$.

An [assignment in a first-order structure](../../../../../assignment-in-a-first-order-structure.md) is a [function](../../../../../function-split.md) $s$ from [logical variables](../../../../../logical-variable.md) to $A$. It induces a [term valuation](../../../../../term-valuation.md) of [first-order terms](../../../../../first-order-term.md) recursively:

$$
x^{\mathcal A}[s]=s(x),\qquad c^{\mathcal A}[s]=c^{\mathcal A},\qquad
f(t_1,\ldots,t_n)^{\mathcal A}[s]=f^{\mathcal A}(t_1^{\mathcal A}[s],\ldots,t_n^{\mathcal A}[s]).
$$

For an [atomic formula](../../../../../atomic-formula.md), substitute these [first-order term](../../../../../first-order-term.md) values into the interpreted relation, or compare them for [equality](../../../../../equality-mathematics.md). Extend [satisfaction for a set structure](../../../../../satisfaction-for-a-set-structure.md) through the [truth tables](../../../../../truth-table.md) of the [logical connectives](../../../../../logical-connective.md), and through the [quantifier](../../../../../quantifier.md) clauses

$$
\mathcal A,s\models\forall x\theta\ \Longleftrightarrow\ (\forall a\in A)\ \mathcal A,s[x\mapsto a]\models\theta,
$$



$$
\mathcal A,s\models\exists x\theta\ \Longleftrightarrow\ (\exists a\in A)\ \mathcal A,s[x\mapsto a]\models\theta.
$$

Thus the [first-order structure](../../../../../first-order-structure.md) and [assignment in a first-order structure](../../../../../assignment-in-a-first-order-structure.md) together determine [truth values](../../../../../truth-value.md) for all [logical formulas](../../../../../logical-formula.md). A [first-order sentence](../../../../../first-order-sentence.md) has no [free variables](../../../../../free-variable.md), so its truth does not depend on the [assignment in a first-order structure](../../../../../assignment-in-a-first-order-structure.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
