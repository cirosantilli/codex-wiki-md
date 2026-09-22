<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use an [Ekert protocol](../../../../ekert-protocol.md). Alice and Bob choose their analyzer settings independently and randomly for each received pair, record the outcomes, and confirm reception before announcing settings over an [authenticated public classical channel](../../../../authenticated-public-classical-channel.md). The authentication prevents an adversary from impersonating either party; it does not conceal the setting announcements. Announcing settings after reception also avoids the [premature basis announcement in quantum key distribution](../../../../premature-basis-announcement-in-quantum-key-distribution.md) attack.

The [polarization correlations of the Psi-plus Bell state](../../../../polarization-correlations-of-the-psi-plus-bell-state.md) satisfy

$$
E_{ij}=\langle\Psi^+|A_i\otimes B_j|\Psi^+\rangle,
\qquad E(\alpha,\beta)=-\cos 2(\alpha+\beta).
$$

Indeed, $\langle Z\otimes Z\rangle=-1$, $\langle X\otimes X\rangle=1$, and the cross terms vanish. In the specified setting order,

$$
(E_{ij})=\begin{pmatrix}
-1&-1/\sqrt2&-1/\sqrt2\\
0&-1/\sqrt2&1/\sqrt2\\
-1/\sqrt2&-1&0
\end{pmatrix}.
$$

For [key sifting](../../../../key-sifting.md), retain the setting pairs **$(i,j)=(1,1)$ and $(3,2)$**. Their outcomes are perfectly anticorrelated. Alice assigns bit $0$ to outcome $+1$ and bit $1$ to outcome $-1$; Bob uses the opposite assignment. Their [raw keys](../../../../raw-key.md) then agree. With uniform independent choices of the three settings, these pairs supply a raw-key fraction **$2/9$**, before sacrificing a test sample. They must keep the remaining raw-key outcomes secret. The four pairs $(1,2),(1,3),(2,2),(2,3)$ supply Bell-test data, and the other three setting pairs can be discarded.

Reveal the outcomes of those Bell-test rounds and estimate

$$
E_{ij}=\frac{N_{++}+N_{--}-N_{+-}-N_{-+}}{N_{++}+N_{--}+N_{+-}+N_{-+}},
\qquad
\boxed{S=-E_{12}-E_{13}-E_{22}+E_{23}.}
$$

The ideal entries give **$S=2\sqrt2$**. The [CHSH inequality](../../../../chsh-inequality.md) gives $|S|\le2$ for [local hidden-variable theories](../../../../local-hidden-variable-theory.md): for predetermined outcomes $a_1,a_2,b_2,b_3\in\{\pm1\}$, the signed combination is $-a_1(b_2+b_3)-a_2(b_2-b_3)$. One bracket is zero and the other is $\pm2$, so averaging cannot exceed two in magnitude. The [Tsirelson bound](../../../../tsirelson-s-bound.md) limits quantum correlations to $2\sqrt2$.

For the specified, trusted [Pauli operators](../../../../pauli-operator.md), the [maximal CHSH witness for a fixed Bell state](../../../../maximal-chsh-witness-for-a-fixed-bell-state.md) makes the ideal security statement precise. Its operator is

$$
\mathcal B=-A_1\otimes(B_2+B_3)-A_2\otimes(B_2-B_3)
=\sqrt2(X\otimes X-Z\otimes Z).
$$

Its largest [eigenvalue](../../../../eigenvalue.md) $2\sqrt2$ has the unique [eigenvector](../../../../eigenvector.md) $|\Psi^+\rangle$. Exact attainment therefore fixes the shared [density matrix](../../../../density-matrix-split.md) to this [pure state](../../../../pure-state.md). Since [purity decouples a subsystem from its purification](../../../../purity-decouples-a-subsystem-from-its-purification.md), Eve cannot hold information correlated with that pair. This rules out information-gaining eavesdropping in the ideal model, rather than proving that no observer exists. More generally, [CHSH self-testing](../../../../chsh-self-testing.md) identifies the entangled qubit pair up to local changes of representation under its own assumptions.

A [quantum measurement](../../../../quantum-measurement-split.md) that reads Eve's chosen polarization generally disturbs correlations in an incompatible basis. The [no-cloning theorem](../../../../no-cloning-theorem.md) also prevents copying arbitrary unknown photon polarizations and retaining a perfect copy while forwarding an unchanged original. The Bell test checks several incompatible settings, so observing perfect correlation in only one key basis is insufficient.

Alice and Bob also reveal a randomly chosen sample of their raw keys to estimate the [quantum bit error rate](../../../../quantum-bit-error-rate.md), then discard that sample. [Information reconciliation](../../../../information-reconciliation.md) corrects discrepancies, and [privacy amplification](../../../../privacy-amplification.md) removes residual information, including leakage from the public transcript. With finite data they need statistical bounds and a security analysis appropriate to their devices and noise. A measured violation $S>2$ alone does not assert zero information for Eve; the exact ideal argument above uses the maximal value.[Original 1991 proposal connecting Bell-correlation tests to quantum key distribution](../../../../quantum-cryptography-based-on-bell-s-theorem-by-artur-k-ekert.md)

## ↑ Ancestors (12)

1. [2](../2.md)
2. [8](../../8-split.md)
3. [2009](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
