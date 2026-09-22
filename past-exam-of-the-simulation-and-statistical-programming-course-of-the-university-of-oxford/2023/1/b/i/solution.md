<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrating the envelope $p\leq Mq$ shows $M\geq1$. One trial of [rejection sampling](../../../../../rejection-sampling.md) draws $Y\sim q$ and an [independent](../../../../../independent-random-variables.md) $U$ from the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$, and accepts $Y$ if $U\leq p(Y)/(Mq(Y))$. Repeat with fresh [independent random variables](../../../../../independent-random-variables.md) after each rejection. Ratios need only be evaluated where $q>0$; the envelope makes the target zero wherever $q=0$.

For any [measurable set](../../../../../measurable-set.md) $B$, integration of the [conditional probability](../../../../../conditional-probability.md) of acceptance gives

$$
\mathbb P(Y\in B,\mathrm{accept})=\int_Bq(y)\frac{p(y)}{Mq(y)}\,dy=\frac1M\int_Bp(y)\,dy.
$$

Taking the whole domain gives acceptance [probability](../../../../../probability.md) $1/M$, and dividing gives $\mathbb P(Y\in B\mid\mathrm{accept})=\int_Bp(y)\,dy$. Fresh trials therefore supply [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) $X_1,\ldots,X_m$ with target [probability density function](../../../../../probability-density-function.md) $p$. The corresponding [Monte Carlo estimator](../../../../../monte-carlo-estimator.md) is

$$
\boxed{\widehat\theta_m^{\mathrm{RS}}=\frac1m\sum_{j=1}^m\phi(X_j).}
$$

The proposal count $T$ up to and including one acceptance has the [geometric distribution](../../../../../geometric-distribution.md)

$$
\mathbb P(T=t)=(1-1/M)^{t-1}/M,\quad t=1,2,\ldots,
\qquad
\boxed{\mathbb ET=M.}
$$

For example, the [tail-sum formula](../../../../../tail-sum-formula.md) gives $\mathbb ET=\sum_{t\geq0}(1-1/M)^t=M$. Thus the expected cost is $M$ proposal draws per accepted target draw.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
