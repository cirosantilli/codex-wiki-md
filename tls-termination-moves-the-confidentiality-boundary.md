# TLS termination moves the confidentiality boundary

↑ **Parent:** [TLS termination](tls-termination.md)

Suppose [client](network-client.md) A uses a protected channel to proxy P, which reads the message and sends it over a second protected channel to service B. Even if both channels protect against outsiders, P has the plaintext by construction. Therefore the conjunction of those channel protections does not imply [cryptographic confidentiality](cryptographic-confidentiality.md) from P. This counterexample does not imply that P is unauthorised; it identifies a trust assumption that application designers must state.

## ↑ Ancestors (5)

1. [TLS termination](tls-termination.md)
2. [Transport Layer Security](transport-layer-security.md)
3. [Cryptography](cryptography.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2020/1/solution.md)
