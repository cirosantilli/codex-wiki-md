<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Use the intended model of [independent random variables](../../../../../independent-random-variables.md) $A,B$ with [exponential distributions](../../../../../exponential-distribution.md) of rates $\alpha,\beta>0$. For $M=\min(A,B)$, independence gives the [survival function](../../../../../survival-function.md)

$$
P(M>t)=P(A>t)P(B>t)=e^{-(\alpha+\beta)t},\qquad t\geq0.
$$

Thus

$$
\boxed{M\sim\operatorname{Exp}(\alpha+\beta),\qquad
f_M(t)=(\alpha+\beta)e^{-(\alpha+\beta)t}\ (t>0),\qquad
\operatorname{sd}(M)=\frac1{\alpha+\beta}.}
$$

The [variance](../../../../../variance-split.md) is $1/(\alpha+\beta)^2$, obtained from the standard first two exponential moments, $E M=1/(\alpha+\beta)$ and $E M^2=2/(\alpha+\beta)^2$.

For these [competing exponential clocks](../../../../../competing-exponential-clocks.md), ties have [probability](../../../../../probability.md) zero. Integrating over Alice's firing time gives

$$
\boxed{P(A<B)=\int_0^\infty\alpha e^{-\alpha t}e^{-\beta t}\,dt
=\frac{\alpha}{\alpha+\beta}.}
$$

Let $H$ denote the event that the next shot hits, and use the stated success probability as $P(H\mid A<B)=1/2$. Bill's corresponding conditional success probability is one. The [law of total probability](../../../../../law-of-total-probability.md) gives

$$
P(H)=\frac12\frac{\alpha}{\alpha+\beta}+\frac{\beta}{\alpha+\beta}.
$$

The [Bayes' theorem](../../../../../bayes-theorem.md) therefore yields

$$
\boxed{P(A<B\mid H)=\frac{\alpha}{\alpha+2\beta}.}
$$

The printed assumptions specify the two marginal [exponential distributions](../../../../../exponential-distribution.md) but do not explicitly specify their independence. The answers above require that extra assumption; marginals alone do not determine the race. For a concrete counterexample, take one $Z\sim\operatorname{Exp}(1)$ and set $A=Z/\alpha$, $B=Z/\beta$. These have the required marginals, but $M\sim\operatorname{Exp}(\max(\alpha,\beta))$; if $\alpha>\beta$, Alice always fires first and $P(A<B\mid H)=1$. Thus the independence qualification changes actual answers, rather than merely their derivation.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
