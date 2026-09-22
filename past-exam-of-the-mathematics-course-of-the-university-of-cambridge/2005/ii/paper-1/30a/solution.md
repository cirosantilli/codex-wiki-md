<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

An [asymptotic power series](../../../../../asymptotic-power-series.md) about $a$ means that for every fixed $N\ge0$,

$$
f(x)-\sum_{k=0}^Nc_k(x-a)^k=o(|x-a|^N)
$$

as $x\to a$ through the specified domain. It makes no assertion that the infinite series converges at nonzero $x-a$. If a [power series](../../../../../power-series.md) converges in a neighbourhood, choose a smaller fixed convergence radius $r$: absolute convergence bounds its tail after $N$ by $|x-a|^{N+1}\sum_{k>N}|c_k|r^{k-N-1}$ for $|x-a|\le r$. Thus a convergent [power series](../../../../../power-series.md) is also asymptotic. The coefficients are unique, successively recovered by

$$
c_0=\lim_{x\to a}f(x),\qquad c_k=\lim_{x\to a}\frac{f(x)-\sum_{j<k}c_j(x-a)^j}{(x-a)^k}.
$$

If two expansions first differed at index $k$, division of their difference by $(x-a)^k$ would contradict this limit.

For the given [integral](../../../../../integral.md), use the exact finite identity $1/(1+2xt)=\sum_{k=0}^{n-1}(-2xt)^k+(-2xt)^n/(1+2xt)$. The gamma [integral](../../../../../integral.md) gives

$$
\frac1{\sqrt\pi}\int_0^\infty e^{-x}x^{k-1/2}dx=\frac{\Gamma(k+1/2)}{\sqrt\pi}=\frac{1\cdot3\cdots(2k-1)}{2^k}.
$$

Consequently

$$
f(t)=\sum_{k=0}^{n-1}(-1)^k(2k-1)!!\,t^k+R_n(t),\qquad R_n(t)=\frac{(-2t)^n}{\sqrt\pi}\int_0^\infty\frac{e^{-x}x^{n-1/2}}{1+2xt}\,dx.
$$

For $t\ge0$ the denominator is at least one, so

$$
\boxed{|R_n(t)|\le(2n-1)!!\,t^n,\qquad f(t)\sim\sum_{k\ge0}(-1)^k(2k-1)!!\,t^k\quad(t\to0^+).}
$$

The empty product for $k=0$ is one. The bound is exactly the magnitude of the next omitted term. For the asymptotic definition through degree $N$, take $n=N+1$, giving an $O(t^{N+1})$ remainder. Only a finite expansion was integrated; interchanging a divergent infinite series with the [integral](../../../../../integral.md) would be invalid. Indeed the ratio of consecutive term magnitudes is $(2k+1)t$, so this formal series diverges at every fixed $t>0$.

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
