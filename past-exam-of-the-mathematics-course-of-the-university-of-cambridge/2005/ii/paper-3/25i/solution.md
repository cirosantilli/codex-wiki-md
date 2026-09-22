<h1 id="25i/solution">Solution</h1>

↑ **Parent:** [25I](../25i.md)

Let $m=\int t\,dF(t)$ be the finite mean service time. Poisson arrivals see the stationary occupancy distribution, so the accepted rate is $\lambda(1-\pi)$. An accepted arrival's independent service time still has mean $m$. [Little's law](../../../../../little-s-law.md) applied to occupied servers gives $\boxed{L=\lambda(1-\pi)m}$; it does not require exponential service times.

For the cafe, $\lambda=3/20$ and the mean table-occupation time is $(2/3)20+(1/3)30=70/3$. Thus $L=(7/2)(1-\pi)$ and the long-run revenue rate, at $2/5$ per occupied table per unit time, is

$$
\boxed{R=\frac75(1-\pi).}
$$

Couple the cafe to an infinite-table system using the same arrivals and assigned service durations. Each accepted finite-cafe party is also present in the infinite system for exactly the same interval, so finite occupancy never exceeds infinite occupancy. Singles and pairs form independent thinned Poisson arrival streams of rates $1/10$ and $1/20$. Their infinite-server occupancies are independent Poisson variables of means two and $3/2$, hence their total is $N\sim\operatorname{Poisson}(7/2)$. Consequently $\boxed{\pi\leq P(N\geq23)}$.

The exponential Markov bound $P(N\geq r)\leq\exp[\mu(e^t-1)-tr]$ is minimized at $t=\log(r/\mu)$. With $\mu=7/2,r=23$ it is $e^{-7/2}(7e/46)^{23}<5\times10^{-11}$. This is far below $10^{-3}$, so blocking and the associated revenue loss are negligible in the specified model.

## ↑ Ancestors (10)

1. [25I](../25i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
