<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An [arithmetic mean](../../../../../../arithmetic-mean.md) is [database aggregation](../../../../../../database-aggregation.md), which is outside classical [relational algebra](../../../../../../relational-algebra.md). Use [SQL](../../../../../../sql.md):
```
SELECT AVG(s.price) AS average_sale_price
FROM Sales AS s
JOIN Car AS c ON c.serialnumber = s.serialnumber
WHERE c.make = 'Saab';
```
For non-null prices $p_1,\ldots,p_n$ of qualifying sales, the result is

$$
\boxed{\overline p=\frac{p_1+\cdots+p_n}{n}\quad(n>0).}
$$

Each sale contributes once, even when a car was sold on several invoices. Do not use `DISTINCT` inside `AVG`: two different sales at the same price must both count. The car's [database primary key](../../../../../../database-primary-key.md) makes the [relational join](../../../../../../relational-join.md) match each sale to exactly one car, so the [relational join](../../../../../../relational-join.md) introduces no extra weighting.

If there are no qualifying non-null prices, `AVG` returns [SQL NULL](../../../../../../sql-null.md). It ignores null prices if the implementation permits them; it does not replace an absent [arithmetic mean](../../../../../../arithmetic-mean.md) with zero.[Section 9.21, `avg` and the paragraph on aggregates with no selected rows](../../../../../../aggregate-functions-in-the-postgresql-documentation.md)

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
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
