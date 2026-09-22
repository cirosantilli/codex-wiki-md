<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $p_i=\mathbb P(X_i=1)$ and $\lambda=\sum_i p_i$. A relative-entropy form of the [Poisson approximation bound for dependent Bernoulli variables](../../../../../../poisson-approximation-bound-for-dependent-bernoulli-variables.md) is

$$
D_e(P_{S_n}\Vert\operatorname{Poisson}(\lambda))
\leq\sum_{i=1}^np_i^2
+\sum_{i=1}^nH_e(X_i)-H_e(X_1,\ldots,X_n).
$$

The last two terms form the [total correlation](../../../../../../total-correlation.md); they vanish when the Bernoulli variables are independent.

Here $D_e$ and $H_e$ use [natural logarithms](../../../../../../natural-logarithm.md).

To prove the bound, let $Q_i$ be the [Poisson distribution](../../../../../../poisson-distribution.md) with mean $p_i$ and let $Q=\bigotimes_iQ_i$. Expanding the [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) against this product law gives

$$
D_e(P_{X_1^n}\Vert Q)
=\sum_iD_e(\operatorname{Bernoulli}(p_i)\Vert\operatorname{Poisson}(p_i))
+\sum_iH_e(X_i)-H_e(X_1^n).
$$

The supplied one-dimensional estimate bounds the first sum by $\sum_i p_i^2$. Under the addition map, $P_{X_1^n}$ becomes $P_{S_n}$, while the [Sum of independent Poisson random variables](../../../../../../addition-of-independent-poisson-random-variables.md) under $Q$ has the Poisson distribution with mean $\lambda$. The [data processing inequality for relative entropy](../../../../../../data-processing-inequality-for-relative-entropy.md) proves the displayed result.

If a bound directly in the paper's unhalved total-variation norm is desired, [Pinsker's inequality](../../../../../../pinsker-s-inequality.md) also gives

$$
\boxed{\lVert P_{S_n}-\operatorname{Poisson}(\lambda)\rVert_1
\leq\sqrt{2\left\{\sum_i p_i^2+\sum_iH_e(X_i)-H_e(X_1^n)\right\}}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
