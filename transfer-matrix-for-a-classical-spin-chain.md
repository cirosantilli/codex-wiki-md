# Transfer matrix for a classical spin chain

↑ **Parent:** [Spin model](spin-model.md)

For a nearest-neighbour classical chain with finitely many spin states and dimensionless bond energy $E(s,t)$, its transfer [matrix](matrix.md) is $W_{st}=e^{-E(s,t)}$. On-site energies are divided between adjacent bonds. [Periodic boundary conditions](periodic-boundary-conditions.md) give [partition function](canonical-partition-function.md) $Z_N=\operatorname{tr}W^N$ by direct multiplication and summation over spin labels. For a strictly positive [symmetric matrix](symmetric-matrix.md), the [Perron–Frobenius theorem](perron-frobenius-theorem.md) gives $\lim_{N\to\infty}N^{-1}\log Z_N=\log\lambda_{\max}$. A diagonal local observable $O$ has [expectation](expected-value.md) $\operatorname{tr}(OW^N)/Z_N$, tending to $v_{\max}^TOv_{\max}$ for a normalized dominant [eigenvector](eigenvector.md).

**Table of contents**

- [Classical Ising chain as a quantum particle](classical-ising-chain-as-a-quantum-particle.md)
  - [Auxiliary-field transfer operator for an Ising chain](auxiliary-field-transfer-operator-for-an-ising-chain.md)
  - [Double-well threshold of an auxiliary Ising potential](double-well-threshold-of-an-auxiliary-ising-potential.md)

## ↑ Ancestors (5)

1. [Spin model](spin-model.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
