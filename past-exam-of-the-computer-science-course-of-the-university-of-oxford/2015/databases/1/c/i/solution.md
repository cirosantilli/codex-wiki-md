<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the two [database queries](../../../../../../database-query.md) have compatible output [database attributes](../../../../../../database-attribute.md). Then

$$
\boxed{\text{True: }Q_1-Q_2\text{ is safe.}}
$$

For a finite input [database](../../../../../../database.md), the result of the [relational difference](../../../../../../relational-difference.md) is a subset of the finite result of $Q_1$, so it is finite and introduces no new values. For the usual [domain independence of a database query](../../../../../../domain-independence-of-a-database-query.md), let $D$ be the input [database](../../../../../../database.md) and let $A\subseteq A'$ be two ambient value domains containing its data and the query constants. [Database query safety](../../../../../../database-query-safety.md) gives

$$
Q_i^A(D)=Q_i^{A'}(D)\quad(i=1,2),
$$

and therefore

$$
Q_1^A(D)\setminus Q_2^A(D)=Q_1^{A'}(D)\setminus Q_2^{A'}(D).
$$

Although a [domain relational calculus](../../../../../../domain-relational-calculus.md) expression for the [relational difference](../../../../../../relational-difference.md) uses negation, its positive membership requirement in $Q_1$ supplies the necessary range restriction. Negation is not by itself a reason for failure of [database query safety](../../../../../../database-query-safety.md).

## ↑ Ancestors (12)

1. [I](../i.md)
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
