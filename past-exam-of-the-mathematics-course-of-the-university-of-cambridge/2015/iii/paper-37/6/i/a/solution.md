<h1 id="6/i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Bayes' theorem](../../../../../../../bayes-theorem.md) to multiply the [Ising model](../../../../../../../ising-model.md) prior by the conditionally independent normal likelihood factors. For fixed observed $x$, the [posterior distribution](../../../../../../../bayesian-posterior.md) is

$$
\boxed{\pi(s\mid x)\propto
\exp\!\left[-J\sum_{\{i,j\}\in\mathcal N}s_is_j
-\frac12\sum_{k\in D}\left\{x_k-\left(\sum_{j\in\mathcal N_k}s_j\right)^7\right\}^2\right],\qquad s\in\{-1,1\}^D.}
$$

There is no boundary wraparound: the neighbor sets use only actual horizontal and vertical edges inside the square. Each unordered edge is counted once. In particular, the prior retains the printed minus sign in front of $J$, and the likelihood retains the seventh power. The finite state space and finite observed values make every posterior weight positive and finite, with a finite positive normalizing sum.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [I](../../i.md)
3. [6](../../../6.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
