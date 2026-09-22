<h1 id="12k/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [RSA cryptosystem](../../../../../../../rsa-cryptosystem.md), choose $N=pq$ and a public exponent $e$ coprime to $\phi(N)$. The public key is $(N,e)$, while the private exponent satisfies

$$
ed\equiv1\pmod{\phi(N)}.
$$

Encryption sends $m$ to $c\equiv m^e\pmod N$, and decryption computes $c^d\equiv m\pmod N$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [12K](../../../12k.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
