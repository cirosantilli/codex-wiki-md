<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M_t=\max_{0\leq s\leq t}B_s$. The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives

$$
\mathbb P(M_t>1)=2\mathbb P(B_t>1).
$$

Here is the reflection argument: on paths that hit $1$ before $t$, reflect all increments after their first hitting time. The [Strong Markov property](../../../../../../strong-markov-property.md) gives [independent](../../../../../../independent-random-variables.md) [Brownian motion](../../../../../../brownian-motion-split.md) after that time, whose sign can be reversed without changing its law. This exchanges paths ending below $1$ with paths ending above $1$. The latter have necessarily hit $1$, and the endpoint has no atom at $1$, giving the displayed equality. It also shows that $M_t$ has a continuous distribution at every positive level.

Writing $\Phi$ for the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md), the [probability](../../../../../../probability.md) of staying below the barrier is therefore

$$
\mathbb P(B_s\leq1\text{ for all }s\leq t)=2\Phi(t^{-1/2})-1.
$$

Since $\Phi(h)-\Phi(0)\sim h/\sqrt{2\pi}$ as $h\downarrow0$, the [Brownian barrier survival asymptotic](../../../../../../brownian-barrier-survival-asymptotic.md) is

$$
\boxed{\alpha=\tfrac12,\qquad \lim_{t\to\infty}\sqrt t\,\mathbb P(B_s\leq1\text{ for all }s\leq t)=\sqrt{\frac2\pi}.}
$$

Any smaller exponent gives a zero limit and any larger exponent gives an infinite limit, so this is the unique exponent producing a finite positive constant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
