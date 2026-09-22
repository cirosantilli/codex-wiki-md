<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take observation periods to have positive lengths $t_i>0$, and let $P$ be the [Markov kernel](../../../../../../markov-kernel.md) of a sweep which first draws $b$ given the current $\theta$ and then draws the new vector $\Theta'$. Write $A_i=a+y_i$. Conditional on $b$, [independence](../../../../../../independent-random-variables.md) and the [gamma distribution](../../../../../../gamma-distribution.md) mean and [variance](../../../../../../variance-split.md) give

$$
\mathbb E\!\left[\left(\sum_i\Theta_i'\right)^2\Bigm|b\right]
=\left(\sum_i\frac{A_i}{b+t_i}\right)^2+
\sum_i\frac{A_i}{(b+t_i)^2}
\leq\left(\sum_i\frac{A_i}{t_i}\right)^2+\sum_i\frac{A_i}{t_i^2}=:D.
$$

Averaging over the [full conditional distribution](../../../../../../full-conditional-distribution.md) of $b$ preserves this bound, uniformly in the current state. Therefore $PV(\theta)\leq M:=1+D<\infty$. This is the mechanism in [bounded conditional moments imply a geometric drift](../../../../../../bounded-conditional-moments-imply-a-geometric-drift.md).

Choose $0<\rho<1$, $R>M/\rho$, and $C=\{\theta:V(\theta)\leq R\}$. Outside $C$, $PV\leq M<\rho V$; inside $C$, $PV\leq M\leq\rho V+M$. Hence

$$
\boxed{PV(\theta)\leq\rho V(\theta)+M\mathbf1_C(\theta),\qquad 0<\rho<1.}
$$

For completeness, $C$ is a [small set](../../../../../../small-set.md), even though it approaches the boundary of the positive orthant. Choose $\delta>0$ small enough that $B=[\delta,2\delta]^n\subset C$. On $C$, $s=\sum_i\theta_i\leq\sqrt{R-1}$. The conditional [gamma distribution](../../../../../../gamma-distribution.md) of $b$ has fixed shape $na+c$ and rate $1+s$ in a compact positive interval. Its [probability density function](../../../../../../probability-density-function.md) therefore has a positive common lower bound on $b\in[1,2]$. For those $b$, the product [probability density function](../../../../../../probability-density-function.md) of $\Theta'$ similarly has a positive common lower bound on $B$, since every shape is positive and every rate $b+t_i$ lies in a compact positive interval. Integrating over $b\in[1,2]$ gives $P(\theta,\cdot)\geq\varepsilon\eta(\cdot)$ on $C$, where $\eta$ is the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $B$ and $\varepsilon>0$.

The transition [probability density function](../../../../../../probability-density-function.md) is positive throughout the positive orthant, giving an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md). Since $B\subset C$, the box minorization includes starts in the same box, which gives an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md). The proper [prior distributions](../../../../../../prior-probability.md) and bounded [Poisson distribution](../../../../../../poisson-distribution.md) likelihood have positive finite evidence, so the invariant [posterior distribution](../../../../../../bayesian-posterior.md) is proper. Together with the [geometric drift condition](../../../../../../geometric-drift-condition.md), these hypotheses imply [geometric ergodicity](../../../../../../geometric-ergodicity.md). In particular, the argument proves the required drift rather than assuming that every [Gibbs sampler](../../../../../../gibbs-sampler.md) is geometrically ergodic.

The positive-period convention matters. If zero lengths are allowed, the printed assertion can fail: take $n=1$, $a=c=1$, $t_1=y_1=0$. Then $b\mid\theta\sim\operatorname{Gamma}(2,1+\theta)$ and $\Theta'\mid b\sim\operatorname{Gamma}(1,b)$, so

$$
\mathbb E[(\Theta')^2\mid\theta]=2\mathbb E[b^{-2}\mid\theta]=\infty.
$$

This example has a proper [posterior distribution](../../../../../../bayesian-posterior.md) but cannot satisfy a finite quadratic [geometric drift condition](../../../../../../geometric-drift-condition.md). Thus the proof establishes the intended claim for positive observation periods, not an unrestricted extension to zero exposure.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
