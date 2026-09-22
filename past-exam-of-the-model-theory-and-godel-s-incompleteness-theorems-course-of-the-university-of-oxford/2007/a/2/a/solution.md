<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [logical formula](../../../../../logical-formula.md) separates $A$ from $B$ in $S$ if it is provable at the standard numeral [tuple](../../../../../finite-tuple.md) of every member of $A$ and refutable at that of every member of $B$:

$$
\vec n\in A\Longrightarrow S\vdash F(\bar{\vec n}),\qquad
\vec n\in B\Longrightarrow S\vdash\neg F(\bar{\vec n}).
$$

There is no obligation on [tuples](../../../../../finite-tuple.md) outside the two [sets](../../../../../set-split.md). In a [first-order consistent](../../../../../first-order-consistency.md) [first-order theory](../../../../../first-order-theory.md) these two obligations make $A$ and $B$ disjoint.

Let $h$ be the [Gödel number](../../../../../godel-number.md) of $H(v_1)$ and take the literal diagonal [first-order sentence](../../../../../first-order-sentence.md) $R=H(\bar h)$. If $S\vdash R$, then $h$ belongs to the second source [set](../../../../../set-split.md), so separation gives $S\vdash\neg H(\bar h)$, a [contradiction](../../../../../contradiction.md). If $S\vdash\neg R$, then $h$ belongs to the first source [set](../../../../../set-split.md), so separation gives $S\vdash H(\bar h)$, again a [contradiction](../../../../../contradiction.md). Hence

$$
\boxed{S\text{ consistent}\Longrightarrow S\nvdash R\text{ and }S\nvdash\neg R.}
$$

The direction of separation matters: here $H$ is provable on refutable diagonal codes and refutable on provable diagonal codes.

## ↑ Ancestors (13)

1. [A](../a.md)
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
