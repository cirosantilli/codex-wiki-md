<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Causal identification](../../../../../../causal-identification.md) means that $\mathbb E[Y(a_1,a_2)]$ is uniquely determined by the observed joint distribution of $(A_1,X,A_2,Y)$ under the causal assumptions. Equivalently, it admits an identifying formula containing only observed-data probabilities and conditional expectations.

The [G-computation](../../../../../../g-computation.md) formula for this two-stage treatment is

$$
\boxed{
\mathbb E[Y(a_1,a_2)]
=\sum_x \mathbb E[Y\mid A_1=a_1,X=x,A_2=a_2]
\mathbb P(X=x\mid A_1=a_1)}.
$$

The first factor is the observed mean outcome after the specified treatment history and intermediate value; the second averages over the intermediate-variable distribution generated after the first treatment.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
