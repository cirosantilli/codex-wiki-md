<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The right-hand [relational projection](../../../../../relational-projection.md) lists the models of cars for which at least one recorded sale was made by a salesperson earning strictly more than $30000$. The outer [relational difference](../../../../../relational-difference.md) removes precisely those models from all models present in `Car`. Thus the answer is

$$
\boxed{\text{Models present in Car with no sale by a salesperson earning more than }30000.}
$$

This includes models with no sales at all, as well as models sold exclusively by salespeople whose salaries are at most $30000$. A model sold by both a low-paid salesperson and a high-paid salesperson is excluded. A salary exactly equal to $30000$ does not trigger exclusion. These are model-level statements: one unsold car of a model does not rescue that model if a different car of the same model had a qualifying sale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
