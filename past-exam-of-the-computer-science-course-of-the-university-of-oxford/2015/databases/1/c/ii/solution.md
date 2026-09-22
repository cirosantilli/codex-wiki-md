<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take a unary [database relation](../../../../../../database-relation.md) $R$ and the positive [domain relational calculus](../../../../../../domain-relational-calculus.md) query

$$
\boxed{Q=\{(x,y)\mid R(x)\lor R(y)\}.\quad\text{The assertion is false.}}
$$

For the finite input $R=\{0\}$, every pair $(0,d)$ and $(d,0)$ belongs to $Q$, for every value $d$ in the ambient domain. On an infinite ambient domain the answer is infinite. Even if one compares only finite ambient domains, adding a fresh value $d$ changes the answer while leaving $R$ fixed, violating [domain independence of a database query](../../../../../../domain-independence-of-a-database-query.md).

The [logical disjunction](../../../../../../logical-disjunction.md) leaves $y$ unrestricted in its first branch and $x$ unrestricted in its second branch. Thus both variables occur in relational atoms somewhere in the formula, yet [database query safety](../../../../../../database-query-safety.md) still fails. No negation or implication symbol occurs.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Databases](../../../../databases-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
