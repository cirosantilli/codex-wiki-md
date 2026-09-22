# Difference of two independent uniform random variables

↑ **Parent:** [Triangular distribution](triangular-distribution.md)

If $U,V$ are [independent random variables](independent-random-variables.md), each with the [uniform distribution](continuous-uniform-distribution.md) on $[0,a]$ for $a>0$, then $T=U-V$ has the symmetric [triangular distribution](triangular-distribution.md)

$$
q(t)=\begin{cases}(a-|t|)/a^2,&|t|<a,\\0,&|t|\geq a.\end{cases}
$$

The [convolution of probability densities](convolution-of-independent-random-variables.md) gives $q(t)=a^{-2}\int\mathbf1_{[0,a]}(s)\mathbf1_{[0,a]}(s+t)\,ds$. The overlap of these two [intervals](interval-mathematics.md) has length $a-|t|$ for $|t|<a$ and is empty otherwise, proving the formula. By [linearity of expectation](linearity-of-expectation.md) and the [variance of a sum](variance-of-a-sum.md),

$$
\mathbb E[T]=0,\qquad\operatorname{Var}(T)=a^2/6.
$$

For $0\leq b\leq a$, its upper-tail [probability](probability.md) is $(a-b)^2/(2a^2)$.

A useful model for elapsed time measured from two independently truncated clock readings uses $a$ as the display resolution and $T$ as the endpoint-offset difference. Independence is essential: uniform marginal [probability distributions](probability-distribution-split.md) alone do not imply this [triangular distribution](triangular-distribution.md). For example $U=V$ gives $T=0$ with certainty. In general, with the same uniform marginals, $\operatorname{Var}(U-V)=a^2/6-2\operatorname{Cov}(U,V)$.

## ↑ Ancestors (8)

1. [Triangular distribution](triangular-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
