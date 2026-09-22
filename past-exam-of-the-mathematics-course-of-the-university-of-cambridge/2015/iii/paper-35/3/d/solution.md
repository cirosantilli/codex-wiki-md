<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume individual incubation delays are [independent](../../../../../../independent-random-variables.md) of the [Inhomogeneous Poisson process](../../../../../../inhomogeneous-poisson-process.md) of infections and of one another. This marking assumption is needed in addition to specifying a marginal incubation density.

In the discrete cohort model let $N_i\sim\operatorname{Poisson}(h_i)$ be the [independent](../../../../../../independent-random-variables.md) infection counts. Mark each infection by its eventual onset interval. For cohort $i$, the categories have probabilities $q_{ik}$ for observed intervals, with the remaining probability assigned to onsets outside the window. [Poisson thinning](../../../../../../poisson-thinning.md) makes the counts $N_{ik}$ in these categories mutually [independent](../../../../../../independent-random-variables.md) [Poisson random variables](../../../../../../poisson-distribution.md) with means $h_iq_{ik}$. One direct proof is their [probability generating function](../../../../../../probability-generating-function.md):

$$
\mathbb E\!\left[\prod_k z_k^{N_{ik}}\right]
=\exp\!\left[h_i\sum_kq_{ik}(z_k-1)\right]
=\prod_k\exp[h_iq_{ik}(z_k-1)].
$$

Different cohorts are [independent](../../../../../../independent-random-variables.md). Summing their counts therefore gives **independent Poisson onset counts in disjoint intervals**:

$$
\boxed{Y_k=\sum_iN_{ik}\sim\operatorname{Poisson}(\mu_k),\qquad
\mu_k=\sum_i h_iq_{ik},\qquad Y_j\perp Y_k\ (j\ne k).}
$$

The same argument applies exactly in continuous time by the [Independent marking theorem for Poisson point processes](../../../../../../independent-marking-theorem-for-poisson-point-processes.md) and mapping each marked infection to its onset time. The endpoint model approximates its means; its independent-Poisson conclusion is exact within that discrete model. A fixed cohort size would instead induce negatively correlated onset-bin counts, so the [Poisson process](../../../../../../poisson-process.md) infection assumption matters.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
