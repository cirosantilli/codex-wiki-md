<h1 id="13j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Writing $Y_i$ for `team1_goal` and $x_i$ for `team1_xg`, the first hypothesis concerns only the [expected value](../../../../../../expected-value.md):

$$
H_1:\quad \mathbb E(Y_i\mid x_i)=x_i
\quad\text{for every }i.
$$

The second specifies the entire conditional [probability distribution](../../../../../../probability-distribution.md):

$$
H_2:\quad Y_i\mid x_i\sim\operatorname{Pois}(x_i)
\quad\text{for every }i,
$$

with independence between matches as assumed in the question. The [Poisson limit theorem](../../../../../../poisson-limit-theorem.md), often called the law of small numbers in this setting, suggests a [Poisson distribution](../../../../../../poisson-distribution.md) when a goal count is the sum of many approximately independent rare scoring opportunities.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
