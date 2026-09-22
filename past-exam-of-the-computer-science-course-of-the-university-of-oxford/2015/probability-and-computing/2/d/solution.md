<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If the bound in part (c) were available, the intended answer would be

$$
j_{\mathrm{intended}}(n)=2+\left\lceil\log_2\!\left(\max\{1,\log_2 n\}\right)\right\rceil,
\qquad n\geq1.
$$

Indeed $2^{j_{\mathrm{intended}}(n)-2}\geq\log_2 n$, so that bound would give $x_{j(n)}\leq n2^{-\log_2 n}=1$. Its growth is $O(\log\log n)$ in [Big O notation](../../../../../big-o-notation.md). Because (c) is false, this substitution alone does not prove the result for the actual [repeated singleton-removal allocation](../../../../../repeated-singleton-removal-allocation.md).

The requested order can nevertheless be established for the actual process. Here is a concrete, deliberately generous replacement, with $j(0)=0$ for the empty system:

$$
\boxed{j(n)=\begin{cases}
\left\lceil\log_{3/2}(2n)\right\rceil,&1\leq n<2^{120},\\
11+\left\lceil\log_2\log_2 n\right\rceil,&n\geq2^{120}.
\end{cases}}
$$

The large cutoff makes the numerical estimates below simple. A finite initial range does not affect the $O(\log\log n)$ [asymptotic analysis](../../../../../asymptotic-analysis.md).

First, whenever $2\leq b\leq n$, a ball is served with [probability](../../../../../probability.md) at least

$$
\left(1-\frac1n\right)^{n-1}\geq e^{-1}>\frac13.
$$

Thus part (a) gives $\mathbb E[B_{t+1}\mid B_t]\leq2B_t/3$, also for $B_t\leq1$. The [law of total expectation](../../../../../law-of-total-expectation.md) yields $x_t\leq n(2/3)^t$. This proves $x_{j(n)}\leq1/2$ for the small-$n$ branch, including $n=1$, whose single ball is served immediately.

For the large-$n$ branch, we need control of the random count, rather than an unjustified recurrence for its [expectation](../../../../../expected-value-split.md). If $b$ balls are allocated in a round, changing one chosen bin changes the number of singleton bins by at most two. The surviving count $F_b$ therefore has the [bounded differences property](../../../../../bounded-differences-property.md) with constants $2$. [McDiarmid's inequality](../../../../../mcdiarmid-s-inequality.md) gives

$$
\mathbb P(F_b>\mathbb EF_b+u)\leq\exp\!\left(-\frac{u^2}{2b}\right),\qquad u>0.
$$

This can be applied conditionally after any history, since the next allocations are fresh [independent random variables](../../../../../independent-random-variables.md).

Use this [concentration inequality](../../../../../concentration-inequality.md) in three stages. Write $L=\lceil\log_2\log_2 n\rceil$.

- For the first eight rounds, whenever $b>n^{3/4}$, the [conditional expectation](../../../../../conditional-expectation.md) is at most $2b/3$. Taking $u=b/12$ shows that the next count is at most $3b/4$, except with [probability](../../../../../probability.md) at most $e^{-b/288}$. If the count has already fallen below $n^{3/4}$, it stays there. Since $(3/4)^8<1/8$ and $n^{3/4}\leq n/8$, this gives $B_8\leq n/8$ outside the stated exceptional events.
- Starting with $a_0=n/8$, set $a_{r+1}=2a_r^2/n$. If $B\leq a_r$ and $a_r\geq n^{3/4}$, part (a) and the [union bound](../../../../../boole-s-inequality.md) give $\mathbb EF_B\leq a_r^2/n$. Taking $u=a_r^2/n$ gives a next count at most $a_{r+1}$, except with [probability](../../../../../probability.md) at most $e^{-a_r^3/(2n^2)}\leq e^{-n^{1/4}/2}$. The deterministic solution is $a_r=(n/2)4^{-2^r}$. It falls below $n^{3/4}$ within $L$ steps. After reaching that threshold the count cannot increase, so $B_{8+L}\leq n^{3/4}$ outside the exceptional events.
- From $b\leq n^{3/4}$, the next [conditional expectation](../../../../../conditional-expectation.md) is at most $n^{1/2}$. A deviation $u=n^{1/2}$ leaves at most $2n^{1/2}$ balls except with [probability](../../../../../probability.md) $e^{-n^{1/4}/2}$. From at most $2n^{1/2}$ balls, the next [conditional expectation](../../../../../conditional-expectation.md) is at most $4$. Taking $u=n^{1/3}-4\geq n^{1/3}/2$ leaves at most $n^{1/3}$ balls except with [probability](../../../../../probability.md) $e^{-n^{1/6}/16}$. Conditional on this final count bound, one more round has [expectation](../../../../../expected-value-split.md) at most $n^{-1/3}$.

Every exceptional [probability](../../../../../probability.md) above is at most $e^{-n^{1/6}/300}$, and there are at most $L+10$ opportunities for an exception. For $n\geq2^{120}$, the elementary bounds $n^{1/6}/300\geq4\ln n$ and $L+10\leq n$ give, by the [union bound](../../../../../boole-s-inequality.md), total exceptional [probability](../../../../../probability.md) at most $n^{-3}$. The first numerical inequality holds at the cutoff and remains true because $n^{1/6}/\ln n$ is increasing there. On an exceptional history there are at most $n$ balls. Taking the last round's [conditional expectation](../../../../../conditional-expectation.md) and then averaging gives

$$
\boxed{x_{11+L}\leq n^{-1/3}+n\,n^{-3}=n^{-1/3}+n^{-2}<1.}
$$

This proves the displayed replacement $j(n)$ for the literal process without relying on either false assertion.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
