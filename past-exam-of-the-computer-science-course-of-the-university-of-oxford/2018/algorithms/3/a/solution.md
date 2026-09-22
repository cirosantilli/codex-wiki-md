<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [standard maximum form of a linear program](../../../../../standard-maximum-form-of-a-linear-program.md)

$$
\boxed{\max\{c^Tz:Az\leq b,\ z\geq0\}.}
$$

An arbitrary [linear program](../../../../../linear-programming-split.md) can be converted by the following operations.

- Replace minimization of $c^Tx$ by maximization of $-c^Tx$, and negate the resulting optimal value when translating back. A constant term in the objective is recorded separately.
- Replace every unrestricted variable $x_j$ by $z_j^+-z_j^-$ with both new variables nonnegative. A nonpositive variable can instead be negated. A lower bound $x_j\geq\ell$ can be eliminated by writing $x_j=\ell+z_j$, $z_j\geq0$; other bounds remain [linear inequalities](../../../../../linear-inequality.md).
- Multiply a $\geq$ row by $-1$. Replace an equality $a^Tx=b$ by the pair $a^Tx\leq b$ and $-a^Tx\leq-b$.

These substitutions preserve the attainable objective values, up to the stated sign and constant corrections, and map [feasible points](../../../../../feasible-point.md) in both directions. An alternative standard-form convention uses $Az=b,z\geq0$: add a nonnegative [slack variable](../../../../../slack-variable.md) to each upper-bound row, or subtract a nonnegative [surplus variable](../../../../../surplus-variable.md) from a lower-bound row. The inequality convention above is used in the remaining solutions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
