<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $1_A$ for the [indicator function](../../../../../../indicator-function.md) and use the normalized [Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md)

$$
\widehat A(r)=\mathbb E_x1_A(x)\omega^{-rx}.
$$

There are $N^5$ sextuples satisfying the equation, since any five coordinates determine the sixth. The desired [probability](../../../../../../probability.md) is consequently

$$
\frac1{N^5}\sum_{x_1+ x_2+x_3=x_4+x_5+x_6}\prod_{j=1}^6 1_A(x_j).
$$

By [orthogonality of complex exponentials](../../../../../../orthogonality-of-complex-exponentials.md), the indicator of the equation is

$$
\frac1N\sum_{r\in\mathbb Z_N}
\omega^{r(x_1+x_2+x_3-x_4-x_5-x_6)}.
$$

Substitution makes all six sums independent and gives the [sixth Fourier moment as a three-sum collision count](../../../../../../sixth-fourier-moment-as-a-three-sum-collision-count.md):

$$
\sum_{r\in\mathbb Z_N}\widehat A(-r)^3\widehat A(r)^3.
$$

Because $1_A$ is real, $\widehat A(-r)=\overline{\widehat A(r)}$. Hence the probability is

$$
\boxed{\sum_{r\in\mathbb Z_N}|\widehat A(r)|^6.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 147](../../../paper-147-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
