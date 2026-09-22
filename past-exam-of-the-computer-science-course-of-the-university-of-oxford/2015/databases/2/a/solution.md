<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Find the salesperson identifiers satisfying each price condition using [relational selection](../../../../../relational-selection.md) and [relational projection](../../../../../relational-projection.md):

$$
L=\pi_{\mathsf{salespersonid}}(\sigma_{\mathsf{price}=10000}S),\qquad H=\pi_{\mathsf{salespersonid}}(\sigma_{\mathsf{price}=30000}S).
$$

Intersect these identifier sets, [relational join](../../../../../relational-join.md) the result to the salesperson records, and apply [relational projection](../../../../../relational-projection.md) to names:

$$
\boxed{\pi_{\mathsf{name}}\left(P\bowtie_{\mathsf{empid=salespersonid}}(L\cap H)\right).}
$$

If intersection is not a primitive of the chosen [relational algebra](../../../../../relational-algebra.md), use $L\cap H=L-(L-H)$ with [relational difference](../../../../../relational-difference.md). There is no need to access `Car`: the [foreign key](../../../../../foreign-key.md) already ensures that every sale refers to a car.

Intersecting names instead of identifiers is wrong. Two different salespeople called Alex, one making only $10000$ sales and the other only $30000$ sales, would make Alex appear in both name sets although neither person satisfies the condition. Nor can one sale satisfy both price tests: the two distinct prices require distinct sale records.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
