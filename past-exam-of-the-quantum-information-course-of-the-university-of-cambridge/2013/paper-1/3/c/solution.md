<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Quantum cryptography](../../../../../quantum-cryptography.md) includes [quantum key distribution](../../../../../quantum-key-distribution.md), which uses quantum transmissions and authenticated public discussion to establish a secret random key. In [BB84](../../../../../bb84.md), the sender independently chooses a random [bit](../../../../../bit.md) and either the computational or Hadamard basis, sending one of $|0\rangle,|1\rangle,|+\rangle,|-\rangle$. A receiver independently chooses one of those two bases. They announce bases after receipt, retain matching-basis positions and reveal a random sample of those bits to estimate noise or eavesdropping. Ideal uniform independent basis choices retain about half of the detected signals before testing and further processing.[1984 key-distribution protocol; original proceedings pp. 175–179](../../../../../quantum-cryptography-public-key-distribution-and-coin-tossing-by-charles-h-bennett-and-gilles-brassard.md)

The [no-cloning theorem](../../../../../no-cloning-theorem.md) prevents an adversary from copying arbitrary unknown nonorthogonal signal states perfectly. In a simple intercept–resend attack, the adversary chooses a random protocol basis. On half of the sifted positions it is the wrong basis, and the resent state then yields an erroneous receiver bit with [probability](../../../../../probability.md) one half. Thus the [BB84 intercept-resend error rate](../../../../../bb84-intercept-resend-error-rate.md) is

$$
\boxed{Q=\frac12\cdot\frac12=\frac14}
$$

if every signal is intercepted, or $Q=q/4$ when an independently selected fraction $q$ is attacked this way. This is an illustrative attack calculation, not a security proof against all possible quantum attacks.

After parameter estimation, classical error reconciliation aligns the remaining keys; [privacy amplification](../../../../../privacy-amplification.md) compresses them to remove the adversary's bounded information, including information leaked during public reconciliation. The classical channel requires [message authentication](../../../../../message-authentication.md), otherwise an attacker could impersonate each party to the other. Real sources, losses, multiphoton pulses and detector behavior must fit the security model. A low observed error rate alone is insufficient to certify arbitrary hardware. Finally the protocol distributes a key; encrypting a later message is a separate step.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
