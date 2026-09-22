<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

In the [RSA cryptosystem](../../../../../rsa-cryptosystem.md), choose distinct large [prime numbers](../../../../../prime-number.md) $p,q$, set $N=pq$, and choose $e$ [coprime](../../../../../coprime-integers.md) to $\varphi(N)=(p-1)(q-1)$. Choose $d$ with $ed\equiv1\pmod{\varphi(N)}$. A plaintext [residue class](../../../../../residue-class.md) $m$ is encrypted as $c=m^e\pmod N$ and decrypted as $c^d\pmod N$. [Fermat's little theorem](../../../../../fermat-little-theorem.md) modulo $p$ and $q$, followed by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md), proves correctness even when $m$ is not [coprime](../../../../../coprime-integers.md) to $N$.

Textbook [RSA cryptosystem](../../../../../rsa-cryptosystem.md) is multiplicative: $E(m_1m_2)=E(m_1)E(m_2)\pmod N$. For a [chosen-ciphertext attack](../../../../../chosen-ciphertext-attack.md), multiply an intercepted $c$ by $r^e$ for a known invertible $r$. A decryption oracle returns $mr$, from which multiplication by $r^{-1}$ recovers $m$. Likewise, multiplying two textbook [RSA signatures](../../../../../rsa-signature.md) produces a signature of their product. These are [homomorphism attacks](../../../../../homomorphism-attack.md), exploiting algebra rather than factoring $N$.

For an [ElGamal signature](../../../../../elgamal-signature-scheme.md), choose a [prime](../../../../../prime-number.md) $p$, a [primitive root](../../../../../primitive-root-modulo-n.md) $g$ modulo $p$, a private exponent $a$, and public $y=g^a$. To sign a message digest $h=H(m)$, choose a fresh secret $k$ [coprime](../../../../../coprime-integers.md) to $p-1$ and set

$$
\boxed{r=g^k\pmod p,\qquad s=k^{-1}(h-ar)\pmod{p-1}.}
$$

Verification checks $1\leq r\leq p-1$ and $g^{H(m)}\equiv y^r r^s\pmod p$, which follows because $ar+ks\equiv h\pmod{p-1}$. Authenticating the ciphertext and its context with such a [digital signature](../../../../../digital-signature.md), before decryption, prevents the simple multiplicative modification from being accepted without a fresh valid signature. One needs an appropriate [cryptographic hash function](../../../../../cryptographic-hash-function.md) and fresh secret [cryptographic nonces](../../../../../cryptographic-nonce.md): this is not a claim that every algebraic attack is impossible. In particular, the unhashed historical [ElGamal signature scheme](../../../../../elgamal-signature-scheme.md) admits existential forgeries of specially chosen message exponents; mere multiplication of encrypted messages is not an authentication mechanism.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
