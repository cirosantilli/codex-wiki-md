<h1 id="b/6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Add a [predicate symbol](../../../../../predicate-symbol.md) $P_\theta$ for each $L$-formula $\theta(\vec x)$, of arity equal to its displayed free-variable [tuple](../../../../../finite-tuple.md). Let $T^+$ consist of $T$ together with all defining axioms

$$
\forall\vec x\ (P_\theta(\vec x)\leftrightarrow\theta(\vec x)).
$$

Every [first-order model](../../../../../model-of-a-first-order-theory.md) of $T$ has a unique such expansion, interpreting the new [predicate symbols](../../../../../predicate-symbol.md) by their defining [sets](../../../../../set-split.md). Conversely the reduct of every [first-order model](../../../../../model-of-a-first-order-theory.md) of $T^+$ satisfies $T$.

Given an arbitrary $L^+$-formula $\psi(\vec x)$, replace each new atomic [predicate symbol](../../../../../predicate-symbol.md) by its original $L$-definition, renaming [bound variables](../../../../../bound-variable.md) to avoid capture. This produces an $L$-formula $\psi^-(\vec x)$ with

$$
T^+\models\forall\vec x\ (\psi(\vec x)\leftrightarrow\psi^-(\vec x)).
$$

The defining axiom for that particular [logical formula](../../../../../logical-formula.md) now gives an atomic replacement:

$$
\boxed{T^+\models\forall\vec x\ (\psi(\vec x)\leftrightarrow P_{\psi^-}(\vec x)).}
$$

Thus the expanded [first-order theory](../../../../../first-order-theory.md) eliminates [quantifiers](../../../../../quantifier.md). For a [first-order sentence](../../../../../first-order-sentence.md), the same translation is an $L$-sentence, decided by completeness of $T$; hence every expanded [first-order sentence](../../../../../first-order-sentence.md) is decided and $T^+$ is complete. Empty free-variable [tuples](../../../../../finite-tuple.md) can be handled by zero-ary [predicate symbols](../../../../../predicate-symbol.md), or by the usual [logical truth](../../../../../logical-truth.md) and falsity constants. This definitional expansion is called [Morleyization](../../../../../morleyization.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
