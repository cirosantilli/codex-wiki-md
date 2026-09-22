<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $B=\|f\|_\infty$, $v=\operatorname{Var}_\mu(f)$, and $N_n=n-m_n$. We first obtain a uniform-in-$f$ stationary bound, then compare the burned-in trajectory with a stationary one.

For a [reversible Markov chain](../../../../../../reversible-markov-chain.md), [geometric ergodicity](../../../../../../geometric-ergodicity.md) gives an [absolute L2 spectral gap of a reversible Markov chain](../../../../../../absolute-l2-spectral-gap-of-a-reversible-markov-chain.md). Thus, for some $r<1$, the [Markov kernel](../../../../../../markov-kernel.md) viewed as an operator satisfies

$$
\|Ph\|_{L^2(\mu)}\leq r\|h\|_{L^2(\mu)}\quad\text{if }\mu h=0.
$$

One can use the rate in the total-variation estimate. To see why, reversibility makes $P$ a [self-adjoint operator](../../../../../../self-adjoint-operator.md). For bounded mean-zero $h$ supported on a set where $M$ is bounded,

$$
0\leq\langle h,P^{2k}h\rangle
\leq2\|h\|_\infty\left(\int|h|M\,d\mu\right)r^{2k}.
$$

The [spectral theorem for normal operators](../../../../../../spectral-theorem-for-normal-operators.md) writes the left side as $\int t^{2k}\,d\nu_h(t)$. Any positive spectral mass where $|t|>r$ would contradict the inequality as $k\to\infty$. These test functions are dense in $L^2_0(\mu)$: truncate a function and restrict it to $\{M\leq j\}$, then correct its mean using a bounded function supported on a fixed positive-measure set where $M$ is bounded. Hence the spectral restriction extends to the entire mean-zero space.

Let $(W_i)$ be the stationary chain. For $h=f-\mu f$, the [stationary covariance bound for reversible Markov chains](../../../../../../stationary-covariance-bound-for-reversible-markov-chains.md) gives

$$
|\operatorname{Cov}(f(W_1),f(W_{1+k}))|
=|\langle h,P^kh\rangle|\leq r^k v.
$$

Consequently

$$
\operatorname{Var}\!\left(\sum_{i=1}^N f(W_i)\right)
\leq v\left[N+2\sum_{k=1}^{N-1}(N-k)r^k\right]
\leq N\gamma v,\qquad\gamma=\frac{1+r}{1-r}.
$$

The initial law of the burned-in trajectory is $P^{m_n}(x,\cdot)$. Its [total variation distance](../../../../../../total-variation-distance.md) from $\mu$ is at most $\varepsilon_n=M(x)r^{m_n}$. Attaching the same conditional future evolution cannot increase that distance, so the entire length-$N_n$ path laws differ by at most $\varepsilon_n$. For either path the sum $S$ has $|S|\leq BN_n$. The dual bound for [total variation distance](../../../../../../total-variation-distance.md) gives a difference of at most $2B^2N_n^2\varepsilon_n$ in the second moments, and at most $4B^2N_n^2\varepsilon_n$ in the squares of the means. This [burn-in total variation comparison](../../../../../../burn-in-total-variation-comparison.md) yields

$$
\operatorname{Var}\!\left(\sum_{i=m_n+1}^n f(X_i)\right)
\leq N_n\gamma v+6B^2N_n^2\varepsilon_n.
$$

Since $m_n=\lfloor n^{1/3}\rfloor$, $N_n r^{m_n}\to0$. Dividing by $N_n$ gives

$$
\boxed{\limsup_{n\to\infty}\frac1{n-m_n}\operatorname{Var}\!\left(\sum_{i=m_n+1}^n f(X_i)\right)\leq\frac{1+r}{1-r}\operatorname{Var}(f(Y)).}
$$

The constant depends on the chain, not on $f$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
