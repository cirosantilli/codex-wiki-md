<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first condition is that $X$ is Markov with transition semigroup  
$P(t)=e^{tQ}$. The second is that, for every function  
$f:S\to\mathbb R$,

$$
M_t^f=f(X_t)-f(X_0)-\int_0^t(Qf)(X_s)\,ds
$$

is a martingale.

The first condition implies the second by conditioning over a short time interval, using  
$P(h)f=f+hQf+o(h)$, summing increments, and passing to the limit. This is Dynkin's formula.

Conversely assume the [martingale problem for a continuous-time Markov chain](../../../../../../martingale-problem-for-a-continuous-time-markov-chain.md). Fix $T>0$ and a function $f$, and put

$$
u(t,x)=(e^{(T-t)Q}f)(x).
$$

The backward equation gives $\partial_tu+Qu=0$. Applying the martingale identity to this time-dependent function shows that $u(t,X_t)$ is a martingale. Therefore, for $s\leq T$,

$$
\mathbb E[f(X_T)\mid\mathcal F_s]
=u(s,X_s)=(e^{(T-s)Q}f)(X_s).
$$

Taking indicator functions $f$ proves both the Markov property and the transition semigroup $e^{tQ}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
