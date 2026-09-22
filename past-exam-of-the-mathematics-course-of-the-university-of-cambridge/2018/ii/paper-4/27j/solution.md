<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

Let $\mathcal F_n=\sigma(X_1,\ldots,X_n)$ be the [natural filtration](../../../../../natural-filtration.md). An integer-valued random variable $M$ is a [stopping time](../../../../../stopping-time.md) with respect to $(X_i)$ when

$$
\boxed{\{M\leq n\}\in\mathcal F_n\quad\text{for every }n}.
$$

Thus whether one has stopped by time $n$ can be decided from the first $n$ observations, without seeing future variables. Equivalently, $\{M\geq i\}\in\mathcal F_{i-1}$.

Write the stopped sum as

$$
\sum_{i=1}^M X_i=\sum_{i=1}^{\infty}X_i\mathbf1_{\{M\geq i\}}.
$$

The event $\{M\geq i\}$ depends only on $X_1,\ldots,X_{i-1}$, so its indicator and $X_i$ are [independent random variables](../../../../../independent-random-variables.md). Since $\mathbb E|X_1|<\infty$ and $\mathbb EM<\infty$, [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\mathbb E\sum_{i=1}^{\infty}|X_i|\mathbf1_{\{M\geq i\}}
=\mathbb E|X_1|\sum_{i=1}^{\infty}\mathbb P(M\geq i)
=\mathbb E|X_1|\,\mathbb EM<\infty.
$$

We may consequently exchange expectation and summation. Using the [tail-sum formula](../../../../../tail-sum-formula.md) for $M$ proves [Wald's equation](../../../../../wald-s-equation.md):

$$
\boxed{
\mathbb E\left[\sum_{i=1}^M X_i\right]
=\sum_{i\geq1}\mu\,\mathbb P(M\geq i)
=\mu\,\mathbb EM
}.
$$

For the [renewal process](../../../../../renewal-process.md), put $S_n=X_1+\cdots+X_n$ and $N_t=\max\{n:S_n\leq t\}$. The random variable $N_t+1$ is a stopping time. Since $S_{N_t+1}>t$, Wald's equation gives

$$
\mu\bigl(m(t)+1\bigr)=\mathbb ES_{N_t+1}>t,
$$

and hence

$$
\liminf_{t\to\infty}\frac{m(t)}t\geq\frac1\mu.
$$

For $c>0$, set $Y_i=X_i\wedge c$ and $\mu_c=\mathbb EY_i$. Wald's equation still applies to the stopping time $N_t+1$ and the independent variables $Y_i$. Because $S_{N_t}\leq t$,

$$
\sum_{i=1}^{N_t+1}Y_i
\leq S_{N_t}+c
\leq t+c.
$$

Therefore

$$
\mu_c\bigl(m(t)+1\bigr)\leq t+c,
\qquad
\limsup_{t\to\infty}\frac{m(t)}t\leq\frac1{\mu_c}.
$$

By the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), $\mu_c\uparrow\mu$ as $c\to\infty$. Combining the bounds proves the [elementary renewal theorem](../../../../../elementary-renewal-theorem.md)

$$
\boxed{\frac{m(t)}t\longrightarrow\frac1\mu}.
$$

For a fixed word over $q$ equally likely symbols, the [waiting time for a word in independent uniform symbols](../../../../../waiting-time-for-a-word-in-independent-uniform-symbols.md) has mean $\sum q^k$, where $k$ runs through the lengths of the [borders of a word](../../../../../border-of-a-word.md), including the full word. The word `lava' has no proper nonempty border, so
$$
\boxed{\mathbb E\tau_{\mathtt{lava}}=100^4=100\,000\,000}.
$$

The word `aa' has borders of lengths $1$ and $2$, so

$$
\boxed{\mathbb E\tau_{\mathtt{aa}}=100+100^2=10\,100}.
$$

For a direct check, let $E_0$ be the expected remaining time with no trailing `a' and $E_1$ with one trailing `a'. Then

$$
E_0=1+\frac1{100}E_1+\frac{99}{100}E_0,
\qquad
E_1=1+\frac{99}{100}E_0,
$$

which gives $E_0=10\,100$.

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
