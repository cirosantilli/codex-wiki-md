<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The random-walk form of the [Skorokhod embedding theorem](../../../../../../skorokhod-embedding-theorem.md) says the following. If $S_n=Y_1+\cdots+Y_n$, where the $Y_i$ are independent and identically distributed with

$$
\mathbb EY_i=0,
\qquad
\mathbb EY_i^2=\sigma^2<\infty,
$$

then on a space carrying a Brownian motion $B$ there are stopping times

$$
0=T_0\leq T_1\leq\cdots
$$

such that $(B_{T_n})_{n\geq0}$ has the same law as $(S_n)_{n\geq0}$, and the increments $T_n-T_{n-1}$ are independent and identically distributed with mean $\sigma^2$.

To prove the one-step statement, first note that every centered distribution is a mixture of centered two-point distributions. Indeed, match the equal-mass size-biased measures $x\,\mathbb P(Y\in dx)$ on $(0,\infty)$ and $|x|\,\mathbb P(Y\in dx)$ on $(-\infty,0)$. This produces a random pair $(L,R)$ of positive numbers such that, conditionally on $(L,R)$, $Y$ has values $-L,R$ with probabilities

$$
\frac R{L+R},\qquad\frac L{L+R},
$$

and $\mathbb E[LR]=\mathbb EY^2=\sigma^2$. Include the atom at zero by taking the stopping time zero.

Choose $(L,R)$ independently of $B_t$ and stop Brownian motion on first leaving $(-L,R)$. The [Brownian exit from an interval](../../../../../../brownian-exit-from-an-interval.md) formulas give the displayed two-point probabilities and conditional mean stopping time $LR$. Thus $B_T$ has the law of $Y$ and $\mathbb ET=\sigma^2$.

Starting from $T_0=0$, repeat this construction after each $T_{n-1}$. The [Strong Markov property](../../../../../../strong-markov-property.md) makes the new Brownian increments independent copies of the first embedding, proving the [Skorokhod embedding of a centered random walk](../../../../../../skorokhod-embedding-of-a-centered-random-walk.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
