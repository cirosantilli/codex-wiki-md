<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $p<1/2$, and put $a=\theta/p$ and $r=p/q\in(0,1)$. The [detailed balance equations](../../../../../detailed-balance.md) give

$$
\frac{\pi_{k+1}}{\pi_k}=\frac{p}{q}\frac{k+a}{k+1}\frac{k+1+\theta}{k+\theta}.
$$

Multiplying from $0$ to $k-1$, the last factor telescopes, while the product involving $a$ is evaluated by the [Gamma function](../../../../../gamma-function.md):

$$
\pi_k=\pi_0\frac{k+\theta}{\theta}\frac{\Gamma(k+a)}{\Gamma(a)k!}r^k\quad(k\geq0).
$$

Consequently the requested [invariant distribution](../../../../../stationary-distribution.md) can be expressed using the paper's power series as

$$
\boxed{\pi_k=\frac{(k+\theta)\Gamma(k+\theta/p)}{k!\,g_{p,\theta}(p/q)}\left(\frac pq\right)^k,\quad k\geq0.}
$$

The assumed convergence of $g_{p,\theta}(r)$ ensures that this normalization is finite and positive.

For an explicit normalizing constant, the [binomial series](../../../../../binomial-series.md) gives

$$
H(r)=\sum_{k=0}^\infty\frac{\Gamma(k+a)}{k!}r^k=\Gamma(a)(1-r)^{-a}.
$$

The [termwise differentiation of a power series](../../../../../termwise-differentiation-of-a-power-series.md) is valid for $|r|<1$, so

$$
\begin{aligned}
g_{p,\theta}(r)&=rH'(r)+\theta H(r)\\
&=\Gamma(a)(1-r)^{-a-1}\bigl[ar+\theta(1-r)\bigr]\\
&=2\theta\Gamma(a)(1-r)^{-a-1}.
\end{aligned}
$$

The last equality uses $r=p/q$ and $a=\theta/p$: $ar+\theta(1-r)=\theta/q+\theta(q-p)/q=2\theta$. Therefore

$$
\boxed{\pi_k=\frac{(1-r)^{a+1}}{2\theta\Gamma(a)}\frac{(k+\theta)\Gamma(k+a)}{k!}r^k,\qquad \pi_0=\frac12(1-r)^{a+1}.}
$$

These positive terms sum to one and satisfy the [detailed balance equations](../../../../../detailed-balance.md), so part (a)(ii) verifies stationarity. Irreducibility makes the [invariant distribution](../../../../../stationary-distribution.md) unique.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
