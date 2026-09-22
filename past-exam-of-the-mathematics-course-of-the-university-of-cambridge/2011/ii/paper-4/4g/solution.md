<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

Use the [BB84 protocol](../../../../../bb84.md) to establish a secret random key, then encrypt the actual message with a [one-time pad](../../../../../one-time-pad.md). Alice chooses independent random bits and independently chooses between the computational [orthonormal basis](../../../../../orthonormal-basis.md) $\{|0\rangle,|1\rangle\}$ and the diagonal basis $\{|+\rangle,|-\rangle\}$, where $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. She sends one photon or other [qubit](../../../../../qubit.md) in each corresponding state. Bob independently chooses one of the two bases for each measurement.

Over an authenticated public classical channel, they announce their bases but not their bit values. They retain only positions where their bases match; absent disturbance these sifted bits agree. They disclose and discard a randomly selected test sample to estimate the error rate. If it is too large they abort. Otherwise they perform information reconciliation and [privacy amplification](../../../../../privacy-amplification.md) to produce a shared key about which an eavesdropper has negligible information. Authentication is essential: without it, an active attacker can impersonate the two parties. It may use a previously shared short authentication key, subsequently replenished from the new secret key.

The [no-cloning theorem](../../../../../no-cloning-theorem.md) prevents an attacker from copying an unknown nonorthogonal state perfectly: preservation of [inner products](../../../../../inner-product.md) would require $\langle\psi|\phi\rangle=\langle\psi|\phi\rangle^2$, impossible when its modulus is strictly between zero and one. In a simple intercept-and-resend attack, Eve chooses the wrong basis with probability $1/2$, and then introduces a wrong sifted bit with probability $1/2$. Thus the test error rate is $1/4$, and the probability that $m$ independent tested bits show no error is $(3/4)^m$. More general attacks are handled by bounding Eve's information from the observed statistics and shortening the reconciled key through [privacy amplification](../../../../../privacy-amplification.md).

Finally Alice sends $C=M\mathbin{\oplus}K$, using a uniform independent key of the message's length exactly once. The [one-time pad](../../../../../one-time-pad.md) makes the ciphertext independent of the message. **The security claim is secrecy with arbitrarily small failure probability after testing and [privacy amplification](../../../../../privacy-amplification.md)**, not that a finite quantum transmission can never be disturbed or intercepted. The scheme assumes trusted devices and an authenticated classical channel; it does not rely on a computational hardness assumption.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
