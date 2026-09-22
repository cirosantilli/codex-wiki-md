<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x\in X$ and $t>0$, form the [Bochner integral](../../../../../../bochner-integral.md)

$$
x_t=\frac1t\int_0^tU(s)x\,ds.
$$

The semigroup property gives, for $h>0$,

$$
\frac{U(h)x_t-x_t}{h}
=\frac1{th}
\left(\int_t^{t+h}U(s)x\,ds-
\int_0^hU(s)x\,ds\right).
$$

Strong continuity lets $h\downarrow0$, yielding

$$
x_t\in D(A),
\qquad
Ax_t=\frac{U(t)x-x}{t}.
$$

Also,

$$
\|x_t-x\|
\leq\frac1t\int_0^t\|U(s)x-x\|\,ds\longrightarrow0
$$

by strong continuity. Every $x\in X$ is therefore a norm limit of elements of $D(A)$, so

$$
\boxed{\overline{D(A)}=X}.
$$

This approximation is the basic [Yosida averaging of a semigroup](../../../../../../yosida-averaging-of-a-semigroup.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
