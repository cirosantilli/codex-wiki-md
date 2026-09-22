<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

For a nonnegative [random variable](../../../../../random-variable-split.md) $Y$ with finite [expected value](../../../../../expected-value.md), and $a>0$, [Markov's inequality](../../../../../markov-inequality.md) states $P(Y\geq a)\leq\mathbb E[Y]/a$. Indeed $Y\geq a\mathbf1_{\{Y\geq a\}}$, and taking [expected values](../../../../../expected-value.md) proves the bound. For a [random variable](../../../../../random-variable-split.md) $X$ with mean $\mu$ and finite [variance](../../../../../variance-split.md) $\sigma^2$, apply [Markov's inequality](../../../../../markov-inequality.md) to $(X-\mu)^2$ at threshold $\varepsilon^2$. This proves [Chebyshev's inequality](../../../../../chebyshev-inequality.md):

$$
\boxed{P(|X-\mu|\geq\varepsilon)\leq\frac{\sigma^2}{\varepsilon^2}.}
$$

For [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) $X_1,X_2,\ldots$ with finite mean $\mu$ and [variance](../../../../../variance-split.md) $\sigma^2$, the sample mean has [expected value](../../../../../expected-value.md) $\mu$ and [variance](../../../../../variance-split.md) $\sigma^2/n$. Thus

$$
P\left(\left|\frac1n\sum_{i=1}^nX_i-\mu\right|\geq\varepsilon\right)\leq\frac{\sigma^2}{n\varepsilon^2}\longrightarrow0.
$$

This is **the weak law: $\boxed{n^{-1}\sum_{i=1}^nX_i\to\mu\text{ in probability}}$**, with the finite-variance hypotheses used in this direct deduction.

The more general [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) needs only $\mathbb E|X_1|<\infty$. To obtain that version, truncate $Y_i^{(K)}=X_i\mathbf1_{\{|X_i|\leq K\}}$. For fixed $K$ the bounded variables obey the result just proved. Their means tend to $\mu$, while [Markov's inequality](../../../../../markov-inequality.md) bounds the probability that the two sample means differ by more than $\varepsilon/3$ by $3\mathbb E[|X_1|\mathbf1_{\{|X_1|>K\}}]/\varepsilon$. First take $n\to\infty$ and then $K\to\infty$; the integrable tail vanishes, proving the full integrable i.i.d. version as well.

Finally assume $\mathbb E[X]=0$ and $\operatorname{Var}(X)=\sigma^2$. For every $b>0$, $X\geq a$ implies $(X+b)^2\geq(a+b)^2$, so [Markov's inequality](../../../../../markov-inequality.md) gives

$$
P(X\geq a)\leq\frac{\mathbb E[(X+b)^2]}{(a+b)^2}=\frac{\sigma^2+b^2}{(a+b)^2}.
$$

If $\sigma^2>0$, the derivative of the right-hand side is $2(ab-\sigma^2)/(a+b)^3$, so its minimum is at $b=\sigma^2/a$. The [Cantelli inequality](../../../../../cantelli-inequality.md) follows:

$$
\boxed{P(X\geq a)\leq\frac{\sigma^2}{\sigma^2+a^2}.}
$$

If $\sigma^2=0$, $X=0$ almost surely and the same bound is immediate. The bound is sharp: put mass $\sigma^2/(\sigma^2+a^2)$ at $a$ and the remaining mass at $-\sigma^2/a$; this has exactly the prescribed mean and [variance](../../../../../variance-split.md).

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
