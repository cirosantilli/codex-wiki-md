<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $\lambda>0$ and choose the positive root

$$
\theta=b+\sqrt{b^2+2\lambda}>0,\qquad \frac{\theta^2}{2}-b\theta=\lambda.
$$

Use the [Exponential martingale for Brownian motion](../../../../../../exponential-martingale-for-brownian-motion.md) $M_t=\exp(\theta B_t-\theta^2t/2)$. Before the linear-boundary [stopping time](../../../../../../stopping-time.md) $\tau$, path continuity gives $B_s<a+bs$. At the boundary there is equality. Consequently

$$
0\leq M_{t\wedge\tau}\leq e^{\theta a}e^{-\lambda(t\wedge\tau)}\leq e^{\theta a}.
$$

The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the bounded [stopping time](../../../../../../stopping-time.md) $t\wedge\tau$ yields $\mathbb E M_{t\wedge\tau}=1$. Separate the two events:

$$
1=e^{\theta a}\mathbb E[e^{-\lambda\tau}\mathbf1_{\{\tau\leq t\}}]+\mathbb E[M_t\mathbf1_{\{\tau>t\}}].
$$

The last term is at most $e^{\theta a-\lambda t}$ and tends to zero. The first term converges by the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). Taking $e^{-\lambda\infty}=0$ therefore proves

$$
\boxed{\mathbb E e^{-\lambda\tau}=\exp\!\left[-a\left(b+\sqrt{b^2+2\lambda}\right)\right].}
$$

This bounded-stopping argument does not assume in advance that $\tau$ is finite. For $b\leq0$, letting $\lambda\downarrow0$ makes the right side tend to one, so it also proves $\mathbb P(\tau<\infty)=1$. Setting $b=0$ gives the [Brownian first-passage Laplace transform](../../../../../../brownian-first-passage-laplace-transform.md)

$$
\boxed{\varphi_a(\lambda)=e^{-a\sqrt{2\lambda}},\qquad\lambda\geq0,\qquad C=\sqrt2.}
$$

The zero-parameter value follows from the just-proved almost-sure finiteness.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
