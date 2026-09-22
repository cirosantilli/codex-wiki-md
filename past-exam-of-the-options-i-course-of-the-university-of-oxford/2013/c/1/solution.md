<h1 id="c/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Euler's totient function](../../../../euler-totient-function.md) is

$$
\varphi(n)=\#\{1\leq r\leq n:\gcd(r,n)=1\},\qquad n\geq1.
$$

[Euler's theorem](../../../../euler-s-theorem.md) states that $\gcd(a,n)=1$ implies $\boxed{a^{\varphi(n)}\equiv1\pmod n}$. For $n>1$, let $r_1,\ldots,r_{\varphi(n)}$ be the invertible residue classes modulo $n$. Multiplication by $a$ permutes these classes, since it has an inverse modulo $n$. Multiplying the resulting congruences gives

$$
a^{\varphi(n)}r_1\cdots r_{\varphi(n)}\equiv r_1\cdots r_{\varphi(n)}\pmod n.
$$

Every factor is a [unit](../../../../unit-in-a-ring.md), so the product can be cancelled, proving the theorem. The case $n=1$ is immediate. For distinct [prime numbers](../../../../prime-number-split.md) $p,q$, removing multiples of either prime from $1,\ldots,pq$ gives

$$
\boxed{\varphi(pq)=pq-q-p+1=(p-1)(q-1).}
$$

For the [RSA cryptosystem](../../../../rsa-cryptosystem.md), choose distinct large primes $p,q$, put $N=pq$, and choose $e$ coprime to $\varphi(N)$. Compute $d$ with $ed\equiv1\pmod{\varphi(N)}$. The public key is $(N,e)$; the private exponent $d$ is retained secretly. Represent a message by $0\leq m<N$, encrypt by $c\equiv m^e\pmod N$, and decrypt by $m'\equiv c^d\pmod N$.

To prove correct decryption even for messages not coprime to $N$, write $ed=1+k(p-1)(q-1)$. Modulo $p$, if $p\mid m$ then $m^{ed}\equiv m\equiv0$; otherwise [Fermat's little theorem](../../../../fermat-little-theorem.md) gives $m^{ed}\equiv m$. The same reasoning holds modulo $q$. The [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) therefore gives $m^{ed}\equiv m\pmod N$, and the chosen representative recovers $m$. Thus **decryption works for every message residue**, not merely the units.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [C](../../c.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
