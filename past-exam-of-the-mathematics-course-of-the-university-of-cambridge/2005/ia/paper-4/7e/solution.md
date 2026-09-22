<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

For finite sets $A_1,\ldots,A_r$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) is

$$
\left|\bigcup_{i=1}^rA_i\right|=
\sum_{\varnothing\ne J\subseteq\{1,\ldots,r\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.
$$

To prove it, fix an element occurring in exactly $k$ of these sets. Its coefficient on the right is $\sum_{s=1}^k(-1)^{s+1}\binom ks=1$, by the [binomial theorem](../../../../../binomial-theorem.md) applied to $(1-1)^k$. An element occurring in none has coefficient zero. Summing these elementwise coefficients proves the formula.

Write the [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) $n=\prod_{i=1}^r p_i^{c_i}$ with distinct primes and positive exponents. In $\{1,\ldots,n\}$ let $A_i$ be the multiples of $p_i$. A number is coprime to $n$ exactly when it is outside their union. For a nonempty index set $J$, the intersection has $n/\prod_{j\in J}p_j$ elements, since that product divides $n$. Applying [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) to the complement therefore gives

$$
\begin{aligned}
\varphi(n)&=n\sum_{J\subseteq\{1,\ldots,r\}}\frac{(-1)^{|J|}}{\prod_{j\in J}p_j}
=n\prod_{i=1}^r\left(1-\frac1{p_i}\right),\\
\varphi(n)&=\prod_{i=1}^r p_i^{c_i-1}(p_i-1).
\end{aligned}
$$

For $n=1$, the empty product gives $\varphi(1)=1$. If positive integers $a,b$ are coprime, their prime factors are disjoint, so the product separates and proves the [multiplicativity of the Euler totient function](../../../../../multiplicativity-of-the-euler-totient-function.md):

$$
\boxed{\varphi(ab)=\varphi(a)\varphi(b).}
$$

For a positive divisor $d\mid n$, write the exponent of a prime in $d$ as $b_i\le c_i$, allowing $b_i=0$. Its contribution to $\varphi(n)/\varphi(d)$ is $p_i^{c_i-b_i}$ if $b_i>0$, and $p_i^{c_i-1}(p_i-1)$ if $b_i=0$. Every contribution is an integer; multiplying proves [totient divisibility along divisors](../../../../../totient-divisibility-along-divisors.md):

$$
\boxed{\varphi(d)\mid\varphi(n).}
$$

Finally suppose $\varphi(n)\mid n$. If $n=1$ the required form is immediate. If $n>1$ were odd, some odd prime $p$ would divide it, and the even factor $p-1$ in $\varphi(n)$ would make an even number divide an odd number, impossible. Thus write $n=2^c\prod_{j=1}^s p_j^{a_j}$ with odd primes and $c\ge1$. Counting powers of two in the totient formula gives

$$
c-1+\sum_{j=1}^s v_2(p_j-1)\le c,
$$

where $v_2$ is the $2$-adic [P-adic valuation](../../../../../p-adic-valuation.md). Every term in the sum is at least one, so there is at most one odd prime $p$ and, if present, $v_2(p-1)=1$. Moreover $p-1\mid\varphi(n)\mid n$. Since $p-1$ is coprime to $p$, and $n$ has no prime factors other than $2,p$, the integer $p-1$ must be a power of two. Its exponent is one, hence $p-1=2$ and $p=3$. This proves

$$
\boxed{n=2^c3^d\quad\text{for some }c,d\ge0.}
$$

More precisely, the [integers whose totient divides them](../../../../../integers-whose-totient-divides-them.md) are $n=1$ and $2^c3^d$ with $c\ge1$, $d\ge0$; substitution in the product formula proves the converse. A positive power of $3$ alone does not satisfy the divisibility condition.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
