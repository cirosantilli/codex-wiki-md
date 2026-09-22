# Measurement characterization of quantum fidelity

↑ **Parent:** [Fidelity of quantum states](fidelity-of-quantum-states.md)

A [POVM](positive-operator-valued-measure.md) $\{E_i\}$ gives outcome [probability distributions](probability-distribution-split.md) $p_i=\operatorname{Tr}(\rho E_i)$ and $q_i=\operatorname{Tr}(\sigma E_i)$ by the [Born rule](born-rule.md). Their classical overlap, the [Bhattacharyya coefficient](bhattacharyya-coefficient.md), is $B(p,q)=\sum_i\sqrt{p_iq_i}$. Fuchs and Caves showed that minimizing this overlap over all [POVMs](positive-operator-valued-measure.md) gives the [unsquared quantum fidelity](fidelity-of-quantum-states.md):

$$
F(\rho,\sigma)=\min_{\{E_i\}}B(p,q)=\min_{\{E_i\}}\sum_i\sqrt{\operatorname{Tr}(\rho E_i)\operatorname{Tr}(\sigma E_i)}.
$$

The same [POVM](positive-operator-valued-measure.md) is applied to either possible input [quantum state](quantum-state.md). Each [measurement in quantum mechanics](quantum-measurement-split.md) has $B(p,q)\geq F$; some measurement attains equality, including when the [density operators](density-matrix-split.md) have zero [eigenvalues](eigenvalue.md). Thus [quantum fidelity](fidelity-of-quantum-states.md) quantifies the smallest classical overlap that observation can reveal. For [fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md), measurement in a common [eigenbasis](eigenbasis.md) attains the minimum. This operational interpretation compares statistics without assigning a probability that two [mixed states](mixed-state.md) are equal. [Fuchs and Caves, Mathematical Techniques for Quantum Communication Theory, equations 5–6 and 17; published 1995, archived 1996](https://arxiv.org/pdf/quant-ph/9604001v1) [Watrous, The Theory of Quantum Information, Theorem 3.24, including singular density operators](https://jhwatrous.github.io/TQI.3.pdf#page=30)

## ↑ Ancestors (6)

1. [Fidelity of quantum states](fidelity-of-quantum-states.md)
2. [Quantum information theory](quantum-information-theory-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bhattacharyya coefficient](bhattacharyya-coefficient.md)
- [Fidelity of quantum states](fidelity-of-quantum-states.md)
- [Squared quantum fidelity](squared-quantum-fidelity.md)
