<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

In the [Rabin cryptosystem](../../../../../rabin-cryptosystem.md), choose distinct large odd primes $p,q$, publish $N=pq$, and encrypt $m$ as $c=m^2\bmod N$. Usually $p,q\equiv3\pmod4$, so a square root modulo each prime is obtained by exponentiating to $(p+1)/4$ or $(q+1)/4$. Combine the two independent choices of signs by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) to obtain the four roots modulo $N$ for a message coprime to $N$. Redundancy or a specified encoding distinguishes the intended message. Factoring $N$ makes decryption easy; a general square-root oracle conversely factors $N$ by obtaining two roots not congruent up to sign and taking their greatest common divisor with $N$.

For the [Repeated-message attack on the Rabin cryptosystem](../../../../../repeated-message-attack-on-the-rabin-cryptosystem.md), first compute $d=\gcd(N,N')$. If $d=1$, use the two ciphertexts to reconstruct $s\in[0,NN')$ with $s\equiv m^2\pmod N$ and $s\equiv m^2\pmod{N'}$. Since $0<m<\min(N,N')$, we have $m^2<NN'$, so this reconstruction is the ordinary integer $m^2$. Therefore

$$
\boxed{m=\sqrt{s}.}
$$

If distinct semiprime moduli have $d>1$, they share a prime; the gcd instead exposes their factors, allowing ordinary Rabin decryption with the usual encoding check. The two cases cover the stated protocol with distinct standard moduli.

In the coprime case, learning this message does not normally reveal the factors or a decryption key, so other messages encrypted only once remain protected by the square-root problem. Exceptional messages with $\gcd(m,N)>1$ do reveal a factor, and the shared-prime-modulus case compromises other messages too. Repetition under fresh coprime moduli is the vulnerability used here, rather than a universal attack on every ciphertext.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
