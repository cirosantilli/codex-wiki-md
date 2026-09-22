<h1 id="27k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $a=\mu/\lambda<1$. The embedded [birth-death chain](../../../../../../birth-death-chain.md) moves upward with [probability](../../../../../../probability.md) $\lambda/(\lambda+\mu)$ and downward with [probability](../../../../../../probability.md) $\mu/(\lambda+\mu)$ away from zero. The [gambler's ruin](../../../../../../gambler-s-ruin.md) formula, obtained by solving its two-point difference equation on $\{0,\ldots,N\}$ and then letting $N\to\infty$, gives $\mathbb P_k(\text{hit }0)=a^k$. Translation gives return [probability](../../../../../../probability.md) $a$ from $r+1$ to $r$. From $r-1$ the chain hits $r$ almost surely: before that hit it remains in a finite reflecting interval, from every state of which a uniformly positive finite-step chance of hitting $r$ is available. This also proves that starting at zero it hits each $r\ge1$ almost surely.

After departure from $r\ge1$ the return [probability](../../../../../../probability.md) is therefore

$$
r_r=\frac{\lambda}{\lambda+\mu}a+\frac{\mu}{\lambda+\mu}
=\frac{2\mu}{\lambda+\mu}.
$$

The holding rate is $q_r=\lambda+\mu$, so the exponential occupation-time parameter is $q_r(1-r_r)=\lambda-\mu$. Applying the [Strong Markov property](../../../../../../strong-markov-property.md) at the almost-sure first hit gives

$$
\boxed{T_r\sim\operatorname{Exp}(\lambda-\mu),\qquad r\ge1}.
$$

At zero the holding rate is $\lambda$ and return [probability](../../../../../../probability.md) after departure is $a$, again giving parameter $\lambda-\mu$. From initial state $k$, the expected occupation time at zero is $a^k/(\lambda-\mu)$, since the time is zero unless zero is reached. Averaging over the initial law with [probability generating function](../../../../../../probability-generating-function.md) $G$ yields

$$
\boxed{\mathbb E T_0=\frac{G(\mu/\lambda)}{\lambda-\mu}}.
$$

For $\mu=0$, the interpretation is $a^0=1$, $a^k=0$ for $k>0$, and $G(0)=\mathbb P(X(0)=0)$; the same formulas hold.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
