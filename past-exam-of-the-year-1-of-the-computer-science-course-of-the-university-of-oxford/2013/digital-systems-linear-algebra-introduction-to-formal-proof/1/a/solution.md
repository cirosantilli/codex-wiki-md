<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [disjunctive normal form](../../../../../disjunctive-normal-form.md), also called a [sum of products](../../../../../disjunctive-normal-form.md), is an OR of AND terms, each made from [Boolean literals](../../../../../boolean-literal.md) such as $a$ or $\bar a$. For example,

$$
f(a,b,c)=ab+\bar a c.
$$

Here juxtaposition means [logical conjunction](../../../../../logical-conjunction.md), $+$ means [logical disjunction](../../../../../logical-disjunction.md), and a bar means [negation](../../../../../negation.md). The expression need not be canonical: a term can omit variables, and need not name a single row of the [truth table](../../../../../truth-table.md).

Implement each product by an [AND gate](../../../../../and-gate.md) and combine the products with an [OR gate](../../../../../or-gate.md). Supply complemented inputs with [NOT gates](../../../../../not-gate.md). Thus

$$
\boxed{\text{sum of products}\quad\longleftrightarrow\quad\text{AND layer followed by OR layer}.}
$$

This is the usual two-level [combinational logic](../../../../../combinational-logic.md) realization, counting complemented inputs as available. If [NOT gates](../../../../../not-gate.md) are counted, a complemented input can traverse three gates. The two-level depth statement also assumes sufficiently large gate fan-in: using only two-input [logic gates](../../../../../logic-gate.md) requires trees for long products or sums. Constant, single-product and single-literal [Boolean functions](../../../../../boolean-function.md) may need fewer levels, so the two-level construction is a general bound, not a claim that every expression requires exactly two layers.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
