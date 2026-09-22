<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative [random variable](../../../../../random-variable-split.md) $Y$ and $a>0$, [Markov inequality](../../../../../markov-s-inequality.md) states

$$
P(Y\geq a)\leq\frac{\mathbb EY}{a}.
$$

For a [random variable](../../../../../random-variable-split.md) $X$ of finite mean $\mu$ and [variance](../../../../../variance-split.md) $\sigma^2$, [Chebyshev inequality](../../../../../chebyshev-s-inequality.md) states that for every $t>0$,

$$
\boxed{P(|X-\mu|\geq t)\leq\frac{\sigma^2}{t^2}.}
$$

To prove it, apply [Markov inequality](../../../../../markov-s-inequality.md) to the nonnegative variable $(X-\mu)^2$ at threshold $t^2$:

$$
P(|X-\mu|\geq t)=P((X-\mu)^2\geq t^2)
\leq\frac{\mathbb E[(X-\mu)^2]}{t^2}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
