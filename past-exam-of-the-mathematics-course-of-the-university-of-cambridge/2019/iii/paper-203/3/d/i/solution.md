<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $z$ and write

$$
L_t(z)=\log(g_t(z)-U_t).
$$

By assumption, $L(z)$ is a continuous local martingale, so $Z_t(z)=e^{L_t(z)}$ is a [semimartingale](../../../../../../../semimartingale.md). The [Chordal Loewner equation](../../../../../../../chordal-loewner-equation.md) gives

$$
g_t(z)=z+\int_0^t\frac2{Z_s(z)}ds,
$$

which has [finite variation](../../../../../../../total-variation-of-a-function.md). Therefore

$$
U_t=g_t(z)-Z_t(z)
$$

is a semimartingale. Thus **the Loewner driver $U$ is a continuous semimartingale**.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
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
