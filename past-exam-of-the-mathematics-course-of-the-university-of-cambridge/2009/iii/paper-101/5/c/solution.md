<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

As in the intended independent-mark construction, take the entire sequence $(X_j)$ [independent](../../../../../../independent-random-variables.md) of the [Poisson process](../../../../../../poisson-process.md), not merely independent of one fixed count. Then $Y$ is a [Compound Poisson process](../../../../../../compound-poisson-process.md). For deterministic $s<t$, its increment $Y_t-Y_s$ is [independent](../../../../../../independent-random-variables.md) of $\mathcal F_s=\sigma(Y_u:0\leq u\leq s)$. To justify this carefully, first condition on $N_s=k$. The past of $Y$ uses only the counting history up to $s$ and marks among $X_1,\ldots,X_k$. The future count has [independent](../../../../../../independent-random-variables.md) rate-$\lambda$ [Poisson process](../../../../../../poisson-process.md) increments, and future marks $X_{k+1},X_{k+2},\ldots$ are fresh with the common law. Their joint conditional law is the same for every $k$ and every past history, so the increment is independent even of this larger marked history, hence of $\mathcal F_s$. Marks equal to zero do not cause a problem: $\mathcal F_s$ may then reveal less than the full counting history.

By part (b), with Poisson parameter $\lambda(t-s)$,

$$
\mathbb E e^{-q(Y_t-Y_s)}
=\exp\{\lambda(t-s)[\phi(q)-1]\}.
$$

The proposed process is adapted to $\mathcal F_t$, nonnegative, and

$$
\mathbb E|Z_t|=e^{\lambda t[1-\phi(q)]}\mathbb E e^{-qY_t}=1<\infty.
$$

In particular, no finite [expectation](../../../../../../expected-value.md) of a mark is required. Also $Z_s>0$, and

$$
\frac{Z_t}{Z_s}
=\exp\{-q(Y_t-Y_s)+\lambda(t-s)[1-\phi(q)]\}
$$

is [independent](../../../../../../independent-random-variables.md) of $\mathcal F_s$ and has mean one. Therefore the [exponential Laplace martingale of a compound Poisson process](../../../../../../exponential-laplace-martingale-of-a-compound-poisson-process.md) satisfies

$$
\boxed{\mathbb E[Z_t\mid\mathcal F_s]
=Z_s\,\mathbb E[Z_t/Z_s]=Z_s\qquad(0\leq s<t).}
$$

This proves every condition for a [continuous-time martingale](../../../../../../continuous-time-martingale.md) in the requested [filtration](../../../../../../filtration-probability-theory.md). When $q=0$, $\phi(0)=1$ and the same conclusion reduces to the constant [martingale](../../../../../../martingale-split.md) $Z_t=1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
