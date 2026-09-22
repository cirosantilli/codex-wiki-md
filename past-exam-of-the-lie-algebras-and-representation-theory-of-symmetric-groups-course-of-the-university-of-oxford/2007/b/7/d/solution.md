<h1 id="b/7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For shape and type both $\mu$, column strictness makes every entry in row $r$ at least $r$. All $\mu_1$ entries equal to one must therefore be in the first row, which has exactly that length; it is filled with ones. Remove that row and repeat after subtracting one from the remaining labels. [Induction](../../../../../mathematical-induction.md) gives the unique filling whose $i$th row consists of $i$'s. Thus $K_{\mu\mu}=1$, and [Young's rule](../../../../../young-s-rule.md) proves that $S^\mu$ occurs exactly once.

More generally, if a semistandard filling of shape $\lambda$ and type $\mu$ exists, its entries at most $k$ must lie in the first $k$ rows. Counting them gives

$$
\sum_{i=1}^k\mu_i\le\sum_{i=1}^k\lambda_i\qquad\text{for every }k.
$$

These are the inequalities defining the [dominance order on partitions](../../../../../dominance-order-on-partitions.md). Hence $K_{\lambda\mu}>0$ implies $\boxed{\lambda\ge\mu}$, and the asserted restriction on summands follows from [Young's rule](../../../../../young-s-rule.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
