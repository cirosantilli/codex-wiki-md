<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditional on $Y_m=i$, the [holding time](../../../../../../holding-time.md) $V_m=U_m/g(i)$ has an [exponential distribution](../../../../../../exponential-distribution.md) of rate $g(i)$, and after that holding time the next state is $j$ with [transition probability](../../../../../../transition-probability.md) $p_{ij}$. The [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md) of exponential random variables and the [Markov property](../../../../../../markov-property.md) of $(Y_m)$ therefore make $(X_t)$ a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md).

Moreover $g(i)<1/\varepsilon$, so $V_m\geq\varepsilon U_m$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $\sum_mU_m=\infty$ almost surely, hence $J_m\to\infty$ and the process is [nonexplosive](../../../../../../nonexplosion-under-uniformly-bounded-jump-rates.md). Its [Q-matrix](../../../../../../transition-rate-matrix.md) is

$$
\boxed{q_{ij}=g(i)p_{ij}\quad(i\ne j),\qquad q_{ii}=-g(i).}
$$

Equivalently, if $D_g$ is the [diagonal matrix](../../../../../../diagonal-matrix.md) with entries $g(i)$, then

$$
\boxed{Q=D_g(P-I).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
