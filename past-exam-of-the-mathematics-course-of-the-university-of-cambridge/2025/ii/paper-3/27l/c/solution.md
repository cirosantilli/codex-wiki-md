<h1 id="27l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F$ be the distribution function of $\xi_1$, write $\overline F=1-F$, and fix $x>0$. Set

$$
q(t)=\mathbb P(L(t)\geq x).
$$

Conditioning on the first interarrival gives

$$
q(t)=\overline F(\max\{x,t\})
+\int_{[0,t]}q(t-y)\,dF(y).
$$

Indeed, if $\xi_1>t$, the first interval contains $t$ and must also have length at least $x$; if $\xi_1\leq t$, the process starts afresh at time $\xi_1$.

Put $h=\overline F(x)$ and $d(t)=q(t)-h$. Then

$$
d(t)=g(t)+\int_{[0,t]}d(t-y)\,dF(y),
$$

where

$$
g(t)=
\begin{cases}
hF(t),&t\leq x,\\
\overline F(t)F(x),&t>x.
\end{cases}
$$

In particular $g\geq0$. Iterating the renewal equation yields

$$
d(t)=\sum_{n=0}^{m}(g*dF^{*n})(t)
+(d*dF^{*(m+1)})(t).
$$

For fixed $t$, the last term tends to zero in absolute value because $d$ is bounded and

$$
F^{*(m+1)}(t)=\mathbb P(S_{m+1}\leq t)\longrightarrow0.
$$

It follows that

$$
d(t)=\sum_{n=0}^{\infty}(g*dF^{*n})(t)\geq0.
$$

Thus the [stochastic length bias of a renewal interval](../../../../../../stochastic-length-bias-of-a-renewal-interval.md) gives

$$
\boxed{\mathbb P(L(t)\geq x)\geq\mathbb P(\xi_1\geq x)}
$$

for every $x,t>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27L](../../27l.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
