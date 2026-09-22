# Coordinate revealment

↑ **Parent:** [Decision-tree query cost](decision-tree-query-cost.md)

The [coordinate revealment](coordinate-revealment.md) of coordinate $i$ for a [decision tree](decision-tree.md) $T$ under [input](input-computer-science.md) [probability distribution](probability-distribution-split.md) $\mu$ is

$$
\delta_i(T,\mu)=\Pr_{X\sim\mu}(T\text{ queries coordinate }i).
$$

It depends on the chosen [decision tree](decision-tree.md) and the [probability distribution](probability-distribution-split.md), not just on the [Boolean function](boolean-function.md). Since no coordinate is queried twice on a [graph path](path-in-a-graph.md), [indicator functions](indicator-function.md) give

$$
q_T(X)=\sum_{i=1}^n\mathbf 1_{\{T\text{ queries }i\}},\qquad \mathbb E_\mu[q_T(X)]=\sum_{i=1}^n\delta_i(T,\mu).
$$

The second equality uses [linearity of expectation](linearity-of-expectation.md); it does not require [independence of random variables](independent-random-variables.md) or a [product measure](product-measure.md). The cited paper defines these inspection [probabilities](probability.md) and their sum for [product measures](product-measure.md); the displayed [indicator function](indicator-function.md) argument extends the identity to any [input](input-computer-science.md) [probability distribution](probability-distribution-split.md).[O'Donnell, Saks, Schramm and Servedio, Every decision tree has an influential variable, section 1.2, p. 2: δ\_i(T) and Δ(T); section 3.1, p. 6: distinct coordinates along each root–leaf path](every-decision-tree-has-an-influential-variable-by-ryan-o-donnell-and-others.md)

For the [three-bit majority decision tree](three-bit-majority-decision-tree.md) under the [discrete uniform distribution](discrete-uniform-distribution.md), $(\delta_1,\delta_2,\delta_3)=(1,1,1/2)$, whose sum is $2.5$. Reading coordinate 3 first, then coordinate 1, and stopping on agreement gives the same [majority function](majority-function.md), depth and [expected query cost](expected-query-cost.md), but [coordinate revealments](coordinate-revealment.md) $(1,1/2,1)$. The asymmetry belongs to the chosen query order. [Parity](parity.md) gives $(1,1,1)$ for every exact [decision tree](decision-tree.md) without repeated queries. If repeated queries were charged, inspection [probabilities](probability.md) would count distinct coordinates; total query count would instead require expected multiplicities.

## ↑ Ancestors (7)

1. [Decision-tree query cost](decision-tree-query-cost.md)
2. [Decision tree](decision-tree.md)
3. [Decision tree model](decision-tree-model.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Coordinate revealment](coordinate-revealment.md)
- [Decision-tree depth](decision-tree-depth.md)
- [Parity lower bound for Boolean queries](parity-lower-bound-for-boolean-queries.md)
