<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $H(\vec v)$ for the proposed stage-comparison [logical formula](../../../../../logical-formula.md) and fix a standard [tuple](../../../../../finite-tuple.md) $\vec a$. If $\vec a\in A$, [numeralwise enumeration in arithmetic](../../../../../numeralwise-enumeration-in-arithmetic.md) supplies a standard $m$ with $S\vdash F(\bar{\vec a},\bar m)$. Disjointness gives $\vec a\notin B$, so $S\vdash\neg G(\bar{\vec a},\bar j)$ for every standard $j$, in particular $j=0,\ldots,m$. The source's finite initial-segment axiom combines this finite list into

$$
S\vdash\forall y\le\bar m\,\neg G(\bar{\vec a},y).
$$

Use $\bar m$ as the [existential witness](../../../../../existential-witness.md) to obtain $S\vdash H(\bar{\vec a})$.

If instead $\vec a\in B$, choose $n$ with $S\vdash G(\bar{\vec a},\bar n)$. Disjointness gives refutations of $F(\bar{\vec a},\bar j)$ for all $j$, so the finitely many $j\le n$ give

$$
S\vdash\forall x\le\bar n\,\neg F(\bar{\vec a},x).
$$

For an arbitrary $x$, the source's comparison axiom gives $x\le\bar n$ or $\bar n\le x$. In the first case the first conjunct of the proposed witness condition is false. In the second case $y=\bar n$ witnesses failure of its bounded universal conjunct, since $G(\bar{\vec a},\bar n)$ is provable. Generalization over $x$ therefore gives $S\vdash\neg H(\bar{\vec a})$.

Thus **the [logical formula](../../../../../logical-formula.md) separates $A$ from $B$**. The [formal proof](../../../../../formal-proof.md) uses the enumerators' numeralwise positive and negative [formal proof](../../../../../formal-proof.md) properties and the two explicit order principles supplied in the source; it does not assume the [first-order theory](../../../../../first-order-theory.md) can decide arbitrary unbounded existential [logical formulas](../../../../../logical-formula.md).

## ↑ Ancestors (13)

1. [B](../b.md)
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
