<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [accounting method](../../../../../accounting-method.md) assigns each operation a charge, its [amortized cost](../../../../../amortized-cost.md), that can differ from its actual cost. Cheap operations save the excess charge as credits associated with the [data structure](../../../../../data-structure-split.md) or its entries. An expensive operation spends these previously saved credits. The essential [invariant](../../../../../invariant-mathematics.md) is that the credit balance never becomes negative.

If the initial balance is zero, operation $i$ has actual cost $c_i$, charge $\widehat c_i$, and leaves balance $B_i$, then

$$
B_i=B_{i-1}+\widehat c_i-c_i,\qquad
\sum_{i=1}^n c_i=\sum_{i=1}^n\widehat c_i-B_n\leq\sum_{i=1}^n\widehat c_i.
$$

Thus **a nonnegative credit balance makes the total charge an upper bound on the total actual cost for every operation sequence**. In particular, a [constant time](../../../../../constant-time.md) charge proves a [linear time](../../../../../linear-time.md) total. The argument is a deterministic [amortized analysis](../../../../../amortized-analysis.md); it requires no [probability distribution](../../../../../probability-distribution-split.md) on the operations. A nonzero initial balance must be included as an additive term in the bound.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
