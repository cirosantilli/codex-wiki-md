<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

This is an entanglement-based [quantum key distribution](../../../../../quantum-key-distribution.md) scheme of the type proposed by [Artur K. Ekert](../../../../../artur-k-ekert.md).[1991 primary proposal: Bell correlations used to test a key-distribution channel](../../../../../quantum-cryptography-based-on-bell-s-theorem-by-artur-k-ekert.md) The measurements generate correlated random data; Alice does not choose a message by choosing their random outcomes.

After the measurements, Alice and Bob announce their basis choices over an authenticated public channel. They retain the pairs with equal axes, here $(\mathbf a_2,\mathbf b_1)$ and $(\mathbf a_3,\mathbf b_2)$, and Bob flips his outcome signs to match Alice's bits. They sacrifice a random subset for error estimation and use the appropriate other setting combinations to estimate $S$. In the ideal source the same-axis bits match after the flip and $S=-2\sqrt2$; the specified intercept-resend attack cannot reproduce that value.

A practical protocol includes information reconciliation, an accounting of information leaked publicly, and [privacy amplification](../../../../../privacy-amplification.md). It must abort when its statistical security conditions fail. Authentication is essential: a completely unauthenticated public channel permits a [man-in-the-middle attack](../../../../../man-in-the-middle-attack.md). A Bell-violation observation alone, without sampling, device and adversary assumptions and a finite-key analysis, is not a proof that Eve knows no key bits.

With a sufficiently uniform secret shared key $k$ of the required length, Alice can send $c=m\oplus k$ publicly using a [one-time pad](../../../../../one-time-pad.md); Bob recovers $m=c\oplus k$. **The pad must be secret, as long as the protected message, and never reused.** A complete security proof makes the probability or distinguishing advantage of failure small under stated assumptions. The ideal exam correlations diagnose the stated attack; they do not provide an unconditional guarantee against every attack or implementation fault.

## ↑ Ancestors (14)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
