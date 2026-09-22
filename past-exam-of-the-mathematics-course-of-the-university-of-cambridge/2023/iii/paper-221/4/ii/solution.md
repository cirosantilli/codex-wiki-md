<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Instrumental-variable monotonicity](../../../../../../instrumental-variable-monotonicity.md) is

$$
A(1)\geq A(0)\quad\text{for every subject}.
$$

It excludes defiers who would quit without the incentive but continue smoking when offered it. The possible [principal strata](../../../../../../principal-stratum.md) are then never-takers $(0,0)$, compliers $(0,1)$, and always-takers $(1,1)$.

By random assignment, consistency, and exclusion,

$$
\begin{aligned}
\mathbb E[Y\mid Z=1]-\mathbb E[Y\mid Z=0]
&=\mathbb E\{Y(A(1))-Y(A(0))\}\\
&=\mathbb E[(Y(1)-Y(0))(A(1)-A(0))].
\end{aligned}
$$

The second identity follows by checking the two possible binary exposure values. Under monotonicity, $A(1)-A(0)$ is the indicator of being a complier. Therefore the numerator is

$$
\mathbb P(\text{complier})
\mathbb E[Y(1)-Y(0)\mid\text{complier}],
$$

while

$$
\mathbb E[A\mid Z=1]-\mathbb E[A\mid Z=0]
=\mathbb E[A(1)-A(0)]
=\mathbb P(\text{complier}).
$$

Their ratio is the [complier average treatment effect](../../../../../../local-average-treatment-effect.md), also called the [local average treatment effect](../../../../../../local-average-treatment-effect.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
