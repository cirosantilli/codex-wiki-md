<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [coprime integers](../../../../../../coprime-integers.md) $\alpha,N$, the [multiplicative order](../../../../../../multiplicative-order.md) is the smallest positive exponent

$$
\boxed{r=\operatorname{ord}_N(\alpha)=\min\{k\geq1:\alpha^k\equiv1\pmod N\}.}
$$

It exists because multiplication by $\alpha$ is an element of the finite [group of units modulo an integer](../../../../../../multiplicative-group-of-integers-modulo-n.md). For the example, the successive residues are

$$
7^1\equiv7,\quad7^2\equiv4,\quad7^3\equiv13,\quad7^4\equiv1\pmod{15}.
$$

None of the first three is one, so **the order is four**.

The [factor extraction from an even modular order](../../../../../../factor-extraction-from-an-even-modular-order.md) uses the factorization $\alpha^r-1=(\alpha^{r/2}-1)(\alpha^{r/2}+1)$. If the [multiplicative order](../../../../../../multiplicative-order.md) $r$ is even, put $z=\alpha^{r/2}\bmod N$. Minimality of the [multiplicative order](../../../../../../multiplicative-order.md) excludes $z=1$; we also require $z\neq-1\pmod N$. Thus $z^2\equiv1\pmod N$ is a nontrivial square root of one. Neither $z-1$ nor $z+1$ is divisible by all of $N$. If either were coprime to $N$, its inverse modulo $N$, applied to $(z-1)(z+1)\equiv0$, would make the other divisible by $N$, a contradiction. Hence the [greatest common divisors](../../../../../../greatest-common-divisor.md)

$$
\boxed{d_-=\gcd(z-1,N),\qquad d_+=\gcd(z+1,N)}
$$

are proper nontrivial factors. For odd $N$, $(z-1)$ and $(z+1)$ have no common prime divisor of $N$, so these two divisors are complementary. If the initial $\alpha$ is not coprime to $N$, a proper $\gcd(\alpha,N)$ already supplies a factor without [quantum order finding](../../../../../../quantum-order-finding.md).

For $N=15$ and $\alpha=7$, $r=4$ and $z=7^2\bmod15=4$, which is neither $1$ nor $14$. **The factors are**

$$
\boxed{\gcd(4-1,15)=3,\qquad\gcd(4+1,15)=5.}
$$

The necessary conditions for this order-based reduction are a unit $\alpha\bmod N$, even true [multiplicative order](../../../../../../multiplicative-order.md), and $\alpha^{r/2}\not\equiv-1\pmod N$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
