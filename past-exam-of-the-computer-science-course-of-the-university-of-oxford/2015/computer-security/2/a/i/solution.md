<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Bilateral authentication](../../../../../../bilateral-authentication.md) means that each participant obtains assurance of the other's identity and participation in the relevant run: Alice authenticates Bob and Bob authenticates Alice. An observed name in a message is not such assurance. The [protocol](../../../../../../communication-protocol.md) must prevent an adversary from supplying the evidence while the named peer is absent.

[Session key transport](../../../../../../session-key-transport.md) means conveying an already selected [session key](../../../../../../session-key.md) securely to its intended users. Here Tim selects $k_{AB}$ and sends it inside separate public-key-encrypted tickets for Alice and Bob. This differs from having Alice and Bob jointly derive a key to which both contribute.

$$
\boxed{\text{Both peers authenticate; Tim chooses and transports their session key.}}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
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
