<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use an ideal [carrier-sense multiple access](../../../../../carrier-sense-multiple-access.md) scheme on the [interference graph](../../../../../interference-graph.md). An active station finishes its transmission after an independent unit-rate [exponential distribution](../../../../../exponential-distribution.md) waiting time. An inactive station has an independent attempt clock with an [exponential distribution](../../../../../exponential-distribution.md) of rate $e^{\theta_r}$; an attempt succeeds only when all its neighbors are inactive. Attempts that are blocked do not change the state. Thus, on the [independent sets](../../../../../independent-set-graph-theory.md) represented by $S$, the [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) has [transition rates](../../../../../transition-intensity.md)

$$
q(n,n+e_r)=e^{\theta_r}\quad(n+e_r\in S),
\qquad q(n,n-e_r)=1\quad(n_r=1).
$$

The empty [independent set](../../../../../independent-set-graph-theory.md) can be reached by successive deactivations, and any other [independent set](../../../../../independent-set-graph-theory.md) can be reached from it by successive activations. Hence this finite chain is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md). The weight $a_\theta(n)=e^{\theta\cdot n}$ satisfies

$$
a_\theta(n)e^{\theta_r}=a_\theta(n+e_r).
$$

By [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md), its **unique stationary law** is

$$
\boxed{\pi_\theta(n)=\frac{e^{\theta\cdot n}}{Z(\theta)},\qquad
Z(\theta)=\sum_{m\in S}e^{\theta\cdot m}.}
$$

This is a finite [exponential family](../../../../../exponential-family-split.md). Its [natural parameter of an exponential family](../../../../../natural-parameter-of-an-exponential-family.md) is $\theta$ and its [mean parameter of an exponential family](../../../../../mean-parameter-of-an-exponential-family.md) is the vector of active fractions.

The [throughput region of an interference graph](../../../../../throughput-region-of-an-interference-graph.md) is exactly $\Lambda=\operatorname{conv}S$. To see the possibly less immediate inclusion, suppose a random feasible schedule has mean $v\geq\lambda$. Retain each of its active vertices $r$ independently with [probability](../../../../../probability.md) $\lambda_r/v_r$, interpreting zero coordinates as always deleted. A subset of an [independent set](../../../../../independent-set-graph-theory.md) remains an [independent set](../../../../../independent-set-graph-theory.md); the thinned schedule has mean exactly $\lambda$. Thus $\lambda$ lies in the [convex hull](../../../../../convex-hull.md) of $S$. The opposite inclusion follows from the definition using equality. Moreover $0,e_1,\ldots,e_R\in S$, so this [convex hull](../../../../../convex-hull.md) has full dimension.

Now choose $\varepsilon>0$ such that $\mu=\lambda+\varepsilon\mathbf1$ remains in the interior of $\operatorname{conv}S$. Use [interior moment matching in a finite exponential family](../../../../../interior-moment-matching-in-a-finite-exponential-family.md). Consider the [convex function](../../../../../convex-function.md)

$$
F(\theta)=\log Z(\theta)-\theta\cdot\mu.
$$

There is a ball of radius $\delta>0$ around $\mu$ contained in $\operatorname{conv}S$. Maximizing a linear functional over the [convex hull](../../../../../convex-hull.md) is the same as maximizing over its generating set, so, for every $\theta$,

$$
F(\theta)\geq\max_{n\in S}\theta\cdot(n-\mu)
\geq\delta\|\theta\|.
$$

The last inequality uses the point $\mu+\delta\theta/\|\theta\|$ when $\theta\ne0$. Hence $F$ is a [coercive function](../../../../../coercive-function.md) and has a finite minimizer $\theta^*$. Differentiating the finite normalizing sum gives

$$
\frac{\partial F}{\partial\theta_r}=\mathbb E_\theta[n_r]-\mu_r,
\qquad \nabla^2F=\operatorname{Cov}_\theta(n).
$$

This [covariance matrix](../../../../../covariance-matrix.md) is a [positive-definite matrix](../../../../../positive-definite-matrix.md): a linear functional constant on all states of positive weight must be constant on $0,e_1,\ldots,e_R$, so its coefficients vanish. Thus $F$ is a [strictly convex function](../../../../../strictly-convex-function.md); its minimizer is unique. At that minimizer the **desired strict service margins** are

$$
\boxed{\mathbb E_{\theta^*}[n_r]=\mu_r=\lambda_r+\varepsilon>\lambda_r
\quad\text{for all }r.}
$$

For a backlogged station that transmits at unit speed whenever active, the long-run [throughput](../../../../../throughput.md) is $\mathbb E_\theta[n_r]$, by the [ergodic theorem for a finite continuous-time Markov chain](../../../../../ergodic-theorem-for-a-finite-continuous-time-markov-chain.md). Therefore the ideal [carrier-sense multiple access](../../../../../carrier-sense-multiple-access.md) scheme can supply a strict service margin for every arrival vector in the interior of the [throughput region of an interference graph](../../../../../throughput-region-of-an-interference-graph.md). The local attempt rates can realize the whole interior capacity region in this sense. Boundary points may require parameters tending to infinity, and the argument gives no uniform delay or mixing-time bound near the boundary.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
