<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The exit time $T$ is finite [almost surely](../../../../../almost-sure-convergence.md). Indeed, if the [Brownian motion](../../../../../brownian-motion-split.md) is still in $(-b,a)$ at an integer time, its next unit increment exceeds $a+b$ with a fixed probability $p>0$ independent of the past; on this event it must exit before the next integer time. Consequently $\mathbb P(T>n)\leq(1-p)^n\to0$. Path [continuity](../../../../../continuous-function.md) gives $B_T\in\{a,-b\}$, and the two exit events partition the [probability space](../../../../../probability-space.md) up to null sets.

For each real $\lambda$, the [exponential Brownian martingale](../../../../../exponential-brownian-martingale.md) $Z_t^\lambda=\exp(\lambda B_t-\lambda^2t/2)$ has expectation one. This follows directly from the [moment-generating function of a normal distribution](../../../../../moment-generating-function-of-a-normal-distribution.md) and [independent increments](../../../../../independent-increments.md). At $t\wedge T$ its value is bounded by $e^{|\lambda|\max(a,b)}$. Bounded-time [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) and then [dominated convergence](../../../../../dominated-convergence-theorem.md) therefore give

$$
1=\mathbb E e^{\lambda B_T-\lambda^2T/2}.
$$

Write $p_\lambda=\mathbb E[e^{-\lambda^2T/2}\mathbf1_{\{T=T_a\}}]$ and $q_\lambda=\mathbb E[e^{-\lambda^2T/2}\mathbf1_{\{T=T_{-b}\}}]$. Applying the identity to $\lambda$ and $-\lambda$ yields

$$
e^{\lambda a}p_\lambda+e^{-\lambda b}q_\lambda=1,\qquad
e^{-\lambda a}p_\lambda+e^{\lambda b}q_\lambda=1.
$$

For $\lambda\ne0$, multiply the first equation by $e^{\lambda b}$, the second by $e^{-\lambda b}$, and subtract. Solving the resulting system gives

$$
\boxed{p_\lambda=\frac{\sinh(\lambda b)}{\sinh(\lambda(a+b))},\qquad q_\lambda=\frac{\sinh(\lambda a)}{\sinh(\lambda(a+b))}.}
$$

Adding and using the sum formula for the [hyperbolic sine](../../../../../hyperbolic-sine.md) gives the [asymmetric Brownian interval-exit transform](../../../../../asymmetric-brownian-interval-exit-transform.md):

$$
\boxed{\mathbb E e^{-\lambda^2T/2}
=\frac{\sinh(\lambda a)+\sinh(\lambda b)}{\sinh(\lambda(a+b))}
=\frac{\cosh(\lambda(a-b)/2)}{\cosh(\lambda(a+b)/2)}.}
$$

At $\lambda=0$, the printed sine ratio is $0/0$ and needs its removable extension. [Dominated convergence](../../../../../dominated-convergence-theorem.md) as $\lambda\to0$ gives

$$
\boxed{\mathbb P(T=T_a)=\frac b{a+b},\qquad\mathbb P(T=T_{-b})=\frac a{a+b},\qquad\mathbb E e^0=1.}
$$

Thus the formulas hold for every real parameter with this endpoint convention. The expectation on the left of the first formula is legible in the original PDF; the converted TeX's nested exponential is an OCR error.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
