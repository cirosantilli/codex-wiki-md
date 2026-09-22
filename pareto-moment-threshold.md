# Pareto moment threshold

↑ **Parent:** [Pareto distribution](pareto-distribution.md)

A [Pareto distribution](pareto-distribution.md) is a proper [probability distribution](probability-distribution-split.md) for every $\alpha,\beta>0$, even when its [mean](expected-value-split.md) is infinite. To see both facts, integrate the [probability density function](probability-density-function.md) against $x^q$. For real $q\geq0$,

$$
\mathbb E[X^q]=\alpha\beta^\alpha\int_\beta^\infty x^{q-\alpha-1}\,dx
=\begin{cases}\dfrac{\alpha\beta^q}{\alpha-q},&0\leq q<\alpha,\\+\infty,&q\geq\alpha.\end{cases}
$$

The [improper integral](improper-integral.md) converges exactly when $q-\alpha-1<-1$. At $q=\alpha$ it diverges logarithmically; above that it diverges as a positive power of the upper endpoint. Setting $q=0$ gives one, proving normalization regardless of whether higher [moments](moment.md) exist.

Taking $q=1,2$ and using $\operatorname{Var}(X)=\mathbb E[X^2]-(\mathbb E[X])^2$ when both terms are finite gives

$$
\mathbb E[X]=\frac{\alpha\beta}{\alpha-1}\quad(\alpha>1),\qquad
\operatorname{Var}(X)=\frac{\alpha\beta^2}{(\alpha-1)^2(\alpha-2)}\quad(\alpha>2).
$$

For $0<\alpha\leq1$, the nonnegative [random variable](random-variable-split.md) has [expected value](expected-value-split.md) $+\infty$; a centered [variance](variance-split.md) about a finite [mean](expected-value-split.md) is unavailable. For $1<\alpha\leq2$, the [mean](expected-value-split.md) is finite and the [variance](variance-split.md) is infinite.[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Pareto Distribution, Moments: existence threshold, mean and variance](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-pareto-distribution.md) A finite total [probability](probability.md) and a finite [expected value](expected-value-split.md) answer different questions.

At the chosen minimum $\beta=10$, $\alpha=3$ gives $\mathbb E[X]=15$, $\mathbb E[X^2]=300$ and [variance](variance-split.md) $300-15^2=75$, but an infinite third [moment](moment.md). At $\alpha=3/2$, the [mean](expected-value-split.md) is 30 and the [variance](variance-split.md) is infinite; at $\alpha=3/4$, even the [mean](expected-value-split.md) is infinite, while the [median](median.md) remains the finite number $10\,2^{4/3}\simeq25.198$. At the boundary $\alpha=2$, the earlier example has [mean](expected-value-split.md) 20 but infinite [variance](variance-split.md). A finite sample contains finite values almost surely; that fact cannot establish that the underlying [mean](expected-value-split.md) or [variance](variance-split.md) is finite.

## ↑ Ancestors (8)

1. [Pareto distribution](pareto-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/11/b/solution.md)
