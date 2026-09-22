<h1 id="p/p4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply successive [Householder reflections](../../../../../householder-transformation.md) supported on smaller trailing coordinate sets. At step $k=1,\ldots,n-2$, let $x$ be the entries in rows $k+1,\ldots,n$ of column $k$ of the current [symmetric matrix](../../../../../symmetric-matrix.md). If $x\ne0$, part (c) gives an orthogonal reflection $H$ taking it to $ce_1$; if $x=0$, use the identity. Embed this as $Q_k=\operatorname{diag}(I_k,H)$ and replace the current matrix by $Q_k^TAQ_k$.

The first $k$ columns are unchanged by right multiplication. Left multiplication turns the tail of column $k$ into a vector supported only in row $k+1$. Previously treated columns have zero entries throughout this trailing coordinate set, so their zeros are preserved. Symmetry makes the matching row zeros appear as well. After the final step all entries below the first subdiagonal, and by symmetry above the first superdiagonal, vanish.

The product $Q=Q_1\cdots Q_{n-2}$ is orthogonal, and

$$
\boxed{Q^TAQ\text{ is tridiagonal}}.
$$

Restricting each transformation to its trailing coordinates is what preserves earlier zero patterns.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
