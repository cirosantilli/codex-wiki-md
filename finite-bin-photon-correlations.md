# Finite-bin photon correlations

↑ **Parent:** [Photon counting](photon-counting.md)

For stationary continuous detection, let $C_j$ count all cross-channel pairs with $t_2-t_1$ in a bin of full width $\Delta\tau$, and let $r_1,r_2$ be observed single-count rates. Let $T_j$ be their joint live observation time at that delay, approximately the common duration $T_{\rm obs}$ when delays are short. Independent streams have expected pair count $r_1r_2T_j\Delta\tau$, giving the displayed estimator. It estimates a bin average of [second-order optical coherence](second-order-optical-coherence.md), further blurred by detector timing response. For a finite uninterrupted run the exact overlap weighting is $T_{\rm obs}-|\tau|$ inside the delay integral, rather than a constant at long delays.

For an original numerical example, choose $r_1=2000\,\mathrm{s^{-1}}$, $r_2=3000\,\mathrm{s^{-1}}$, $T_j=100\,\mathrm s$, and $\Delta\tau=10\,\mathrm{ns}$. The independent reference is six pairs per bin. Chosen counts $C_j=3,6,12$ give estimates $0.5,1,2$; they are teaching inputs with large counting fluctuations, not historical measurements. For pulsed sources, compare properly normalized same-pulse and separate-pulse coincidences instead of assuming this continuous-source baseline.

[Detector dead time](detector-dead-time.md) suppresses nearby same-detector counts and can manufacture an apparent dip in a single-detector record. Two independent detector channels avoid that particular same-channel exclusion, but shared electronics can still reject pairs. Timing spread and wide bins wash out narrow features. A device recording only the first stop after each start measures a waiting-time distribution; interpreting it as all-pair correlations requires a sufficiently low stop probability over the relevant delay range.

## ↑ Ancestors (6)

1. [Photon counting](photon-counting.md)
2. [Quantum optics](quantum-optics-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
