<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The entries of $M^TM$ are real, and the [transpose](../../../../../transpose.md) rule gives $(M^TM)^T=M^TM$. Thus it is a real [symmetric matrix](../../../../../symmetric-matrix.md), hence also a [Hermitian matrix](../../../../../hermitian-operator.md).

For any complex vector $v$,

$$
v^\dagger M^TMv=(Mv)^\dagger(Mv)=\|Mv\|^2\geq0.
$$

In particular, if $M^TMv=\lambda v$ with $v\ne0$,

$$
\boxed{\lambda=\frac{\|Mv\|^2}{\|v\|^2}\geq0.}
$$

Thus $M^TM$ is [positive semidefinite](../../../../../positive-semidefinite-matrix.md). Its zero [eigenspace](../../../../../eigenspace.md) is precisely the kernel of $M$, since $\|Mv\|^2=0$ is equivalent to $Mv=0$. This is the Gram-matrix structure behind the nonnegative [eigenvalues](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
