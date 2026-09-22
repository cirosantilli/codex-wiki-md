# Bit commitment

↑ **Parent:** [Cryptography](cryptography.md)

A bit commitment allows a sender to fix a bit while concealing it from the receiver until an opening phase. Binding prevents a sender from opening the same commitment as either bit; hiding prevents the receiver from learning the bit prematurely. With a [one-way permutation](one-way-permutation.md) $F$ and a [hard-core predicate](hard-core-predicate.md) $h$, a commitment can consist of $F(x)$ and the masked bit $b\mathbin{\oplus}h(x)$. Opening reveals $x$. Injectivity gives binding, while unpredictability of the [hard-core predicate](hard-core-predicate.md) gives computational hiding. For an [RSA cryptosystem](rsa-cryptosystem.md), the receiver must not possess the inverse trapdoor.

**Table of contents**

- [Ensemble-steering attack on quantum bit commitment](ensemble-steering-attack-on-quantum-bit-commitment.md)

## ↑ Ancestors (3)

1. [Cryptography](cryptography.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [One-way permutation](one-way-permutation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/12g/solution.md)
