<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

For a dominated family of sample distributions, a statistic $T$ is a [sufficient statistic](../../../../../sufficient-statistic.md) precisely when the [probability mass function](../../../../../probability-mass-function.md) or [density](../../../../../density.md) factors as

$$
p_\theta(x)=g_\theta(T(x))h(x),
$$

where $h$ does not depend on the parameter. This is the [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md).

Here is the discrete proof in both directions. Suppose the factorization holds, and write $H(t)=\sum_{x:T(x)=t}h(x)$. Then $\mathbb P_\theta(T=t)=g_\theta(t)H(t)$. Whenever this probability is positive, $H(t)$ is finite and positive and

$$
\mathbb P_\theta(X=x\mid T=t)=\frac{h(x)}{H(t)},\qquad T(x)=t,
$$

is independent of $\theta$. Thus the [conditional distribution](../../../../../conditional-distribution.md) of the whole sample given $T$ is parameter-free, which is the definition of a [sufficient statistic](../../../../../sufficient-statistic.md).

Conversely, if $T$ is sufficient, let $q_t(x)$ denote this common conditional mass function on each possible fiber. Then

$$
p_\theta(x)=\mathbb P_\theta(T=T(x))q_{T(x)}(x).
$$

Take $g_\theta(t)=\mathbb P_\theta(T=t)$ and $h(x)=q_{T(x)}(x)$ to obtain the factorization. Fibers impossible for every parameter can be assigned $h=0$; conditional probabilities are required only for fibers with positive probability.

For the independent [Poisson](../../../../../poisson-distribution.md) sample the joint mass function is

$$
p_\theta(x_1,\ldots,x_n)=\frac{e^{-n\theta}\theta^{\sum_i x_i}}{\prod_i x_i!},\qquad x_i\in\{0,1,2,\ldots\}.
$$

All parameter dependence is through

$$
\boxed{T=\sum_{i=1}^nX_i},
$$

so this is a one-dimensional [sufficient statistic](../../../../../sufficient-statistic.md). The sample mean contains the same information, since $n$ is known.

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
