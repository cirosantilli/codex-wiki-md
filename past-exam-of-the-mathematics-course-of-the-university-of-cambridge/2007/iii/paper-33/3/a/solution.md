<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $\sigma_1>n$, all the integer-time positions through $n$ lie in $(-1,1)$, so every increment over an intervening unit interval has absolute value at most two. The unit-time increments of [Brownian motion](../../../../../../brownian-motion-split.md) are independent standard [normal random variables](../../../../../../gaussian-random-variable.md). Put

$$
\rho=\mathbb P(|N(0,1)|\leq2)=2\Phi(2)-1\in(0,1).
$$

The inclusion of events and [independence](../../../../../../independent-random-variables.md) give

$$
\boxed{\mathbb P(\sigma_1>n)\leq\rho^n\quad(n\geq0).}
$$

In particular $\sigma_1$ is finite almost surely. For real $t\geq0$, its tail is at most $\rho^{\lfloor t\rfloor}$. The [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md) therefore gives, for every $p>0$,

$$
\mathbb E\sigma_1^p=p\int_0^\infty t^{p-1}\mathbb P(\sigma_1>t)\,dt
\leq p\sum_{j=0}^\infty\rho^j\int_j^{j+1}t^{p-1}\,dt<\infty.
$$

An exponential geometric factor dominates the polynomial factors in this sum. This proves the requested moment finiteness for $p>1$, and in fact for every positive $p$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
