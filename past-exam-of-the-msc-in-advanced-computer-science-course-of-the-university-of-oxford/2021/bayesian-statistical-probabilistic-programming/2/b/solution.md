<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $0<p(x)<\infty$, take $q_\lambda$ supported where $p(z,x)>0$, and assume the following [expectations](../../../../../expected-value-split.md) exist. By the definition of [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) and [Bayes' theorem](../../../../../bayes-theorem.md),

$$
\begin{aligned}
D_{\rm KL}(q_\lambda\Vert p(\cdot\mid x))
&=\mathbb E_{q_\lambda}\left[\log q_\lambda(z)-\log\frac{p(z,x)}{p(x)}\right]\\
&=\log p(x)-\mathbb E_{q_\lambda}[\log p(z,x)-\log q_\lambda(z)].
\end{aligned}
$$

Therefore the [evidence lower bound](../../../../../evidence-lower-bound.md) is

$$
\boxed{\mathcal L(\lambda)=\mathbb E_{q_\lambda}[\log p(z,x)-\log q_\lambda(z)]=\log p(x)-D_{\rm KL}(q_\lambda\Vert p(\cdot\mid x)).}
$$

Nonnegativity of [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) proves $\mathcal L(\lambda)\leq\log p(x)$. The [marginal likelihood](../../../../../bayesian-model-evidence.md) $p(x)$ is constant with respect to the variational parameter $\lambda$, so maximizing $\mathcal L$ minimizes the stated [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md).

The practical advantage is that evaluating [logarithms](../../../../../logarithm.md) of joint [probabilities](../../../../../probability.md) and $\log q_\lambda$ requires no evaluation of the usually intractable [marginal likelihood](../../../../../bayesian-model-evidence.md). One can estimate $\mathcal L$ and its [gradient](../../../../../gradient.md) with [Monte Carlo method](../../../../../monte-carlo-method-split.md). Equality with the log [marginal likelihood](../../../../../bayesian-model-evidence.md) occurs only when $q_\lambda=p(\cdot\mid x)$ almost everywhere. Merely maximizing the [evidence lower bound](../../../../../evidence-lower-bound.md) over a restricted family neither computes the exact [posterior distribution](../../../../../bayesian-posterior.md) nor proves that the maximum attains this equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
