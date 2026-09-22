# Memoryless quantum channel

↑ **Parent:** [Quantum channel](quantum-channel.md)

A memoryless quantum channel has independent identical noise on successive uses, described by the tensor-power map $\Phi^{\otimes n}$. This factorization does not restrict the encoder to product inputs: one can feed an [entangled state](entangled-state.md) across uses. A block code with equally likely messages $m$ chooses states $\rho_m$ and a decoder [POVM](positive-operator-valued-measure.md) $(D_m)$. Its average error is $1-|\mathcal M|^{-1}\sum_m\operatorname{Tr}[D_m\Phi^{\otimes n}(\rho_m)]$, and its rate is $n^{-1}\log_2|\mathcal M|$. The [classical capacity of a quantum channel](classical-capacity-of-a-quantum-channel.md) allows such entangled block inputs; the one-use [Holevo capacity](holevo-capacity.md) gives the product-input capacity and requires regularization in general.

**Table of contents**

- [Quantum erasure channel](quantum-erasure-channel.md)
  - [Entanglement-assisted capacity of a quantum erasure channel](entanglement-assisted-capacity-of-a-quantum-erasure-channel.md)
- [Entanglement-assisted classical capacity](entanglement-assisted-classical-capacity.md)

## ↑ Ancestors (8)

1. [Quantum channel](quantum-channel.md)
2. [Completely positive map](completely-positive-map.md)
3. [Positive linear map](positive-linear-map.md)
4. [Quantum information theory](quantum-information-theory-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Entanglement-assisted classical capacity](entanglement-assisted-classical-capacity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/5/solution.md)
