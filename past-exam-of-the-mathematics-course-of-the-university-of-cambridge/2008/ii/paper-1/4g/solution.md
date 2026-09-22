<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

If the possible values have [probabilities](../../../../../probability.md) $p_1,\ldots,p_N$, allowing zeros, the [Shannon entropy](../../../../../information-entropy.md) in bits is $H(X)=-\sum_i p_i\log_2p_i$, with $0\log_20=0$. Each term is nonnegative, so $H\geq0$, with equality precisely when one value has [probability](../../../../../probability.md) one.

For the upper bound, prove first that $\log t\leq t-1$ for $t>0$: the function $t-1-\log t$ has derivative $1-1/t$ and its unique minimum, zero, at $t=1$. Let $m$ be the number of positive [probabilities](../../../../../probability.md). Applying this inequality to $t=(Np_i)^{-1}$ gives

$$
\sum_{p_i>0}p_i\log\frac1{Np_i}\leq\sum_{p_i>0}\left(\frac1N-p_i\right)=\frac mN-1\leq0.
$$

The left side is $H(X)\log2-\log N$, proving

$$
\boxed{0\leq H(X)\leq\log_2N.}
$$

Equality at the maximum requires $m=N$ and equality in every logarithmic inequality, so every $p_i=1/N$. Conversely the [uniform distribution](../../../../../continuous-uniform-distribution.md) attains it. For $N=1$ the maximum and minimum coincide at zero.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
