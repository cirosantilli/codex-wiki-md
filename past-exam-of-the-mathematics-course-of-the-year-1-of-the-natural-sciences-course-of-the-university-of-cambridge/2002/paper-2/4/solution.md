<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The number $R$ of successes has a [binomial distribution](../../../../binomial-distribution.md). Each arrangement of $r$ successes and $n-r$ failures has [probability](../../../../probability.md) $p^rq^{n-r}$ by [independence](../../../../independent-random-variables.md), and the [binomial coefficient](../../../../binomial-coefficient-split.md) counts the arrangements. Therefore

$$
\boxed{p_r=\binom nr p^rq^{n-r},\quad 0\leq r\leq n;\qquad\sum_{r=0}^n p_r=(p+q)^n=1.}
$$

The final equality is the [binomial theorem](../../../../binomial-theorem.md). Writing $R$ as a sum of [independent](../../../../independent-random-variables.md) [Bernoulli random variables](../../../../bernoulli-distribution.md) gives its [expectation](../../../../expected-value-split.md) and [variance](../../../../variance-split.md): $\mathbb E R=np$, $\operatorname{Var}(R)=npq$. Thus the matching [normal distribution](../../../../normal-distribution.md) has

$$
\boxed{\mu=np,\qquad\sigma=\sqrt{npq}.}
$$

The [normal approximation](../../../../normal-approximation.md) is appropriate when both expected counts $np$ and $nq$ are sufficiently large; large $n$ alone is insufficient if $p$ is extremely close to zero or one.

For the guessing student, $n=60$, $p=1/4$, $q=3/4$. Therefore the expected number of correct answers is $\boxed{15}$, and $\sigma^2=45/4$, $\sigma=3\sqrt5/2$. The inclusive integer range $13,14,15,16,17$ becomes $12.5\leq X\leq17.5$ after the [continuity correction](../../../../continuity-correction.md). Standardizing the [normal distribution](../../../../normal-distribution.md) gives

$$
\begin{aligned}
\mathbb P(13\leq R\leq17)&\approx\mathbb P(12.5\leq X\leq17.5)\\
&=\frac1{\sqrt{2\pi}}\int_{-\sqrt5/3}^{\sqrt5/3}e^{-z^2/2}\,dz\\
&=\frac2{\sqrt{2\pi}}\int_0^{\sqrt5/3}e^{-z^2/2}\,dz>2\cdot\frac14=\boxed{\frac12}.
\end{aligned}
$$

Here $(5/2)/(3\sqrt5/2)=\sqrt5/3$, and the last step uses the supplied bound. The approximate [probability](../../../../probability.md) is $0.54394$. The [normal approximation](../../../../normal-approximation.md) provides the requested conclusion; as a separate check, summing the five exact [binomial probabilities](../../../../binomial-probability.md) gives approximately $0.54370$, also exceeding one half.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
