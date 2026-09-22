<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $f_n\to f$ and $g_n\to g$ with [uniform convergence](../../../../../../../uniform-convergence.md). The [triangle inequality](../../../../../../../triangle-inequality.md) gives

$$
\sup_E|(f_n+g_n)-(f+g)|\leq\sup_E|f_n-f|+\sup_E|g_n-g|\longrightarrow0.
$$

Hence $f_n+g_n\to f+g$ with [uniform convergence](../../../../../../../uniform-convergence.md).

If every $f_n,g_n$ is a [bounded function](../../../../../../../bounded-function.md), part [iii](../../a/iii.md) gives constants $M_f,M_g$ bounding the two families. Their [pointwise limits](../../../../../../../pointwise-limit.md) satisfy $|f|\leq M_f$ and $|g|\leq M_g$. Consequently

$$
\begin{aligned}
\sup_E|f_ng_n-fg|
&\leq\sup_E\bigl(|f_n|\,|g_n-g|+|g|\,|f_n-f|\bigr)\\
&\leq M_f\sup_E|g_n-g|+M_g\sup_E|f_n-f|\longrightarrow0.
\end{aligned}
$$

Thus **both sums and products have [uniform convergence](../../../../../../../uniform-convergence.md) under the stated hypotheses**. The product estimate is the [uniform convergence product rule for bounded functions](../../../../../../../uniform-convergence-product-rule-for-bounded-functions.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
