<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The statement requires $K\ne\varnothing$; an empty set is closed and convex but contains no minimizer. Assume this necessary condition and put $d=\inf_{g\in K}\|g-f\|_p$. Since $K$ is closed and $f\notin K$, $d>0$. Choose a [minimizing sequence](../../../../../../minimizing-sequence.md) $g_j\in K$ with $\|g_j-f\|_p\to d$.

The midpoint $(g_j+g_k)/2$ lies in the [convex set](../../../../../../convex-set.md) $K$. Applying the stated [Clarkson inequality](../../../../../../clarkson-s-inequalities.md) to $g_j-f$ and $g_k-f$ gives

$$
\|g_j-g_k\|_p^p
\leq2^{p-1}\bigl(\|g_j-f\|_p^p+\|g_k-f\|_p^p\bigr)
-\|g_j+g_k-2f\|_p^p
\leq2^{p-1}\bigl(\|g_j-f\|_p^p+\|g_k-f\|_p^p\bigr)-2^pd^p.
$$

The right side tends to zero, so $g_j$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). By [completeness of Lp spaces](../../../../../../completeness-of-lp-spaces.md), proved in Question 2(a), it converges to some $h$. Closedness puts $h$ in $K$, and continuity of the norm gives $\boxed{\|h-f\|_p=d}$. This is the [closest point theorem for a closed convex subset of Lp](../../../../../../closest-point-theorem-for-a-closed-convex-subset-of-lp.md). The same inequality applied to two minimizers forces their difference to be zero, so the minimizer is also unique.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
