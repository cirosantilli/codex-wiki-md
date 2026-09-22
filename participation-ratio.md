# Participation ratio

↑ **Parent:** [Localized eigenstate](localized-eigenstate.md)

For an [eigenvector](eigenvector.md) normalized by $\sum_{n=1}^N|\psi_n|^2=1$, the [participation ratio](participation-ratio.md) in its site basis is

$$
P=\frac{1}{\sum_{n=1}^N|\psi_n|^4},\qquad 1\leq P\leq N.
$$

It estimates how many sites carry appreciable probability. Equal weight on $K$ sites and zero elsewhere gives $P=K$, irrespective of their [wave phases](phase-waves.md). A single occupied site gives $P=1$; uniform probability on all sites gives $P=N$. These are exact constructed examples, not claims about particular [Hamiltonian operators](hamiltonian-quantum-mechanics.md).

To prove the bounds, write $p_n=|\psi_n|^2$. Since $0\leq p_n\leq1$, $\sum_np_n^2\leq\sum_np_n=1$, giving $P\geq1$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $1=(\sum_np_n)^2\leq N\sum_np_n^2$, giving $P\leq N$. Thus the measure has useful limits without assuming an exponential shape. Comparing $P$ as $N$ increases helps distinguish a state filling the sample from one occupying a fixed region, provided [energy](energy-split.md) selection and disorder statistics are controlled.

## ↑ Ancestors (8)

1. [Localized eigenstate](localized-eigenstate.md)
2. [Anderson localization](anderson-localization.md)
3. [Wave propagation in a random medium](wave-propagation-in-a-random-medium.md)
4. [Random medium](random-medium.md)
5. [Wave scattering](wave-scattering.md)
6. [Wave](wave-split.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Localization length](localization-length.md)
- [Localized eigenstate](localized-eigenstate.md)
- [One-dimensional Anderson chain](one-dimensional-anderson-chain.md)
- [Participation ratio](participation-ratio.md)
