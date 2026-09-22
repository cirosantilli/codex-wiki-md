<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Expose the vertices in order, revealing at step $i$ every [edge](../../../../../edge-of-a-graph.md) from vertex $i$ to an earlier vertex. With the resulting [filtration](../../../../../filtration-probability-theory.md) $\mathcal F_i$, put

$$
M_i=\mathbb E[\chi(G)\mid\mathcal F_i],\qquad M_0=\mu,\quad M_n=\chi(G).
$$

This is the [vertex exposure for chromatic number](../../../../../vertex-exposure-for-chromatic-number.md) [martingale](../../../../../martingale-split.md). Its increments $D_i=M_i-M_{i-1}$ have [conditional mean](../../../../../conditional-expectation.md) zero and satisfy $|D_i|\leq1$, by the permitted [Lipschitz condition](../../../../../lipschitz-continuity.md).

Here is the required exponential-moment proof of the [Azuma-Hoeffding inequality](../../../../../azuma-s-inequality.md). More generally, suppose $|D_i|\leq c_i$ for deterministic $c_i$. [Convexity](../../../../../convex-function.md) of the [exponential function](../../../../../exponential-function.md) gives, for $-c_i\leq d\leq c_i$,

$$
e^{td}\leq\frac{c_i+d}{2c_i}e^{tc_i}+\frac{c_i-d}{2c_i}e^{-tc_i}.
$$

Taking [conditional expectation](../../../../../conditional-expectation.md) and using the zero [conditional mean](../../../../../conditional-expectation.md) yields

$$
\mathbb E[e^{tD_i}\mid\mathcal F_{i-1}]\leq\cosh(tc_i)\leq e^{t^2c_i^2/2}.
$$

For the last inequality, integrate $(\log\cosh u)'=\tanh u\leq u$ for $u\geq0$, and use evenness. A zero $c_i$ simply means a zero increment. Iterated [conditional expectation](../../../../../conditional-expectation.md) now gives

$$
\mathbb E e^{t(M_n-M_0)}\leq\exp\left(\frac{t^2}{2}\sum_i c_i^2\right).
$$

For $s,t>0$, the strict Markov bound on the event $M_n-M_0>s$ gives

$$
\mathbb P(M_n-M_0>s)<\exp\left(-ts+\frac{t^2}{2}\sum_i c_i^2\right).
$$

The strict inequality follows directly by integrating $e^{t(M_n-M_0)}>e^{ts}$ on that event; it is also immediate if the event is empty. Optimize at $t=s/\sum_i c_i^2$ and apply the same argument to the negative increments. For $c_i=1$ and $s=\lambda\sqrt n$, the [union bound](../../../../../boole-s-inequality.md) proves, for every $\lambda>0$,

$$
\boxed{\mathbb P(|\chi(G)-\mu|>\lambda\sqrt n)<2e^{-\lambda^2/2}.}
$$

At $\lambda=0$ the displayed strict bound is trivial.

For the second conclusion write $a_n=n/\log n$ and choose a fixed $C>\sqrt{2\log10}$. If $\mu\geq a_n+C\sqrt n$, then $\{\chi(G)<a_n\}\subseteq\{\chi(G)-\mu<-C\sqrt n\}$, whose [probability](../../../../../probability.md) is less than $e^{-C^2/2}<1/10$. Thus the given positive [probability](../../../../../probability.md) forces $\mu<a_n+C\sqrt n$. For sufficiently large $n$,

$$
\mathbb P\bigl(\chi(G)\geq a_n+(\log n)\sqrt n\bigr)
\leq\exp\left(-\frac{(\log n-C)^2}{2}\right)\longrightarrow0.
$$

Here the non-strict one-sided bound follows by the usual non-strict [Markov inequality](../../../../../markov-inequality.md). Consequently **the asserted upper bound holds [with high probability](../../../../../with-high-probability.md)**, uniformly over any sequence $p=p(n)$ satisfying the stated assumption.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
