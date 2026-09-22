<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

For [Rabin cryptosystem](../../../../../rabin-cryptosystem.md), choose primes $p,q\equiv3\pmod4$, publish $N=pq$, and encrypt $x$ as $x^2\bmod N$. The factors let the receiver take square roots modulo $p$ and $q$ and combine them using the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md); redundancy identifies the intended one of four roots.

For [RSA cryptosystem](../../../../../rsa-cryptosystem.md), choose $N=pq$, select $e$ coprime to $\varphi(N)$ and $d$ with $ed\equiv1\pmod{\varphi(N)}$. Encrypt $x$ as $x^e$ and decrypt by raising to $d$ modulo $N$. Rabin inversion is provably equivalent to factoring, while ordinary RSA lacks that reduction; Rabin's disadvantage is its fourfold decryption ambiguity.

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
