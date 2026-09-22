<h1 id="22h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $K$ is nonempty; without that necessary hypothesis the assertion is false. Put $d=\inf_{z\in K}\|x-z\|_p$ and choose $y_n\in K$ with $\|x-y_n\|_p\to d$. Convexity gives $(y_n+y_m)/2\in K$, so its distance to $x$ is at least $d$. Apply the supplied uniform-convexity inequality to $x-y_n$ and $x-y_m$:

$$
\|y_n-y_m\|_p^p\leq2^{p-1}(\|x-y_n\|_p^p+\|x-y_m\|_p^p)-2^pd^p\longrightarrow0.
$$

Thus the minimizing sequence is Cauchy. Completeness of the [Banach space](../../../../../../banach-space-split.md) $\ell^p$ gives $y_n\to y$; closedness gives $y\in K$, and continuity of the norm gives $\|x-y\|_p=d$. **The minimum distance is attained.** This is the [nearest point in a uniformly convex Banach space](../../../../../../nearest-point-in-a-uniformly-convex-banach-space.md) property. The same inequality applied to two minimizers shows uniqueness, though existence alone was requested.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22H](../../22h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
