<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the exit law, the two identified processes have the same argument. Starting at zero, neither can skip $-a$ or $b$: [Brownian motion](../../../../../brownian-motion-split.md) is continuous, and the [symmetric Poisson difference process](../../../../../symmetric-poisson-difference-process.md) has unit jumps with integer boundary levels. Therefore $|X_{t\wedge T}|\leq K=\max(a,b)$, and if $T$ is finite, $X_T\in\{-a,b\}$.

To justify finiteness rather than presume it, apply the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the [martingale](../../../../../martingale-split.md) $X_t^2-t$ at the bounded [stopping time](../../../../../stopping-time.md) $t\wedge T$:

$$
\mathbb E(t\wedge T)=\mathbb E X_{t\wedge T}^2\leq K^2.
$$

The first boundary [hitting time](../../../../../first-passage-time.md) is a [stopping time](../../../../../stopping-time.md) in both cases: in the continuous case use the continuous-path hitting criterion, and in the jump case inspect the successive jump times. [Monotone convergence](../../../../../monotone-convergence-theorem.md) now gives $\mathbb E T\leq K^2$, so $T<\infty$ almost surely. The stopped position tends to $X_T$ as $t\to\infty$ and is bounded, making [dominated convergence](../../../../../dominated-convergence-theorem.md) applicable. Stopping $X$ at $t\wedge T$ and taking this limit yields $\mathbb E X_T=0$.

If $\pi=\mathbb P(X_T=-a)$, then $0=-a\pi+b(1-\pi)$. Thus in both cases the entire distribution is

$$
\boxed{\mathbb P(X_T=-a)=\frac{b}{a+b},\qquad
\mathbb P(X_T=b)=\frac{a}{a+b}.}
$$

This is the same balanced [gambler's ruin](../../../../../gambler-s-ruin.md) law despite the different one-time distributions. As a further consistency check, passing to the limit in the stopped square-martingale identity gives

$$
\mathbb E T=\mathbb E X_T^2=a^2\frac{b}{a+b}+b^2\frac{a}{a+b}=ab.
$$

All uses of an unbounded exit time were obtained by limits of bounded-time sampling with an explicit bound on the stopped position.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
