<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [adapted process](../../../../../adapted-process.md) is bounded by $1$, so every $X_n$ is an [integrable random variable](../../../../../integrable-random-variable.md), indeed a [square-integrable](../../../../../square-integrable-function.md) [random variable](../../../../../random-variable-split.md). [Independence](../../../../../independent-random-variables.md) of $U_{n+1}$ from $\mathcal F_n$ and its [continuous uniform distribution](../../../../../continuous-uniform-distribution.md) give

$$
\mathbb E[B_{n+1}\mid\mathcal F_n]=X_n.
$$

This calculation with a random threshold is justified by conditioning on the $\mathcal F_n$-[measurable](../../../../../measurability.md) value of $X_n$: for a fixed $t\in[0,1]$, the [Lebesgue integral](../../../../../lebesgue-integral.md) $\int_0^1\mathbf1_{\{u\leq t\}}\,du$ equals $t$. More formally, [independence](../../../../../independent-random-variables.md) integrates the bounded [Borel measurable function](../../../../../borel-measurable-function.md) $(t,u)\mapsto\mathbf1_{\{u\leq t\}}$ over its second coordinate. Therefore

$$
\mathbb E[X_{n+1}\mid\mathcal F_n]
=\tfrac12X_n+\tfrac12\mathbb E[B_{n+1}\mid\mathcal F_n]=X_n,
$$

which verifies the [martingale](../../../../../martingale-split.md) property for this [filtration](../../../../../filtration-probability-theory.md).

Since $B_{n+1}^2=B_{n+1}$, the [conditional expectation](../../../../../conditional-expectation.md) of the squared [martingale difference](../../../../../martingale-difference.md) is

$$
\begin{aligned}
\mathbb E[(X_{n+1}-X_n)^2\mid\mathcal F_n]
&=\tfrac14\mathbb E[(B_{n+1}-X_n)^2\mid\mathcal F_n]\\
&=\tfrac14(X_n-2X_n^2+X_n^2)
=\tfrac14X_n(1-X_n).
\end{aligned}
$$

The [law of total expectation](../../../../../law-of-total-expectation.md) yields **$\mathbb E[(X_{n+1}-X_n)^2]=\frac14\mathbb E[X_n(1-X_n)]$**. In particular, $\mathbb EX_n=x$ for every $n$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
