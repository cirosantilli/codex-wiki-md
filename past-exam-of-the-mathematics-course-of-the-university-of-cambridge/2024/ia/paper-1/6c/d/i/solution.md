<h1 id="6c/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expanding $\det A^{(n)}$ along its last row gives the last diagonal contribution $a_nd_{n-1}$. The only other nonzero entry is $c_{n-1}$; expanding its minor along the last column contributes

$$
-b_{n-1}c_{n-1}d_{n-2}.
$$

Thus the [tridiagonal determinant recurrence](../../../../../../../tridiagonal-determinant-recurrence.md) is

$$
\boxed{d_n=a_nd_{n-1}-b_{n-1}c_{n-1}d_{n-2}},
$$

so

$$
\boxed{X_n=a_n,\qquad Y_n=-b_{n-1}c_{n-1}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [6C](../../../6c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
