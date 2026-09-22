<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Quantum cryptography](../../../../../quantum-cryptography.md) includes [quantum key distribution](../../../../../quantum-key-distribution.md), which establishes a shared secret key rather than transmitting an arbitrary plaintext directly. In [BB84](../../../../../bb84.md), Alice randomly prepares one of the two computational-basis or two complementary-basis [qubit](../../../../../qubit.md) states; Bob randomly measures in either basis. They announce bases over an authenticated classical channel and retain the positions where their choices agree, about half in the ideal unbiased case. They test a subset for errors, reconcile the remaining strings, and apply [privacy amplification](../../../../../privacy-amplification.md) to remove a bounded eavesdropper's information. A protocol can abort when the observed data do not support a secret key.[1984 protocol; authors' later upload of the original proceedings contribution](../../../../../quantum-cryptography-public-key-distribution-and-coin-tossing-by-charles-h-bennett-and-gilles-brassard.md)

Nonorthogonal states cannot be perfectly copied by a state-independent device, by the [no-cloning theorem](../../../../../no-cloning-theorem.md). An intercept-resend attacker who measures each signal in a random [BB84](../../../../../bb84.md) basis chooses the wrong basis half the time. On those sifted positions Bob has a one-half error [probability](../../../../../probability.md), giving the ideal [BB84 intercept-resend error rate](../../../../../bb84-intercept-resend-error-rate.md) $1/4$. This simple calculation demonstrates detectable disturbance for that attack; it is not a complete security proof for arbitrary attacks.

Authentication is essential: otherwise an adversary can impersonate both participants. Error correction reveals information that must be included in the privacy budget, and losses, finite sample sizes, multiphoton emission and detector behavior belong in the security model. Entanglement-based variants can use Bell [correlations](../../../../../pearson-correlation-coefficient.md), but observing some entanglement or a Bell violation alone does not replace a quantitatively specified key-distillation protocol. The final key can subsequently be used in a suitable classical encryption scheme.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum information course of the University of Cambridge](../../../../split.md)
6. [Quantum Information course of the University of Cambridge](../../../../../quantum-information-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
