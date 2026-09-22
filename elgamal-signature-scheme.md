# ElGamal signature scheme

↑ **Parent:** [Digital signature](digital-signature.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ElGamal_signature_scheme)

For a [prime number](prime-number.md) $p$, [primitive root](primitive-root-modulo-n.md) $g$ and [public key](public-key.md) $y=g^a$, choose a fresh secret $k$ [coprime](coprime-integers.md) to $p-1$, set $r=g^k\pmod p$ and $s=k^{-1}(H(m)-ar)\pmod{p-1}$, and verify $g^{H(m)}=y^r r^s\pmod p$. Reusing the [cryptographic nonce](cryptographic-nonce.md) can reveal secret information. The unhashed historical construction allows existential forgery of specially chosen message exponents, so authentication claims require suitable hashing and protocol assumptions.

## ↑ Ancestors (4)

1. [Digital signature](digital-signature.md)
2. [Cryptography](cryptography.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cryptographic nonce](cryptographic-nonce.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/3g/solution.md)
