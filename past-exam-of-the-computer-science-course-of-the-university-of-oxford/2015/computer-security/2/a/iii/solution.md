<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the [Dolev-Yao model](../../../../../../dolev-yao-model.md), an adversary controls the network: it can intercept, suppress, delay, replay and redirect messages, impersonate network senders, and construct messages from values it knows. In particular, it can concatenate or split unprotected tuples, and can apply [encryption](../../../../../../encryption.md) using any known [public key](../../../../../../public-key.md) or known symmetric key.

[Cryptography](../../../../../../cryptography.md) is idealised. Without the required [private key](../../../../../../private-key.md) or symmetric key, the adversary cannot recover a protected [plaintext](../../../../../../plaintext.md) or construct an otherwise unavailable protected value. It cannot invent an unknown long-term secret merely because the containing [ciphertext](../../../../../../ciphertext.md) is visible. [Protocol](../../../../../../communication-protocol.md) failures arise from the arrangement of messages even when these cryptographic primitives behave perfectly.

$$
\boxed{\text{Complete network control, with perfect cryptographic operations.}}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
