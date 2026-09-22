<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\sigma_N=\sqrt{Np(1-p)}$ and use the [floor function](../../../../../../floor-function.md) to choose

$$
\boxed{k_a(N)=\max\{0,\lfloor Np+a\sigma_N\rfloor+1\},\qquad
k_b(N)=\min\{N,\lfloor Np+b\sigma_N\rfloor\}.}
$$

Interpret an empty integer interval as an empty sum. These bounds give exactly the event $a<(K_N-Np)/\sigma_N\leq b$, where $K_N$ has the [binomial distribution](../../../../../../binomial-distribution.md) of parameters $N,p$. Since $0<p<1$, the [central limit theorem](../../../../../../central-limit-theorem.md) for a sum of [independent](../../../../../../independent-random-variables.md) [Bernoulli distribution](../../../../../../bernoulli-distribution.md) variables gives [convergence in distribution](../../../../../../convergence-in-distribution.md) of that standardized count to the [standard normal distribution](../../../../../../standard-normal-distribution.md). Its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is continuous at both endpoints, so

$$
\boxed{\sum_{k=k_a(N)}^{k_b(N)}p_k(N,p)
\longrightarrow\Phi(b)-\Phi(a)
=\frac1{\sqrt{2\pi}}\int_a^be^{-u^2/2}\,du.}
$$

The TeX's additional malformed inequality involving $p/k_a(N)$ and $p/k_b(N)$ is absent from the PDF and is not a condition on the requested integers.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
