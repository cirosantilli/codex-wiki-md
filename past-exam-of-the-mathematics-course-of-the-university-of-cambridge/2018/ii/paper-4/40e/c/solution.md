<h1 id="40e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $C(n)$ counts complex multiplications and a twiddle product is reused in the two butterfly outputs, then

$$
C(n)=2C(n/2)+\frac n2,
\qquad C(1)=0.
$$

For $n=2^k$, solving the recurrence gives

$$
\boxed{C(n)=\frac n2\log_2n=2^{k-1}k}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
