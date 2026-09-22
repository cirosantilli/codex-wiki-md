<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $t>0$, put $M_t=\sup_{0\leq s\leq t}B_s$. For $\lambda>0$, reflect the Brownian path after its first hit of $\lambda$. The [Strong Markov property](../../../../../../strong-markov-property.md) and symmetry of subsequent [Brownian increments](../../../../../../brownian-increment.md) make this reflection preserve the path distribution. It exchanges the events $\{M_t\geq\lambda,B_t<\lambda\}$ and $\{B_t>\lambda\}$. Since $B_t$ has no atom at $\lambda$, the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives

$$
\boxed{\mathbb P(M_t>\lambda)=2\mathbb P(B_t>\lambda)=2\bigl(1-\Phi(\lambda/\sqrt t)\bigr),\qquad t>0,\ \lambda\geq0.}
$$

The case $\lambda=0$ follows by decreasing positive levels to zero: the [probability](../../../../../../probability.md) is one. At $t=0$, $M_0=0$ and the [probability](../../../../../../probability.md) is zero for every $\lambda\geq0$.

The displayed tail probabilities are exactly those of $|B_t|$, so $M_t$ has the [half-normal distribution](../../../../../../half-normal-distribution.md) of $\sqrt t\,|Z|$ with $Z\sim N(0,1)$. Thus

$$
\boxed{\|M_t\|_2=\sqrt{\mathbb E B_t^2}=\sqrt t,\qquad t\geq0.}
$$

For $A_t=\sup_{s\leq t}|B_s|$, the pointwise inequality $A_t\geq M_t$ gives the lower non-strict bound. To prove strictness when $t>0$, fix $\lambda>0$. Reflection at $\lambda$ also gives

$$
\mathbb P(B_t<-\lambda,M_t\geq\lambda)=\mathbb P(B_t>3\lambda).
$$

Subtracting this from $\mathbb P(B_t<-\lambda)=\mathbb P(B_t>\lambda)$ gives

$$
\mathbb P(B_t<-\lambda,M_t<\lambda)
=\mathbb P(B_t>\lambda)-\mathbb P(B_t>3\lambda)>0.
$$

On this event $A_t\geq|B_t|>\lambda>M_t$, so $A_t^2-M_t^2$ is strictly positive with positive [probability](../../../../../../probability.md). Finally, $|B_t|$ is a continuous nonnegative [submartingale](../../../../../../submartingale.md) by the conditional [Jensen inequality](../../../../../../jensen-s-inequality.md), and part (a) gives $\|A_t\|_2\leq2\|B_t\|_2=2\sqrt t$. Its square is therefore integrable, and the strict pointwise comparison on a positive-probability event gives

$$
\boxed{\sqrt t<\|A_t\|_2\leq2\sqrt t\quad(t>0).}
$$

This is the [strict comparison of one-sided and absolute Brownian maxima](../../../../../../strict-comparison-of-one-sided-and-absolute-brownian-maxima.md). The strict lower inequality printed with $t\geq0$ needs the qualification $t>0$: at $t=0$ both maxima vanish and all three quantities are zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
