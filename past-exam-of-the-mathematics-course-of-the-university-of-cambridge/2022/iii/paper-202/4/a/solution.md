<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Applying the [Itô formula](../../../../../../ito-s-lemma.md) to $f(x)=x^2$ and the semimartingale $B$ gives

$$
B_t^2=2\int_0^tB_s\,dB_s+t.
$$

Hence

$$
X_t=-2\int_0^tB_s\,dB_s+\int_0^t(B_s^2-1)\,ds.
$$

The first term is a continuous local martingale and the second has finite variation. By uniqueness of the continuous semimartingale decomposition, $X$ could be a local martingale only if the finite-variation term were constant. Its derivative $B_s^2-1$ is not zero almost everywhere, so $X$ is not a local martingale.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
