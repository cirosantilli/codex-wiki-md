<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $X_s$ count the copies of the [complete graph](../../../../../complete-graph.md) $K_s$ in the [binomial random graph](../../../../../binomial-random-graph.md) $G_{n,p}$. By linearity of the [expected value](../../../../../expected-value.md) and independence of distinct edges,

$$
\mathbb EX_s=\binom ns p^{\binom s2}.
$$

Throughout, $n$ is sufficiently large that $k=\lfloor\log\log n\rfloor\geq2$. We have $k\to\infty$, $k=O(\log\log n)$ and $k\log k=o(\log n)$.

First, since $p=n^{-2/k}$,

$$
\mathbb EX_{k+1}=\binom n{k+1}n^{-(k+1)}\leq\frac1{(k+1)!}\longrightarrow0.
$$

The [first moment method](../../../../../first-moment-method.md) proves $\mathbb P(X_{k+1}>0)=o(1)$.

For the existence of a $k$-[clique](../../../../../clique-graph-theory.md), put $X=X_k$ and $\mu=\mathbb EX$. Since $p^{\binom k2}=n^{-(k-1)}$,

$$
\mu=\frac n{k!}\prod_{i=0}^{k-1}\left(1-\frac in\right)=\frac n{k!}(1+o(1))\longrightarrow\infty.
$$

This alone is insufficient: we must control the [variance](../../../../../variance-split.md) via the [overlap formula for the variance of a clique count](../../../../../overlap-formula-for-the-variance-of-a-clique-count.md). Let $I_S$ indicate that a given $k$-set $S$ spans a [clique](../../../../../clique-graph-theory.md). If $|S\cap T|=j$, the two copies share $\binom j2$ edges, so

$$
\mathbb E(I_SI_T)=p^{2\binom k2-\binom j2}.
$$

For $j=0,1$ their edge sets are disjoint and the [covariance](../../../../../covariance.md) vanishes, even when they share one vertex. Counting ordered pairs of $k$-sets gives the exact formula

$$
\frac{\operatorname{Var}X}{\mu^2}=\sum_{j=2}^k\frac{\binom kj\binom{n-k}{k-j}}{\binom nk}\left(p^{-\binom j2}-1\right).
$$

This includes the diagonal case $j=k$.

To bound the overlap factor, regard it as the probability that a uniformly chosen $k$-set $T$ intersects a fixed $S$ in exactly $j$ vertices. A [union bound](../../../../../boole-s-inequality.md) over the possible specified $j$-subsets of $S$ yields

$$
\frac{\binom kj\binom{n-k}{k-j}}{\binom nk}\leq\binom kj\frac{(k)_j}{(n)_j}\leq\left(\frac{k^2}{n-k}\right)^j\leq\left(\frac{2k^2}{n}\right)^j.
$$

Here $(a)_j=a(a-1)\cdots(a-j+1)$ is a [falling factorial](../../../../../falling-factorial.md), and the last bound holds for $n\geq2k$. Therefore

$$
\frac{\operatorname{Var}X}{\mu^2}\leq\sum_{j=2}^k(2k^2)^j n^{-j+j(j-1)/k}=\sum_{j=2}^k(2k^2)^j n^{-j(k-j+1)/k}.
$$

For $2\leq j\leq k$, the concave quadratic $j(k-j+1)$ is minimized at an endpoint. Its endpoint values are $2(k-1)$ and $k$, both at least $k$. Thus every power of $n$ in the last sum is at most $n^{-1}$, and

$$
\frac{\operatorname{Var}X}{\mu^2}\leq\frac{k(2k^2)^k}{n}=o(1),
$$

because the [logarithm](../../../../../logarithm.md) of its numerator is $O(k\log k)=o(\log n)$. The [second moment method](../../../../../second-moment-method.md), or [Chebyshev's inequality](../../../../../chebyshev-inequality.md) directly, gives $\mathbb P(X=0)=o(1)$. Finally, every larger [clique](../../../../../clique-graph-theory.md) contains a $(k+1)$-[clique](../../../../../clique-graph-theory.md), so the absence of $K_{k+1}$ excludes all larger sizes. **The [clique number](../../../../../clique-number.md) is exactly $k$ [with high probability](../../../../../with-high-probability.md):**

$$
\boxed{\mathbb P(\omega(G_{n,p})=k)=1-o(1).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 112](../../paper-112-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
