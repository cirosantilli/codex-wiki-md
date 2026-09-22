<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The empty-bin indicators are not independent. For distinct $i,k$,

$$
\mathbb P(Z_i=Z_k=1)=\left(1-\frac2n\right)^m,
$$

whereas $\mathbb P(Z_i=1)\mathbb P(Z_k=1)=(1-1/n)^{2m}$.

Each bin is empty precisely when all $m$ balls avoid it, so

$$
\mathbb EZ_i=\left(1-\frac1n\right)^m.
$$

The [linearity of expectation](../../../../../../linearity-of-expectation.md) does not require independence and gives

$$
\boxed{\mathbb EZ=n\left(1-\frac1n\right)^m.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
