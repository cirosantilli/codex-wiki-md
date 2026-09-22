<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

In [RSA](../../../../../rsa-cryptosystem.md), choose $N=pq$ with distinct large primes, an exponent $e$ coprime to $\varphi(N)$, and $d$ satisfying $ed\equiv1\pmod{\varphi(N)}$. Publish $(N,e)$ and keep $d$ secret. Encrypt a [residue](../../../../../residue.md) $m$ as $c=m^e\bmod N$ and decrypt by $c^d\bmod N$. [Fermat's little theorem](../../../../../fermat-little-theorem.md) on each prime and the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) prove decryption, including messages not coprime to $N$.

A customer knows a nonzero multiple $M=ed-1$ of $\varphi(N)$. Write $M=2^st$ with $t$ odd. Choose a base $a$ at random. A nontrivial $\gcd(a,N)$ already factors $N$. Otherwise compute $a^t,a^{2t},\ldots,a^{2^st}$ modulo $N$. The last entry is $1$. If the first occurrence of $1$ is preceded by $z\not\equiv\pm1\pmod N$, then

$$
\boxed{\gcd(z-1,N)\text{ is a nontrivial factor of }N.}
$$

Indeed, the two prime components of this square root of $1$ must have opposite signs. This procedure succeeds for some bases: by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md), choose a base whose component modulo $p$ has order $2$ and whose component modulo $q$ has order $1$. Its odd $t$-th power is already a nontrivial square root of $1$. Trying bases therefore gives an explicit factoring algorithm, and repeated random choices give the usual efficient attack. More precisely, if the two components' orders have different powers of $2$, the procedure succeeds. For a uniform element of a cyclic group with $2$-part $2^r$, those order valuations have probabilities $2^{-r}$ for $0$ and $2^{j-1-r}$ for $1\leq j\leq r$. Independence of the two prime components shows that equal valuations have probability at most $1/2$. Thus a random unit succeeds with probability at least $1/2$. Once $N$ is factored, every customer's private exponent is computable. The exceptional $ed=1$ is an identity cipher and is already insecure.

For the outsider's [RSA common-modulus attack](../../../../../common-modulus-rsa-attack.md), find integers $a,b$ with $ae_1+be_2=1$ by [Bézout's identity](../../../../../bezout-identity.md). For a unit message,

$$
\boxed{m\equiv c_1^a c_2^b\pmod N,}
$$

using modular inverses for negative powers. If a ciphertext is a nonzero nonunit, its greatest common divisor with $N$ factors $N$ instead; zero ciphertext corresponds to the zero message for a squarefree modulus. **The common message is recoverable without a private key.** For a generic unit message this alone does not supply the factorization or all private keys, so it does not demonstrate a complete break for unrelated messages. The nonunit case does give that stronger break.

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
