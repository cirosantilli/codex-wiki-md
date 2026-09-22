<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [additive arithmetic function](../../../../../../additive-function-number-theory.md) $f$, one standard form of the [Turán-Kubilius inequality](../../../../../../turan-kubilius-inequality.md) uses

$$
A_f(N)=\sum_{p^k\le N}\frac{f(p^k)}{p^k}\left(1-\frac1p\right),\qquad B_f(N)^2=\sum_{p^k\le N}\frac{|f(p^k)|^2}{p^k}.
$$

It states, with an absolute constant,

$$
\frac1N\sum_{n\le N}|f(n)-A_f(N)|^2\ll B_f(N)^2.
$$

For real $f$, this also bounds the [variance](../../../../../../variance-split.md) under the [discrete uniform distribution](../../../../../../discrete-uniform-distribution.md), because centering at the actual [expectation](../../../../../../expected-value.md) minimizes the mean square.

For the [prime omega function](../../../../../../prime-omega-function.md), $f(p^k)=1$. The [Mertens theorem for reciprocal primes](../../../../../../mertens-second-theorem.md) states $\sum_{p\le N}1/p=\log\log N+O(1)$. The contribution of higher [prime powers](../../../../../../prime-power.md) is bounded by $\sum_p1/(p(p-1))\le1$, as proved in 1(a). It follows that $A_\omega(N)=\log\log N+O(1)$ and $B_\omega(N)^2\ll\log\log N$. Writing $L=\log\log N$, the [Turán-Kubilius inequality](../../../../../../turan-kubilius-inequality.md) and [Chebyshev inequality](../../../../../../chebyshev-inequality.md) therefore yield

$$
\boxed{\mathbb P_N(|\omega-L|\ge0.01L)\ll L^{-1}.}
$$

The bounded error in $A_\omega-L$ is absorbed by, for example, using the threshold $0.005L$ around $A_\omega$ for sufficiently large $N$.

For the [multiplication table problem](../../../../../../multiplication-table-problem.md), call a pair $(a,b)\in[N]^2$ good when $\omega(a),\omega(b)\ge0.99L$ and $\omega(\gcd(a,b))\le0.1L$. The preceding [Chebyshev inequality](../../../../../../chebyshev-inequality.md) excludes only $O(N^2/L)$ pairs by either of the first two conditions. For the [greatest common divisor](../../../../../../greatest-common-divisor.md) condition, [linearity of expectation](../../../../../../linearity-of-expectation.md) under uniform sampling of the two coordinates gives

$$
\frac1{N^2}\sum_{a,b\le N}\omega(\gcd(a,b))=\sum_{p\le N}\left(\frac{\lfloor N/p\rfloor}{N}\right)^2\le\sum_{m=2}^\infty\frac1{m^2}<\infty.
$$

[Markov inequality](../../../../../../markov-inequality.md) therefore excludes only another $O(N^2/L)$ pairs.

The [prime factors](../../../../../../prime-factor.md) of a product form the union of those of its factors. Consequently, for every good pair,

$$
\omega(ab)=\omega(a)+\omega(b)-\omega(\gcd(a,b))\ge1.88L.
$$

On the other hand, apply the proved concentration estimate at $N^2$. Since $\log\log(N^2)=L+\log2$, for large $N$ every integer $m\le N^2$ with $\omega(m)\ge1.88L$ is exceptional there. There are only $O(N^2/L)$ such integers. Products of good pairs lie in this exceptional set; products having only bad representations are at most as numerous as the bad pairs. This proves **the multiplication-table upper bound, using distinct prime factors alone**:

$$
\boxed{\#\{ab:1\le a,b\le N\}\ll\frac{N^2}{\log\log N}=o(N^2).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
