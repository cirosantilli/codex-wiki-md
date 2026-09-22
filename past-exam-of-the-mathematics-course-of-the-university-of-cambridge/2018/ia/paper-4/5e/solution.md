<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

[Bezout identity](../../../../../bezout-identity.md) gives integers $b,c$ with $ab+nc=1$ whenever $\gcd(a,n)=1$, so $ab\equiv1\pmod n$. If $b,b'$ are inverses, multiplying $a(b-b')\equiv0$ by an inverse gives $b\equiv b'\pmod n$. Multiplying Bezout identities for $a$ and $b$ shows that $\gcd(ab,n)=1$.

[Wilson theorem](../../../../../wilson-s-theorem.md) states that $(p-1)!\equiv-1\pmod p$ for prime $p$. Pair the nonzero residues with their unique multiplicative inverses. The only self-inverse residues are $1,-1$, whose product is $-1$, proving the theorem.

Counting one factor of $p$ for every multiple of $p$, another for every multiple of $p^2$, and so on proves [Legendre formula](../../../../../legendre-s-formula.md)

$$
\boxed{v_p(n!)=\sum_{i\geq1}\left\lfloor\frac n{p^i}\right\rfloor.}
$$

Now $22!\equiv20!\cdot21\cdot22\equiv2(20!)\equiv-1\pmod{23}$, so **$20!\equiv11\pmod{23}$**. Also $v_5(1000!)=200+40+8+1=249$, while $v_2(1000!)>249$, so **$1000!\equiv0\pmod{10^{249}}$**.

Finally,

$$
\binom{p^m}{k}=\frac{p^m}{k}\binom{p^m-1}{k-1}.
$$

For $1\leq j<p^m$, $v_p(p^m-j)=v_p(j)$, so the second factor is a $p$-adic unit. If $v_p(k)=\ell$, then

$$
\boxed{v_p\binom{p^m}{k}=m-\ell.}
$$

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
