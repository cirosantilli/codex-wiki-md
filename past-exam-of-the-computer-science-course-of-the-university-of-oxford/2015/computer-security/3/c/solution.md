<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [existential forgery](../../../../../existential-forgery.md) produces a valid [digital signature](../../../../../digital-signature.md) on at least one new message, even if the adversary has no useful control over that message's meaning. A [universal forgery](../../../../../universal-forgery.md) gives a way to forge a [digital signature](../../../../../digital-signature.md) on an arbitrary specified message. Recovering the [private key](../../../../../private-key.md) suffices for a [universal forgery](../../../../../universal-forgery.md), but is not required if another general signing method exists.

In a [key-only signature attack](../../../../../key-only-signature-attack.md), the adversary knows the verification [public key](../../../../../public-key.md) and the public scheme. In a [known-message signature attack](../../../../../known-message-signature-attack.md), it additionally obtains valid message–[digital signature](../../../../../digital-signature.md) pairs whose messages it did not choose. In a [chosen-message signature attack](../../../../../chosen-message-signature-attack.md), it can ask for [digital signatures](../../../../../digital-signature.md) on messages it chooses, possibly adaptively. Its final forged message must not be one of the messages already submitted for signing; otherwise simply returning a supplied pair would count as a forgery.

$$
\boxed{\text{Existential: some new message; universal: an arbitrary target message.}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Computer security](../../../computer-security-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
