<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Markov's inequality](../../../../../markov-s-inequality.md) states that for $Y\geq0$ and $t>0$, $\mathbb P(Y\geq t)\leq\mathbb E Y/t$. It follows by taking expectations in $Y\geq t\mathbf1_{\{Y\geq t\}}$.

If $X$ has finite [mean](../../../../../expected-value-split.md) $\mu$ and [variance](../../../../../variance-split.md) $\sigma^2$, apply Markov to $(X-\mu)^2$ to obtain [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md):

$$
\boxed{\mathbb P(|X-\mu|\geq t)\leq\frac{\sigma^2}{t^2}\qquad(t>0).}
$$

For the [first moment method](../../../../../first-moment-method.md), assume $\mu_n=\mathbb E X_n\to0$. Nonnegative [integer](../../../../../integer-split.md) values give $\{X_n>0\}=\{X_n\geq1\}$, so

$$
\boxed{\mathbb P(X_n>0)\leq\mathbb E X_n\longrightarrow0.}
$$

For a standard [second moment method](../../../../../second-moment-method.md), suppose $\mu_n>0$ eventually, the [second moments](../../../../../second-moment.md) are finite, and $\mathbb E X_n^2/\mu_n^2\to1$. Equivalently, $\operatorname{Var}(X_n)/\mu_n^2\to0$. The zero [event](../../../../../event.md) is contained in $\{|X_n-\mu_n|\geq\mu_n\}$, so

$$
\mathbb P(X_n=0)\leq\frac{\operatorname{Var}(X_n)}{\mu_n^2}\longrightarrow0.
$$

Hence $\boxed{\mathbb P(X_n>0)\to1}$. The second-moment condition controls the fluctuations relative to the [mean](../../../../../expected-value-split.md); a large [mean](../../../../../expected-value-split.md) alone is insufficient.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
