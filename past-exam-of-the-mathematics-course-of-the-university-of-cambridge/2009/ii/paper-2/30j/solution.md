<h1 id="30j/solution">Solution</h1>

↑ **Parent:** [30J](../30j.md)

A [martingale](../../../../../martingale-split.md) is an adapted integrable process $M_n$ with $\mathbb E(M_{n+1}\mid\mathcal F_n)=M_n$. A [stopping time](../../../../../stopping-time.md) $T$ satisfies $\{T\leq n\}\in\mathcal F_n$. The bounded [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) states that for bounded [stopping times](../../../../../stopping-time.md) $S\leq T$, $\mathbb E(M_T\mid\mathcal F_S)=M_S$.

To prove it, let $A\in\mathcal F_S$ and take a common deterministic bound $N$. Then

$$
\mathbb E[\mathbf1_A(M_T-M_S)]=\sum_{j=0}^{N-1}\mathbb E[\mathbf1_{A\cap\{S\leq j<T\}}(M_{j+1}-M_j)]=0,
$$

since each indicator is $\mathcal F_j$-measurable. This proves the conditional identity. The theorem extends to almost surely finite [stopping times](../../../../../stopping-time.md) for a uniformly integrable [martingale](../../../../../martingale-split.md) by truncating the times and passing in $L^1$; without such a hypothesis unrestricted optional sampling is false.

For the proposed exponential process, conditioning on one increment gives the [martingale](../../../../../martingale-split.md) condition $z(pe^\theta+qe^{-\theta})=1$. Thus, when $q>0$, the complete set is

$$
\boxed{\theta_\pm=\log\left(\frac{1\pm\sqrt{1-4pqz^2}}{2pz}\right).}
$$

These are the two real logarithms: $\theta_-<0<\theta_+$. If $q=0$, the sole finite value is $\theta=-\log z$. Stop the $\theta_+$ [martingale](../../../../../martingale-split.md) at $n\wedge\tau_k$. Before the first hit, $S_n<k$, so the stopped process is bounded above by $e^{k\theta_+}$. On failure to hit, its value tends to zero because of $z^n$. Bounded convergence after bounded optional sampling gives $1=e^{k\theta_+}\mathbb E[z^{\tau_k};\tau_k<\infty]$, hence

$$
\boxed{G_k(z)=\left(\frac{2pz}{1+\sqrt{1-4pqz^2}}\right)^k.}
$$

Its limit at $z=1$ is one, proving almost-sure hitting as well. Differentiating at one gives

$$
\boxed{\mathbb E\tau_k=\frac{k}{p-q}.}
$$

For instance implicit differentiation of the [martingale](../../../../../martingale-split.md) equation gives $\theta_+'(1)=-1/(p-q)$.

For the first subsequent return $\tau'_k$, the walk may first rise above $k$, so the uniform bound used in the stopping-limit argument fails. In fact after reaching $k$ it returns with probability $q+p(q/p)=2q<1$: a downward first step is followed by an almost-sure upward hit, while an upward first step hits the level below only with probability $q/p$. Thus $\tau'_k=\infty$ with positive probability and its unconditional mean is infinite. This pinpoints why repeating the earlier differentiation argument is invalid; bounded-time optional sampling itself remains valid.

## ↑ Ancestors (10)

1. [30J](../30j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
