# Boltzmann machine

↑ **Parent:** [Neural network](neural-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boltzmann_machine)

A [Boltzmann machine](boltzmann-machine.md) is a stochastic [neural network](neural-network.md) that learns a [probability distribution](probability-distribution-split.md) specified by pairwise [energies](energy-split.md). To compare it directly with a [Hopfield network](hopfield-network.md), use the bipolar [energy](energy-split.md) $E(x)=-\sum_{i<j}w_{ij}x_ix_j+\sum_i\theta_ix_i$. Here $\beta>0$ controls the preference for low [energy](energy-split.md), and the [partition function](canonical-partition-function.md) $Z=\sum_xe^{-\beta E(x)}$ normalizes all states. In a computational model, $\beta$ is an algorithmic inverse [temperature](temperature-split.md); interpreting it as $1/(k_BT)$ additionally requires physical [energy](energy-split.md) units.

A random single-unit [Gibbs sampling](gibbs-sampler.md) update has [conditional probability](conditional-probability.md)

$$
p_\beta(x_k=1\mid x_{-k})=\frac1{1+e^{-2\beta h_k}},\qquad h_k=\sum_{j\ne k}w_{kj}x_j-\theta_k.
$$

Indeed, the two possible [energies](energy-split.md) differ by $-2h_k$; their normalized [Boltzmann weights](boltzmann-factor.md) give this [logistic function](logistic-function.md). Random selection of one unit at a time satisfies [detailed balance](detailed-balance.md). For finite weights and finite positive $\beta$, all conditional probabilities lie strictly between zero and one, so the finite [Markov chain](markov-chain-split.md) can reach every state and can remain in place. Its unique [stationary distribution](stationary-distribution.md) is $p_\beta$. A short run need not yet sample that distribution accurately.

As $\beta\to\infty$, a nonzero field selects its sign, approaching [asynchronous Hopfield energy descent](asynchronous-hopfield-energy-descent.md). At zero field the stochastic rule remains a fair coin, whereas the deterministic convention above retains the old value. At finite inverse [temperature](temperature-split.md), uphill moves permit exploration beyond one [local minimum](local-minimum.md). Recall and learning are different operations: sampling changes the units at fixed weights; learning changes the weights to fit the [training data](training-data.md).

**Table of contents**

- [Positive and negative phases of Boltzmann learning](positive-and-negative-phases-of-boltzmann-learning.md)
  - [Visible unit](visible-unit.md)
- [Two-spin Boltzmann learning](two-spin-boltzmann-learning.md)
- [Boltzmann encoder demonstration](boltzmann-encoder-demonstration.md)

## ↑ Ancestors (8)

1. [Neural network](neural-network.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Boltzmann machine](boltzmann-machine.md)
- [Hebbian learning](hebbian-learning.md)
- [Visible unit](visible-unit.md)
