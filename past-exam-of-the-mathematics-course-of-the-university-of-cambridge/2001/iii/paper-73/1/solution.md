<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [closed migration process](../../../../../closed-migration-process.md) is a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) with state $n=(n_1,\ldots,n_m)\in\mathbb Z_+^m$, conserved population $\sum_i n_i=N$, and transition rates

$$
q(n,n-e_i+e_j)=\phi_i(n_i)p_{ij}\qquad(i\ne j).
$$

Here $\phi_i(0)=0$, $\phi_i(k)>0$ for $k>0$, and $P=(p_{ij})$ is a fixed stochastic routing [matrix](../../../../../matrix.md). Take $p_{ii}=0$ for convenience; self-routing can instead be omitted from the actual jumps. Assume irreducible routing. Let positive traffic weights satisfy $\theta_j=\sum_i\theta_i p_{ij}$. Define $d_i(0)=1$, $d_i(k)=\prod_{h=1}^k\phi_i(h)$. The [product-form stationary distribution of a closed migration process](../../../../../product-form-stationary-distribution-of-a-closed-migration-process.md) is

$$
\boxed{\pi(n)=\frac1{G_N}\prod_i\frac{\theta_i^{n_i}}{d_i(n_i)},\qquad G_N=\sum_{\sum_i n_i=N}\prod_i\frac{\theta_i^{n_i}}{d_i(n_i)}.}
$$

To prove it, an incoming transition $i\to j$ to $n$ comes from $m=n+e_i-e_j$, and is possible only if $n_j>0$. The weight ratio gives

$$
\pi(m)\phi_i(n_i+1)p_{ij}=\pi(n)\frac{\theta_i}{\theta_j}\phi_j(n_j)p_{ij}.
$$

Summing over $i$ and using the traffic equations gives $\pi(n)\phi_j(n_j)$. Summing then over $j$ equals $\pi(n)\sum_j\phi_j(n_j)$, the outgoing probability flux, proving [global balance for a continuous-time Markov chain](../../../../../global-balance-for-a-continuous-time-markov-chain.md). The state space is finite and irreducible, so this normalized [stationary distribution](../../../../../stationary-distribution.md) is unique. [Detailed balance](../../../../../detailed-balance.md) is not required; a directed routing cycle, for example, is not reversible.

For the switchboard, make each of the $N$ lines one circulating individual. Use colonies $F,O,C$ for free lines, calls waiting for or receiving the operator's connection service, and already connected calls. The transitions form the cycle $F\to O\to C\to F$, with departure rates

$$
\phi_F(f)=\nu\mathbf1_{\{f>0\}},\qquad\phi_O(k)=\lambda\mathbf1_{\{k>0\}},\qquad\phi_C(i)=\mu i.
$$

The first rate is $\nu$, not $f\nu$: incoming calls form one external [Poisson process](../../../../../poisson-process.md), not one per free line. An arrival when $f=0$ changes no state and is counted as lost. Exponential connection and conversation times make this the required [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md); only one call receives the operator's service at a time, whereas every connected call independently completes at rate $\mu$.

The cyclic traffic weights can all be chosen equal to one. Multiplying all unnormalized weights by the same $\nu^N$ gives, for $f+k+i=N$,

$$
\pi(f,k,i)\propto\left(\frac\nu\lambda\right)^k\frac{(\nu/\mu)^i}{i!}.
$$

If $n=k+i$ is the number of occupied lines, sum over the $n+1$ possibilities for the connected-call count:

$$
\sum_{i=0}^n\left(\frac\nu\lambda\right)^{n-i}\frac{(\nu/\mu)^i}{i!}=\left(\frac\nu\lambda\right)^n\sum_{i=0}^n\frac{(\lambda/\mu)^i}{i!}=H(n).
$$

Thus the normalizer is $\sum_{n=0}^NH(n)$ and the full-state probability is $H(N)/\sum_{n=0}^NH(n)$. By [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md), this is also the long-run fraction of attempted calls rejected:

$$
\boxed{P_{\rm loss}=\frac{H(N)}{\sum_{n=0}^NH(n)}.}
$$

One can also see the arrival-rate argument directly: the lost-call counting process has conditional intensity $\nu\mathbf1_{\{F=0\}}$, so its equilibrium rate is $\nu\pi(F=0)$; dividing by the total attempted-call rate $\nu$ gives the same fraction. As an independent check, [stationary flow conservation in a finite-line switchboard](../../../../../stationary-flow-conservation-in-a-finite-line-switchboard.md) gives $\nu(1-P_{\rm loss})=\lambda\Pr\{O>0\}=\mu\mathbb E[C]$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
