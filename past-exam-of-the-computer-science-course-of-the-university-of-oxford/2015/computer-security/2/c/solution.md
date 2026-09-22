<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [denial-of-service attack](../../../../../denial-of-service-attack.md) can exploit both an honest relay and replay at Tim. The adversary repeatedly sends cheap unauthenticated message-1 requests naming Alice and Bob. Bob then performs the public-key [encryption](../../../../../encryption.md) in message 2, and Tim performs a private-key [decryption](../../../../../decryption.md), generates a [session key](../../../../../session-key.md), looks up the users' records and performs two public-key [encryptions](../../../../../encryption.md). The adversary's first messages contain no cryptographic work.

Alternatively, after observing one valid message 2, the adversary submits copies directly to Tim. It remains well formed; the printed [protocol](../../../../../communication-protocol.md) has no request-replay cache. Tim's promise to reject malformed requests does not imply duplicate suppression. Each replay can provoke the expensive operations again. If such a cache is added, the repeated-message-1 method still induces distinct requests through Bob unless admission is controlled.

$$
\boxed{\text{Unauthenticated initiations or replayed valid requests amplify work at Tim.}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computer security](../../../computer-security-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
