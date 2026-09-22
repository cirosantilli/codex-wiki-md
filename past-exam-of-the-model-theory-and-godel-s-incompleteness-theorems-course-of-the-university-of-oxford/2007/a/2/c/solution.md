<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [logical formula](../../../../../logical-formula.md) $D(\vec x,y)$ weakly defines a total numerical [function](../../../../../function-split.md) $f$ in $S$ if, for every standard input [tuple](../../../../../finite-tuple.md) $\vec n$ and $m=f(\vec n)$,

$$
S\vdash D(\bar{\vec n},\bar m),\qquad
S\vdash\neg D(\bar{\vec n},\bar r)\quad(r\ne m).
$$

[Strong definability of a numerical function](../../../../../strong-definability-of-a-numerical-function.md) additionally requires the internal uniqueness statement

$$
S\vdash\forall y\,(D(\bar{\vec n},y)\to y=\bar m).
$$

Together with the positive instance, this is equivalent to proving $\forall y(D(\bar{\vec n},y)\leftrightarrow y=\bar m)$ for each standard input. The [universal quantifier](../../../../../universal-quantification.md) is the extra strength: it covers nonstandard potential outputs in [first-order models](../../../../../model-of-a-first-order-theory.md) of $S$. These are the weak and strong [function](../../../../../function-split.md) conventions used here. [Gödel's Incompleteness Theorems, printed page99, definition of weak and [strong definability of a numerical function](../../../../../strong-definability-of-a-numerical-function.md) of [functions](../../../../../function-split.md)](https://www.brucewatkins.org/math/docs/Smullyan.pdf)

Suppose the graph of the total [function](../../../../../function-split.md) is Sigma-1. Its complement is also Sigma-1, since

$$
f(\vec x)\ne y\quad\Longleftrightarrow\quad
\exists z\,(f(\vec x)=z\wedge z\ne y).
$$

Replace the graph assertion on the right by its Sigma-1 definition; [existential quantifiers](../../../../../existential-quantification.md) can be collected into one block. [Bounded completeness of an arithmetic theory](../../../../../bounded-completeness-of-an-arithmetic-theory.md) supplies numeralwise stage enumerators for each of these two disjoint complementary [sets](../../../../../set-split.md). Apply (b) to them. Its separating [logical formula](../../../../../logical-formula.md) is provable exactly at the required graph [tuples](../../../../../finite-tuple.md) in the positive direction and refutable at all the other standard [tuples](../../../../../finite-tuple.md), proving [weak definability of a numerical function](../../../../../weak-definability-of-a-numerical-function.md).

Using the graph [logical formula](../../../../../logical-formula.md) alone would only supply positive instances from true existential witnesses; the separation construction is what supplies the negative-instance [formal proofs](../../../../../formal-proof.md) without assuming [Sigma-1 soundness](../../../../../sigma-1-soundness.md) or completeness for false Sigma-1 statements.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
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
