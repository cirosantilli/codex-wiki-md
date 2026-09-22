<h1 id="11f/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

**True.** By the [Weierstrass approximation theorem](../../../../../../../weierstrass-approximation-theorem.md), choose polynomials $q_n$ with $q_n\to f^{(m)}$ uniformly. Define $P_n$ by integrating $q_n$ exactly $m$ times and choose the $m$ integration constants so that

$$
P_n^{(r)}(0)=f^{(r)}(0),
\qquad 0\leq r<m.
$$

Then $P_n^{(m)}=q_n$, and repeated use of the [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) gives

$$
\|P_n^{(r)}-f^{(r)}\|_\infty
\leq\frac{\|q_n-f^{(m)}\|_\infty}{(m-r)!}
\qquad(0\leq r<m).
$$

Every derivative therefore converges uniformly as required.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [11F](../../../11f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
