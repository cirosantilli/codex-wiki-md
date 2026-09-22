<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [binomial series](../../../../../../binomial-series.md) gives

$$
1-\alpha(1-s)^\beta=(1-\alpha)+\sum_{k\ge1}\alpha(-1)^{k+1}\binom\beta k\,s^k.
$$

Thus $p_0=1-\alpha>0$ and, for $k\ge1$,

$$
\boxed{p_k=\frac{\alpha\beta(1-\beta)(2-\beta)\cdots(k-1-\beta)}{k!}>0,}
$$

with the factors after $\beta$ omitted for $k=1$. The signs follow from $0<\beta<1$. As $s\uparrow1$, the series has nonnegative terms and its sum increases to $G(1)=1$, so [monotone convergence](../../../../../../monotone-convergence-theorem.md) gives $\sum_{k\ge0}p_k=1$. These are therefore genuine [probabilities](../../../../../../probability.md) on the nonnegative integers, proving that $G$ is a [probability generating function](../../../../../../probability-generating-function.md). Its [expected value](../../../../../../expected-value.md) is infinite, since $G'(s)=\alpha\beta(1-s)^{\beta-1}\to\infty$; finiteness of the mean is not required for this [branching process](../../../../../../branching-process.md).

Write $G_n(s)=1-A_n(1-s)^{\beta^n}$. The composition formula gives $A_{n+1}=A_n\alpha^{\beta^n}$, with $A_0=1$. Consequently $A_n=\alpha^{1+\beta+\cdots+\beta^{n-1}}$, and summing the [geometric series](../../../../../../geometric-series.md) yields **the explicit generation generating function**

$$
\boxed{G_n(s)=1-\alpha^{(1-\beta^n)/(1-\beta)}(1-s)^{\beta^n},\quad n\ge0.}
$$

This is the [fractional-power offspring generating function](../../../../../../fractional-power-offspring-generating-function.md) and its iterates.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
