<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The graph has no cause of $D$, so $D$ is independent of its potential outcomes. By [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md), the [G-formula](../../../../../../g-computation.md) therefore gives

$$
\mathbb E[Y(d)]=\mathbb E[Y\mid D=d].
$$

Condition on $M$ and use the structural zero from part ii:

$$
\begin{aligned}
\mathbb E[Y(d)]
&=\mathbb E[Y\mid D=d,M=1]\mathbb P(M=1\mid D=d)\\
&\quad+\mathbb E[Y\mid D=d,M=0]\mathbb P(M=0\mid D=d)\\
&=\mathbb E[Y\mid D=d,M=1]\mathbb P(M=1\mid D=d).
\end{aligned}
$$

Consequently the [causal risk ratio](../../../../../../causal-risk-ratio.md) is

$$
\frac{\mathbb E[Y(1)]}{\mathbb E[Y(0)]}
=\frac{\mathbb E[Y\mid D=1,M=1]}{\mathbb E[Y\mid D=0,M=1]}
\frac{\mathbb P(M=1\mid D=1)}{\mathbb P(M=1\mid D=0)}.
$$

Applying [Bayes' theorem](../../../../../../bayes-theorem.md) to the second factor gives

$$
\frac{\mathbb P(M=1\mid D=1)}{\mathbb P(M=1\mid D=0)}
=\frac{\mathbb P(D=1\mid M=1)/\mathbb P(D=0\mid M=1)}
{\mathbb P(D=1)/\mathbb P(D=0)},
$$

which proves the stated formula. The unmeasured common cause $U$ of $M$ and $Y$ does not obstruct this total-effect argument because no mediator effect is being identified.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
