<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [first-order structure](../../../../../first-order-structure.md) consists of a nonempty domain $A$, an interpretation $c^A\in A$ of each [constant symbol](../../../../../constant-symbol.md), a total function $f^A:A^n\to A$ for each $n$-ary [function symbol](../../../../../function-symbol.md), and a relation $R^A\subseteq A^n$ for each $n$-ary [predicate symbol](../../../../../predicate-symbol.md). [Logical equality](../../../../../logical-equality.md) is interpreted as actual identity.

An [assignment in a first-order structure](../../../../../assignment-in-a-first-order-structure.md) is a map $s$ from the variables into $A$. It extends recursively to terms: $x^A[s]=s(x)$, $c^A[s]=c^A$, and $f(t_1,\ldots,t_n)^A[s]=f^A(t_1^A[s],\ldots,t_n^A[s])$. Atomic truth is determined by membership of the resulting tuple in $R^A$, or equality of the two term values. [Negation](../../../../../negation.md) reverses the [truth value](../../../../../truth-value.md), and an implication is false exactly when its antecedent is true and its consequent false.

For a [universal quantifier](../../../../../universal-quantification.md),

$$
A,s\models\forall x\theta\quad\Longleftrightarrow\quad A,s[x\mapsto a]\models\theta\text{ for every }a\in A.
$$

These clauses define a valuation on every formula by [structural recursion](../../../../../structural-recursion.md). Only free-variable values affect a formula's truth; consequently a sentence has the same [truth value](../../../../../truth-value.md) under every assignment. This is a semantic assignment of domain elements, not a programming assignment operation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
