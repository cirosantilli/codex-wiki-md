# Photon correlation loss and background model

↑ **Parent:** [Photon counting](photon-counting.md)

Independent loss alone leaves normalized [factorial moments](factorial-moment.md) invariant: if every input [photon](photon.md) is retained with [probability](probability.md) $\eta$, [binomial thinning conditional on a total](binomial-thinning-conditional-on-a-total.md) gives $\langle K\rangle=\eta\mu$ and $\langle K(K-1)\rangle=\eta^2\langle N(N-1)\rangle$. Both powers cancel from $g^{(2)}(0)$. Fewer coincidences still mean poorer statistical precision.

Now let each channel contain a signal rate $s_i$ and an independent [Poisson process](poisson-process-split.md) background rate $b_i$, independent also of the signal. Put $\rho_i=s_i/(s_i+b_i)$. The pair density is $s_1s_2g^{(2)}_{\rm sig}+s_1b_2+b_1s_2+b_1b_2$. Dividing by $(s_1+b_1)(s_2+b_2)$ proves the displayed formula, for the same bin and timing response. For chosen equal signal fractions $\rho_1=\rho_2=4/5$, ideal signal values $0,1,2$ become $9/25,1,41/25$. Background pulls both dips and peaks toward one.

This calculation assumes additive, mutually independent background counts. Scattered coherent [light](light.md) that interferes with the signal, correlated electronic noise, or recovery effects require a different model. Correcting a dip without independently estimating the backgrounds cannot establish [photon antibunching](photon-antibunching.md).

## ↑ Ancestors (6)

1. [Photon counting](photon-counting.md)
2. [Quantum optics](quantum-optics-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Finite-response stellar intensity correlations](finite-response-stellar-intensity-correlations.md)
