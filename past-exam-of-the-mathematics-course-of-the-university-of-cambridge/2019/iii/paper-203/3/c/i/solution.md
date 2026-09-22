<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Z_t=g_t(z)-U_t$. For $\operatorname{SLE}_4$, $dU_t=2dB_t$, and the [Chordal Loewner equation](../../../../../../../chordal-loewner-equation.md) gives

$$
dZ_t=\frac2{Z_t}dt-2dB_t,
\qquad d\langle Z\rangle_t=4dt.
$$

The complex [Itô formula](../../../../../../../ito-s-lemma.md) yields

$$
d\log Z_t
=\frac1{Z_t}dZ_t-\frac1{2Z_t^2}d\langle Z\rangle_t
=-\frac2{Z_t}dB_t.
$$

Therefore

$$
\boxed{\log(g_t(z)-U_t)\text{ is a continuous local martingale}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
