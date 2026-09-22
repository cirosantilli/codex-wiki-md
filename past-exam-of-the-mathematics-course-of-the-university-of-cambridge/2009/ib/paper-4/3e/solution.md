<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

[Uniform convergence](../../../../../uniform-convergence.md) means that for every $\varepsilon>0$ there is $N$ such that $|s_n(x)-s(x)|<\varepsilon$ for every $x\in\mathbb R$ and every $n\geq N$. Equivalently, $\sup_x|s_n(x)-s(x)|\to0$. The nonzero constant functions $s_n=1/n$ converge uniformly to zero. In contrast, the continuous moving bumps $s_n(x)=\max(0,1-|x-n|)$ converge pointwise to zero but have supremum one for every $n$.

On the compact interval,

$$
\left|\int_{-1}^1s_n(x)\,dx-\int_{-1}^1s(x)\,dx\right|
\leq2\sup_{x\in\mathbb R}|s_n(x)-s(x)|\longrightarrow0.
$$

Thus [uniform convergence](../../../../../uniform-convergence.md) permits the stated interchange with integration.

Choose $\boxed{s(x)=1/(1+|x|)}$. It is continuous, nonnegative and tends to zero at infinity, but its improper integral diverges logarithmically. This even choice also makes the prescribed cutoff continuous at both $n$ and $-n$: beyond either endpoint it remains at $s(n)$ for another unit of distance and then decreases as $s(n)/(|x|-n)^2$.

Inside $[-n,n]$, $s_n=s$. Outside, both functions lie between zero and $1/(n+1)$, so $\sup_x|s_n-s|\leq1/(n+1)\to0$. Nevertheless each cutoff has finite integral:

$$
\boxed{\int_{\mathbb R}s_n(x)\,dx
=2\log(n+1)+\frac{2}{n+1}\int_0^\infty\min(1,t^{-2})\,dt
=2\log(n+1)+\frac4{n+1}.}
$$

Here the value of the minimum at $t=0$ is its continuous limiting value one. This example shows that [uniform convergence](../../../../../uniform-convergence.md) on an unbounded domain does not by itself ensure convergence of the integrals over that domain.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
