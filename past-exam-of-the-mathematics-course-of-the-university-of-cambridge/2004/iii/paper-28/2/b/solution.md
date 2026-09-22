<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First the exit time has sufficiently many finite moments. Over any interval of length $a^2$, a [Brownian motion](../../../../../../brownian-motion-split.md) increment has probability $q=\mathbb P(|B_{a^2}|>2a)>0$ of absolute size larger than $2a$. If the process is still inside $(-a,a)$, such an increment forces it to exit before the next interval endpoint. [Independence](../../../../../../independent-random-variables.md) of increments at deterministic times therefore gives

$$
\mathbb P(T>ka^2)\leq(1-q)^k.
$$

Thus $T<\infty$ [almost surely](../../../../../../almost-sure-convergence.md) and all its positive moments are finite. This justifies extracting moments from its transform rather than presupposing them.

For $\lambda>0$, put $\theta=\sqrt{2\lambda}$. The process

$$
M_t=e^{-\lambda t}\cosh(\theta B_t)
=\frac12\left(e^{\theta B_t-\theta^2t/2}+e^{-\theta B_t-\theta^2t/2}\right)
$$

is a [martingale](../../../../../../martingale-split.md), being the average of two [exponential martingales for Brownian motion](../../../../../../exponential-martingale-for-brownian-motion.md). Apply the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the bounded time $T\wedge t$. Since $|B_{T\wedge t}|\leq a$, the stopped values are bounded by $\cosh(\theta a)$. Continuity gives $B_T\in\{-a,a\}$. Letting $t\to\infty$ by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) yields

$$
1=\mathbb E[e^{-\lambda T}\cosh(\theta B_T)]
=\cosh(a\sqrt{2\lambda})\,\mathbb Ee^{-\lambda T}.
$$

Hence the [Laplace transform of symmetric Brownian interval-exit time](../../../../../../laplace-transform-of-symmetric-brownian-interval-exit-time.md) is

$$
\boxed{\phi_T(\lambda)=\frac1{\cosh(a\sqrt{2\lambda})},\qquad\lambda\geq0.}
$$

The value at zero follows from almost-sure finiteness. Expanding the reciprocal gives

$$
\phi_T(\lambda)=1-a^2\lambda+\frac56a^4\lambda^2+O(\lambda^3).
$$

Compare with part (a), now applicable because of the geometric tail bound. The [Brownian symmetric interval-exit moments](../../../../../../brownian-symmetric-interval-exit-moments.md) are

$$
\boxed{\mathbb ET=a^2,\qquad\mathbb ET^2=\frac53a^4,\qquad
\operatorname{Var}(T)=\frac23a^4.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
