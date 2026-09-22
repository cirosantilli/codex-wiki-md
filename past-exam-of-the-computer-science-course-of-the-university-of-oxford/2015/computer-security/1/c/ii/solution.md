<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each candidate nonzero offset $k\in\{1,\ldots,2^{16}-1\}$, expansion gives

$$
\begin{aligned}
D_k&=c_2-c_1+2k^3\equiv3k(m^2+km+k^2),\\
N_k&=k(c_2+2c_1-k^3)\equiv3km(m^2+km+k^2).
\end{aligned}
$$

Consequently, if $D_k$ is invertible, the candidate is

$$
\boxed{m_k\equiv k(c_2+2c_1-k^3)(c_2-c_1+2k^3)^{-1}\pmod n.}
$$

Compute the [modular multiplicative inverse](../../../../../../modular-multiplicative-inverse.md) using the [extended Euclidean algorithm](../../../../../../extended-euclidean-algorithm.md), then verify both $m_k^3\equiv c_1$ and $(m_k+k)^3\equiv c_2\pmod n$. The [RSA cryptosystem](../../../../../../rsa-cryptosystem.md) cubing map is a [bijection](../../../../../../bijection.md), so an accepted candidate cannot be a different [plaintext](../../../../../../plaintext.md) with the same first [ciphertext](../../../../../../ciphertext.md). This costs fewer than $2^{16}$ trials, each involving polynomially many operations in the bit length of $n$.

There is a useful way to handle every denominator exception for a correct nonzero $k$. Compute $g=\gcd(D_k,n)$. If $1<g<n$, this [greatest common divisor](../../../../../../greatest-common-divisor.md) factors $n$, allowing ordinary [RSA cryptosystem](../../../../../../rsa-cryptosystem.md) [decryption](../../../../../../decryption.md). If $g=n$, then $D_k=0\pmod n$. The permitted [prime numbers](../../../../../../prime-number-split.md) are $2\pmod3$ and much larger than $k$, so $k$ is invertible modulo each. The equation $m^2+km+k^2=0$ would make $m/k$ a nontrivial cube root of one, impossible in a group of order [coprime](../../../../../../coprime-integers.md) to three. Thus $g=n$ cannot occur for the correct nonzero offset under these hypotheses.

If the bound in the question is read as also allowing $k=0$, then $c_1=c_2$ and there is no additional information: the problem reduces to inverting a single ordinary [RSA cryptosystem](../../../../../../rsa-cryptosystem.md) [ciphertext](../../../../../../ciphertext.md). The small-offset attack requires a nonzero difference; that is the natural reading of distinct related messages.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
