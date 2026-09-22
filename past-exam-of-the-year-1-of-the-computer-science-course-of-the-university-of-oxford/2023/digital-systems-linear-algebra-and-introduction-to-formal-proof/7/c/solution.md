<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [propositional substitution](../../../../../propositional-substitution.md) simultaneously to the atomic variables:

$$
\varphi S=\bigl((X\lor Y)\land(X\lor\neg Y)\bigr)
\lor\bigl((Y\to X)\to\neg X\bigr).
$$

By distributivity and the complementary [literals](../../../../../boolean-literal.md) $Y,\neg Y$,

$$
(X\lor Y)\land(X\lor\neg Y)\equiv X.
$$

The other disjunct simplifies using [logical implication](../../../../../logical-implication.md) and absorption:

$$
(Y\to X)\to\neg X
\equiv\neg(\neg Y\lor X)\lor\neg X
\equiv(Y\land\neg X)\lor\neg X
\equiv\neg X.
$$

Thus **$\varphi S\equiv X\lor\neg X\equiv\top$**, a [tautology](../../../../../tautology.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Introduction to formal proof](../../introduction-to-formal-proof.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
