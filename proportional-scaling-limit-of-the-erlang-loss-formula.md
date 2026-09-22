# Proportional scaling limit of the Erlang loss formula

↑ **Parent:** [Erlang loss formula](erlang-loss-formula.md)

Scale the offered load and capacity together. Reversing the denominator of the [Erlang loss formula](erlang-loss-formula.md) gives

$$
E(N\nu,NC)^{-1}=\sum_{j=0}^{NC}\prod_{\ell=0}^{j-1}\frac{NC-\ell}{N\nu}.
$$

For each fixed $j$, the summand tends to $(C/\nu)^j$. If $\nu>C$, the [dominated convergence theorem](dominated-convergence-theorem.md) applies with the summable [geometric series](geometric-series.md) bound $(C/\nu)^j$. Otherwise each fixed finite partial sum has limiting value at least its number of terms, so the reciprocal diverges. Taking reciprocals proves the formula, including the critical case $\nu=C$.

## ↑ Ancestors (9)

1. [Erlang loss formula](erlang-loss-formula.md)
2. [Loss network](loss-network.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fluid scaling proof of multiple Erlang fixed points](fluid-scaling-proof-of-multiple-erlang-fixed-points.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/3/c/solution.md)
