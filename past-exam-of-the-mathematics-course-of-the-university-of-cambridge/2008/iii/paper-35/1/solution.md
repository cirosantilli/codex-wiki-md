<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume $\nu,\lambda,\mu>0$ and regard each line as an individual circulating through three colonies. Then $n$ is a [closed migration process](../../../../../closed-migration-process.md) on $\{n\in\mathbb Z_{\ge0}^3:n_1+n_2+n_3=N\}$. With $e_j$ the coordinate vectors, its nonzero transition intensities are

$$
\boxed{\begin{aligned}
q(n,n-e_1+e_2)&=\nu\mathbf1_{\{n_1>0\}},\\
q(n,n-e_2+e_3)&=\lambda\mathbf1_{\{n_2>0\}},\\
q(n,n-e_3+e_1)&=\mu n_3.
\end{aligned}}
$$

The [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) of the [exponential distributions](../../../../../exponential-distribution.md) and the independent [Poisson process](../../../../../poisson-process.md) make these counts a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md). In particular, the accepted-arrival rate is $\nu$, not $\nu n_1$: free lines are availability tokens, not independent callers. An attempted arrival when $n_1=0$ is lost and causes no state change, so it does not enter the off-diagonal generator.

For the cyclic routing $1\to2\to3\to1$, take equal traffic weights at all colonies. The [product-form stationary distribution of a closed migration process](../../../../../product-form-stationary-distribution-of-a-closed-migration-process.md) gives weights

$$
w(n)=\frac{(\nu/\lambda)^{n_2}(\nu/\mu)^{n_3}}{n_3!}.
$$

Here is a direct [global balance for a continuous-time Markov chain](../../../../../global-balance-for-a-continuous-time-markov-chain.md) verification. Set $\phi_1(k)=\nu\mathbf1_{\{k>0\}}$, $\phi_2(k)=\lambda\mathbf1_{\{k>0\}}$, $\phi_3(k)=\mu k$, with cyclic subscripts. The predecessor for a $j\to j+1$ transition is $m=n+e_j-e_{j+1}$, allowed when $n_{j+1}>0$. The product weights obey

$$
w(m)\phi_j(n_j+1)=w(n)\phi_{j+1}(n_{j+1}).
$$

Summing these incoming weights over the three edges gives $w(n)\sum_j\phi_j(n_j)$, precisely the outgoing weight. Thus $\pi(n)=w(n)/G_N$ is stationary. The finite state space is irreducible, so this [stationary distribution](../../../../../stationary-distribution.md) is unique.

Let $k=n_2+n_3$ be the occupied-line count. Summing over its automated-service count $i=n_3$ gives

$$
\sum_{n_2+n_3=k}w(n)=\sum_{i=0}^k(\nu/\lambda)^{k-i}\frac{(\nu/\mu)^i}{i!}=(\nu/\lambda)^k\sum_{i=0}^k\frac{(\lambda/\mu)^i}{i!}=H(k),
$$

so $G_N=\sum_{k=0}^NH(k)$. The external [Poisson process](../../../../../poisson-process.md) sees the stationary state probabilities by [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md). A call is lost exactly when $n_1=0$, equivalently $k=N$. Therefore

$$
\boxed{P_{\mathrm{loss}}=\frac{H(N)}{\sum_{k=0}^NH(k)}.}
$$

For two independent identical operators, the middle transition rate becomes $\lambda\min(n_2,2)$: one call receives one operator's service, while two or more calls keep both operators busy. Define $D_2(0)=1$ and $D_2(m)=\prod_{h=1}^m\min(h,2)=2^{m-1}$ for $m\ge1$. The same [global balance for a continuous-time Markov chain](../../../../../global-balance-for-a-continuous-time-markov-chain.md) calculation applies to

$$
w_2(n)=\frac{(\nu/\lambda)^{n_2}(\nu/\mu)^{n_3}}{D_2(n_2)n_3!},\qquad H_2(k)=\sum_{i=0}^k\frac{(\nu/\lambda)^{k-i}(\nu/\mu)^i}{D_2(k-i)i!}.
$$

Consequently the [blocking probability in a finite-line sequential-service network](../../../../../blocking-probability-in-a-finite-line-sequential-service-network.md) is

$$
\boxed{P_{\mathrm{loss}}^{(2)}=\frac{H_2(N)}{\sum_{k=0}^NH_2(k)},\qquad H_2(k)=2\left(\frac{\nu}{2\lambda}\right)^k\sum_{i=0}^k\frac{(2\lambda/\mu)^i}{i!}-\frac{(\nu/\mu)^k}{k!}.}
$$

The subtraction corrects the $n_2=0$ term, for which $D_2(0)=1$ rather than $2^{-1}$. In particular $H_2(0)=1$, and when $N\le1$ replacing one operator by two does not change blocking.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
