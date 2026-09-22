<h1 id="18/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the recurrence repeatedly down to $m=2$:

$$
I_{m,n}=\frac{(m-2)(m-3)\cdots1}{(m+n-3)(m+n-4)\cdots n}\,I_{2,n}.
$$

Including the base factor $1/(n-1)$ and rewriting the products as [factorials](../../../../../../factorial.md) gives

$$
\boxed{I_{m,n}=\frac{(m-2)!(n-2)!}{(m+n-3)!},\qquad m,n\in\mathbb Z,\quad m,n>1.}
$$

The formula also includes $m=2$ because $0!=1$. It is symmetric in $m,n$, consistent with the [integration by substitution](../../../../../../integration-by-substitution.md) $x=1/t$. Equivalently it is the [Euler beta function](../../../../../../beta-function.md) $B(m-1,n-1)$, although that identification is not needed for the recurrence derivation.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [18](../../../18.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
