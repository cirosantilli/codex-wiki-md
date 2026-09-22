<h1 id="11i/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $q=2d-n>0$. If $M$ is even, part (iii) gives

$$
\frac{dM(M-1)}2\le\frac{nM^2}{4},
$$

so

$$
qM\le2d.
$$

Because $M$ is even,

$$
M\le2\left\lfloor\frac dq\right\rfloor.
$$

If $M$ is odd, part (iii) instead gives

$$
\frac{dM(M-1)}2\le\frac{n(M^2-1)}4.
$$

Cancelling $M-1$ yields $qM\le n=2d-q$, and therefore

$$
M\le\frac{2d}{q}-1
<2\left\lfloor\frac dq\right\rfloor+1.
$$

Since $M$ is an integer, the same desired upper bound follows. Thus the binary [Plotkin bound](../../../../../../../plotkin-bound.md) is

$$
\boxed{A(n,d)\le
2\left\lfloor\frac d{2d-n}\right\rfloor}.
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [11I](../../../11i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
