# Rearrangeable triangular loss network

↑ **Parent:** [Loss network](loss-network.md)

Three nodes have integer link capacities $C_{12},C_{13},C_{23}$. Calls between a node pair use either its direct link or the two-link alternative. With unrestricted instantaneous rearrangement of existing calls, counts $n_{12},n_{13},n_{23}$ are feasible exactly when $n_{12}+n_{13}\leq C_{12}+C_{13}$, $n_{12}+n_{23}\leq C_{12}+C_{23}$ and $n_{13}+n_{23}\leq C_{13}+C_{23}$. Necessity follows by counting calls crossing each node cut. For sufficiency, the inequalities allow at most one count to exceed its direct-link capacity. Divert precisely that excess to the other two links; the same inequalities ensure capacity there. The counts thus have the same feasible set as a [fixed routing](fixed-routing.md) [loss network](loss-network.md) with one virtual resource at each node, capacity equal to the sum of its two incident physical-link capacities, and each call using its two endpoint resources. With independent [Poisson processes](poisson-process.md) for arrivals and independent routing-independent [exponential distributions](exponential-distribution.md) for holding times, this gives the usual [product-form stationary distribution of a loss network](product-form-stationary-distribution-of-a-loss-network.md) and exact [Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md) blocking probabilities.

**Table of contents**

- [Cut feasibility for a rearrangeable triangle](cut-feasibility-for-a-rearrangeable-triangle.md)

## ↑ Ancestors (8)

1. [Loss network](loss-network.md)
2. [Stochastic network](stochastic-network.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30/2/solution.md)
