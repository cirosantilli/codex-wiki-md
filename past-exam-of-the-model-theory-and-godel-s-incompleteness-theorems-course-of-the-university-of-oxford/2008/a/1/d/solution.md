<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $T=S\cup\{\neg G_S\}$. The first supplied equivalence, retained in $T$, combines with its new axiom to give

$$
T\vdash\neg\operatorname{Con}(S).
$$

The supplied implication $\operatorname{Con}(T)\to\operatorname{Con}(S)$ then yields, by contraposition,

$$
T\vdash\neg\operatorname{Con}(T).
$$

Finally the second supplied equivalence is $T\vdash G_T\leftrightarrow\operatorname{Con}(T)$, so propositional reasoning gives

$$
\boxed{T\vdash\neg G_T.}
$$

No extra [first-order consistency](../../../../../first-order-consistency.md) assumption is needed for this formal derivation. If $S$ is [first-order consistent](../../../../../first-order-consistency.md), part (b) shows that adding $\neg G_S$ preserves [first-order consistency](../../../../../first-order-consistency.md), because inconsistency of the extension would imply $S\vdash G_S$. Such a [first-order consistent](../../../../../first-order-consistency.md) extension therefore proves the [negation](../../../../../negation.md) of its own true [Gödel sentence](../../../../../godel-sentence.md), illustrating why [first-order consistency](../../../../../first-order-consistency.md) alone does not imply [one-consistency](../../../../../one-consistency.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [A](../../../a.md)
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
