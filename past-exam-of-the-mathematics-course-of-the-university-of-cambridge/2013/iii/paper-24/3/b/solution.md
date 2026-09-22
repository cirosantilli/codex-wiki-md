<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\tau=\tau_x$ and $T_t=t\wedge\tau$. Path continuity gives $|B_{T_t}|\leq x$. Stop the [martingale](../../../../../../martingale-split.md) $B_s^2-s$ at the bounded [stopping time](../../../../../../stopping-time.md) $T_t$ and apply the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md):

$$
\mathbb E T_t=\mathbb E B_{T_t}^2\leq x^2.
$$

By the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), $\mathbb E\tau\leq x^2$, so $\tau<\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Path continuity then gives $B_\tau\in\{-x,x\}$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) for the bounded variables $B_{T_t}^2$ shows

$$
\boxed{\mathbb E\tau_x=x^2.}
$$

Next stop the quartic [Hermite polynomial martingale](../../../../../../space-time-hermite-polynomial.md) from part (a), again only at $T_t$. Its [expectation](../../../../../../expected-value.md) is zero, so

$$
3\mathbb E T_t^2
=6\mathbb E[T_tB_{T_t}^2]-\mathbb E B_{T_t}^4
\leq6x^2\mathbb E T_t\leq6x^4.
$$

[Monotone convergence](../../../../../../monotone-convergence-theorem.md) proves $\mathbb E\tau^2\leq2x^4$, establishing the needed second-moment integrability before the final passage to the limit. Since $T_tB_{T_t}^2\leq x^2\tau$ and $B_{T_t}^4\leq x^4$, [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives

$$
3\mathbb E\tau^2=6x^2\mathbb E\tau-x^4=5x^4.
$$

Consequently the [Brownian symmetric interval-exit moments](../../../../../../brownian-symmetric-interval-exit-moments.md) are

$$
\boxed{\mathbb E\tau_x^2=\frac53x^4,\qquad
\operatorname{Var}(\tau_x)=\frac23x^4.}
$$

To obtain the [Laplace transform of symmetric Brownian interval-exit time](../../../../../../laplace-transform-of-symmetric-brownian-interval-exit-time.md), put $a=\sqrt{2\lambda}$. The [Exponential martingale for Brownian motion](../../../../../../exponential-martingale-for-brownian-motion.md) shows that

$$
H_t=e^{-\lambda t}\cosh(aB_t)
=\tfrac12\bigl(e^{aB_t-a^2t/2}+e^{-aB_t-a^2t/2}\bigr)
$$

is a [martingale](../../../../../../martingale-split.md) with $H_0=1$. Bounded-time stopping gives $\mathbb E H_{T_t}=1$. Its stopped values are bounded by $\cosh(ax)$, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) applies as $t\to\infty$. Since $\cosh(aB_\tau)=\cosh(ax)$, it yields

$$
\boxed{\mathbb E[e^{-\lambda\tau_x}]
=\frac1{\cosh(x\sqrt{2\lambda})}\quad(\lambda>0).}
$$

Every use of stopping at $\tau$ has thus been justified through bounded stopping and an explicit integrability or domination argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
