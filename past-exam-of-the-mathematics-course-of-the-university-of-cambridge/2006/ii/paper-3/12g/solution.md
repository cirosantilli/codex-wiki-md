<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

In the [RSA cryptosystem](../../../../../rsa-cryptosystem.md), choose distinct large [primes](../../../../../prime-number.md) $p,q$, put $N=pq$, choose $e$ [coprime](../../../../../coprime-integers.md) to $\varphi(N)=(p-1)(q-1)$, and choose $d$ with $ed\equiv1\pmod{\varphi(N)}$. Publish $(N,e)$ and keep the factorization and $d$ private. Encrypt a properly encoded message $M$ as $C=M^e\bmod N$ and decrypt as $M=C^d\bmod N$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) proves correctness even for nonunits: modulo either prime, the message is either zero or satisfies [Fermat's little theorem](../../../../../fermat-little-theorem.md).

The public exponent $65537=2^{16}+1$ has few nonzero binary digits, so exponentiation needs only sixteen squarings and one extra multiplication. It is an efficient conventional choice, subject to the required [coprimality](../../../../../coprime-integers.md) and secure randomized message encoding. The same numerical choice for the private exponent would speed decryption, but for large moduli with balanced prime factors it is disastrously small: the continued-fraction attack on a small RSA private exponent recovers $d$ when, for example, $d<\frac13N^{1/4}$ and $q<p<2q$. **A small public exponent and a small private exponent have very different security implications.**

To factor $N$ from $e,d$, write $ed-1=2^st$ with $t$ odd. Choose random $a$ modulo $N$. If $\gcd(a,N)$ is nontrivial, factoring is already done. Otherwise compute $b=a^t$ and repeatedly square; the final value is one. If a value $x$ immediately preceding the first one is neither $1$ nor $-1$ modulo $N$, then $x^2\equiv1\pmod N$ and

$$
\boxed{\gcd(x-1,N)\text{ is a nontrivial factor of }N.}
$$

Indeed, the signs of $x$ modulo $p$ and $q$ differ. Restart if the chain begins at one or reaches $-1$ first. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) makes the two prime components independent for a uniformly chosen unit. Their two-primary orders differ with probability at least one half: if the two exponents of two in $p-1,q-1$ are equal, the probability of equal orders is at most one half, and if unequal it is smaller. Since odd $t$ preserves these orders, this gives a randomized factoring procedure with bounded expected repetitions.

A [bit commitment](../../../../../bit-commitment.md) must be hiding before opening and binding after it. A concrete RSA construction uses a valid public RSA permutation whose inverse is unavailable to the receiver. Choose a random unit $x$ and a random bit vector $r$, and set $h(x,r)$ to their binary inner product modulo two. Send $y=x^e\bmod N$, $r$, and $c=b\mathbin{\oplus}h(x,r)$. To open, reveal $x$; the receiver checks $x^e=y$ and recovers $b=c\mathbin{\oplus}h(x,r)$. Injectivity makes the opening bit unique. The [hard-core predicate](../../../../../hard-core-predicate.md) theorem applied to $(x,r)\mapsto(x^e,r)$ gives computational hiding under the RSA inversion assumption. The setup must ensure a valid modulus and exponent without giving the receiver the private exponent; otherwise hiding fails. Merely encrypting $0$ or $1$ would not hide a bit, since both ciphertexts could be computed publicly.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
