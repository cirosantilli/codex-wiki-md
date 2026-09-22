<h1 id="6c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiply the [birth-death master equation](../../../../../../birth-death-master-equation.md) by $n$ and sum. Index shifts give

$$
\dot\mu=(B-D)\mu.
$$

For the second moment, a birth changes $n^2$ by $2n+1$ and a death changes it by $-2n+1$, so

$$
\frac d{dt}\mathbb E[N^2]
=2(B-D)\mathbb E[N^2]+(B+D)\mu.
$$

Since $\sigma^2=\mathbb E[N^2]-\mu^2$,

$$
\boxed{\ (\sigma^2)'=2(B-D)\sigma^2+(B+D)\mu\ }.
$$

Together these are the [moment equations of a linear birth-death process](../../../../../../moment-equations-of-a-linear-birth-death-process.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
