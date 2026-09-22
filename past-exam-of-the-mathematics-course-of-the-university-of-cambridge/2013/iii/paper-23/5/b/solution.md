<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the matrix $A_{r,n}=e(nx_r)$, [operator norm duality](../../../../../../operator-norm-duality.md) gives $\|A\|=\|A^*\|$. Thus the [analytic large sieve inequality](../../../../../../exponential-sum-large-sieve.md)

$$
\sum_r\left|\sum_{M<n\le M+N}a_ne(nx_r)\right|^2
\le C(N+\delta^{-1})\sum_n|a_n|^2
$$

is equivalent to the dual bound with the roles of $a_n$ and $b_r$ exchanged and the conjugate exponential. The absolute constant is independent of all the parameters.

Here is a [Fejér-kernel proof of the analytic large sieve](../../../../../../fejer-kernel-proof-of-the-analytic-large-sieve.md). Choose an [integer](../../../../../../integer.md) center $c$ of the summation interval and an [integer](../../../../../../integer.md) $m\asymp N+1$ large enough that the triangular weights $w_n=(1-|n-c|/m)_+$ are at least $1/2$ throughout it. Their Fourier kernel is $e(c\theta)F_m(\theta)$, with

$$
F_m(\theta)=\frac1m\left(\frac{\sin\pi m\theta}{\sin\pi\theta}\right)^2
\le C\min\left(m,\frac1{m\|\theta\|^2}\right),\qquad F_m(0)=m.
$$

For fixed $r$, spacing allows at most a bounded number of points at each successive distance $j\delta$. Splitting at $j\asymp1/(m\delta)$ gives the row bound

$$
\sum_s|F_m(x_r-x_s)|\le C(m+\delta^{-1}).
$$

In detail the near terms contribute at most $Cm/(m\delta)=C/\delta$, and the square-decay tail contributes $C/(m\delta^2)\sum_{j>1/(m\delta)}j^{-2}\le C/\delta$; when $m\delta\ge1$, the tail is bounded directly by $C/\delta$.

Expand the weighted dual square sum. Its matrix entries have the kernel just estimated. The symmetric row bound, or $2|b_rb_s|\le|b_r|^2+|b_s|^2$, bounds the [quadratic form](../../../../../../quadratic-form.md) by $C(m+\delta^{-1})\sum|b_r|^2$. The weights majorize half the desired interval, proving the dual inequality and hence the primal inequality. This supplies the sieve estimate with an absolute constant, including the technical interaction between close pairs and the kernel's decaying tail.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
