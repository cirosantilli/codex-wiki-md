<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

In the [RSA cryptosystem](../../../../../rsa-cryptosystem.md), choose distinct primes $p,q$, set $N=pq$, and choose $e$ with $\gcd(e,\phi(N))=1$. The public key is $(N,e)$; the private exponent satisfies

$$
ed\equiv1\pmod{\phi(N)}.
$$

A message $m$ is encrypted and decrypted by

$$
c\equiv m^e\pmod N,
\qquad
m\equiv c^d\pmod N.
$$

Suppose $\phi(N)\mid2^ab$, where $b$ is odd. For a unit $x$ modulo $N$, both $O_p(x^b)$ and $O_q(x^b)$ are powers of two dividing $2^a$. If these orders differ, assume without loss of generality that

$$
O_p(x^b)=2^r<2^s=O_q(x^b).
$$

Taking $t=r<a$ gives

$$
x^{2^tb}\equiv1\pmod p,
\qquad
x^{2^tb}\not\equiv1\pmod q,
$$

and hence

$$
\boxed{\gcd(x^{2^tb}-1,N)=p,}
$$

a nontrivial factor.

To count successful $x$, write $p-1=2^ru$ and $q-1=2^sv$ with $u,v$ odd. Raising to the odd power $b$, which is divisible by the odd parts, maps a uniformly chosen element of each cyclic multiplicative group uniformly onto its Sylow two-subgroup. In a cyclic group of order $2^r$, the probability of order $1$ is $2^{-r}$ and that of order $2^j$ is $2^{j-1-r}$ for $1\leq j\leq r$. If $r\leq s$, the probability that the two resulting orders agree is

$$
\frac{1+\sum_{j=1}^r4^{j-1}}{2^{r+s}}
=\frac{4^r+2}{3\cdot2^{r+s}}
\leq\frac12.
$$

Thus at least half of the $\phi(N)$ units satisfy $O_p(x^b)\ne O_q(x^b)$.

Knowing $d$ reveals the multiple $ed-1$ of $\phi(N)$. Writing $ed-1=2^ab$ with $b$ odd and trying random units therefore yields a factor with probability at least one half per trial; nonunits already reveal a factor by taking their greatest common divisor with $N$. Conversely, factoring $N$ gives $\phi(N)$ and hence $d=e^{-1}\pmod{\phi(N)}$. This proves that recovering the private key is computationally equivalent, up to randomized polynomial-time work, to factoring the RSA modulus, as summarized by [RSA private exponent reveals the factorization](../../../../../rsa-private-exponent-reveals-the-factorization.md).

For $N=77$ and $e=43$, $\phi(N)=60$ and

$$
d\equiv43^{-1}\equiv7\pmod{60}.
$$

Therefore

$$
\boxed{m\equiv5^7\equiv47\pmod{77}.}
$$

Finally, $e$ is odd because it is coprime to the even integer $\phi(N)$. If $m^e\equiv m\pmod N$, then

$$
(N-m)^e\equiv(-m)^e\equiv-m^e\equiv-m\equiv N-m\pmod N.
$$

Thus **fixed points occur in complementary pairs $m,N-m$**, which is the [Complementary RSA fixed points](../../../../../complementary-rsa-fixed-points.md) property.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
