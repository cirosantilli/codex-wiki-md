<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A [digital signature](../../../../../digital-signature.md) lets the holder of a [private key](../../../../../private-key.md) authenticate a message so that anyone with the corresponding trusted [public key](../../../../../public-key.md) can verify its origin and integrity. The signature does not conceal the message. Public-key certification, a suitable message hash and protection of the signing key are needed for that interpretation.

For the [ElGamal signature scheme](../../../../../elgamal-signature-scheme.md), choose a large prime $p$ and a [primitive root](../../../../../primitive-root-modulo-n.md) $g$ modulo $p$. The secret key is $x$, and the [public key](../../../../../public-key.md) is $(p,g,y)$ with $y=g^x\bmod p$. Represent the message by a hash $m$ modulo $p-1$. Choose a fresh secret nonce $k$ coprime to $p-1$ and set

$$
\boxed{r=g^k\bmod p,\qquad s=k^{-1}(m-xr)\bmod(p-1).}
$$

The signature is $(r,s)$. After checking the prescribed ranges, the verifier accepts when

$$
\boxed{g^m\equiv y^r r^s\pmod p.}
$$

A genuine signature passes because $xr+ks\equiv m\pmod{p-1}$. The security aim is that someone without $x$ cannot efficiently produce a valid signature on a new authenticated message. Nonce secrecy and freshness matter: reuse gives linear congruences relating two message hashes, the nonce and the secret key. Signing unhashed arbitrary messages also permits algebraic forgeries, so the hash is part of the practical scheme.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
