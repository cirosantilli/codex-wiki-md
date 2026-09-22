<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

A [digital signature](../../../../../digital-signature.md) lets a holder of a private key authenticate a message while anyone with the public key verifies it. Signing a message digest ties the signature to the message and detects alterations; it does not conceal the message. Authentication also requires a trustworthy association of the public key with its owner.

For the [ElGamal signature scheme](../../../../../elgamal-signature-scheme.md), choose a large [prime](../../../../../prime-number.md) $p$ and a generator $g$ of $\mathbb F_p^\times$. The secret is $x$, and the public key is $(p,g,y)$ with $y=g^x\bmod p$. To sign a message whose hash is represented by $m\bmod(p-1)$, choose a fresh secret nonce $k$ coprime to $p-1$ and set

$$
\boxed{r=g^k\bmod p,\qquad s=k^{-1}(m-xr)\bmod(p-1).}
$$

Transmit $(r,s)$ with the message. Verification checks the permitted ranges and $\boxed{g^m\equiv y^r r^s\pmod p}$. Correctness follows from $xr+ks\equiv m\pmod{p-1}$. The secret exponent prevents an outsider from directly constructing this relation for an arbitrary hashed message; nonce reuse can expose the exponent through the repeated linear congruences. Hashing is part of the signature scheme, rather than signing arbitrary raw exponents with no message encoding.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
