<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Within the approximation that a factory has either zero or one accident, let $N$ be the accident count. The factories' independence gives $N\sim\operatorname{Binomial}(m,p)$. Given an accident, its cluster of claims has a [Poisson distribution](../../../../../../poisson-distribution.md) of mean $\lambda$, independently across factories. Its [probability generating function](../../../../../../probability-generating-function.md) is $G_X(z)=e^{\lambda(z-1)}$. Thus this is a [binomial accident portfolio with Poisson clusters](../../../../../../binomial-accident-portfolio-with-poisson-clusters.md), with

$$
G_S(z)=\left(q+pe^{\lambda(z-1)}\right)^m,\qquad\boxed{\mathbb P(S=0)=\left(q+pe^{-\lambda}\right)^m.}
$$

A factory can contribute no claims either because it has no accident or because its accident's Poisson cluster is empty. Hence the no-claim probability differs from the no-accident probability $q^m$.

For $0\leq n\leq m$, the accident [probability mass function](../../../../../../probability-mass-function.md) is $p_n=\binom mn p^nq^{m-n}$. For $1\leq n\leq m$,

$$
\frac{p_n}{p_{n-1}}=\frac{m-n+1}{n}\frac pq=-\frac pq+\frac{(m+1)p}{nq}.
$$

Therefore its [Panjer claim-count class](../../../../../../panjer-claim-count-class.md) parameters are

$$
\boxed{a=-\frac pq,\qquad b=\frac{(m+1)p}{q}.}
$$

At $n=m+1$ the multiplier is zero, and afterwards both successive masses are zero, so the recurrence holds for all $n\geq1$. Finally, $f_0=e^{-\lambda}$ and $G_N(z)=(q+pz)^m$ reproduce the same initialization $g_0=G_N(f_0)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
