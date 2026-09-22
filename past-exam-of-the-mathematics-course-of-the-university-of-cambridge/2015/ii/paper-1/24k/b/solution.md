<h1 id="24k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The number present is an [M-M-s queue](../../../../../../m-m-s-queue.md): births occur at rate $\lambda$, deaths at rate $\mu\min(n,s)$. Both rates are bounded, so the chain is nonexplosive. For $\lambda,\mu>0$ and an integer $s\geq1$, the detailed-balance weights with $\pi_0=1$ are

$$
\pi_n=\frac{(\lambda/\mu)^n}{n!}\quad(0\leq n\leq s),\qquad
\pi_n=\frac{(\lambda/\mu)^s}{s!}\left(\frac\lambda{s\mu}\right)^{n-s}\quad(n\geq s).
$$

Their sum is finite precisely when $\lambda<s\mu$, giving **positive recurrence** and a stationary [probability distribution](../../../../../../probability-distribution.md) after normalization.

For completeness, the birth–death recurrence criterion is $\sum_{n\geq0}(\lambda_n\pi_n)^{-1}=\infty$. It follows by solving the harmonic hitting-probability recurrence: successive differences are proportional to $(\lambda_n\pi_n)^{-1}$, and divergence makes the probability of escaping to infinity before reaching zero vanish. The geometric tail of the weights makes this sum diverge when $\lambda\leq s\mu$ and converge when $\lambda>s\mu$. Thus **$\lambda=s\mu$ gives null recurrence**, since the chain is recurrent but has no finite invariant normalization, and **$\lambda>s\mu$ gives transience**. The critical case is not positive recurrent merely because arrival and maximum service rates balance.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24K](../../24k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
