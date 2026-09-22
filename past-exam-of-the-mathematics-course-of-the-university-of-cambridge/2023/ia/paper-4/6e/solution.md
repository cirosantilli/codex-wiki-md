<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

For prime $p$, the nonzero residues pair with their distinct inverses except for $1$ and $-1$, so [Wilson theorem](../../../../../wilson-s-theorem.md) gives

$$
(p-1)!\equiv-1\pmod p.
$$

If composite $n>4$ has a factorization $n=ab$ with $1<a<b<n$, both factors occur in $(n-1)!$. If $n=m^2$, the distinct factors $m$ and $2m$ occur and their product is divisible by $n$; the excluded case $m=2$ is exactly $n=4$. Thus $(n-1)!\equiv0\pmod n$.

The [Fermat-Euler theorem](../../../../../euler-s-theorem.md) states $a^{\phi(n)}\equiv1\pmod n$ when $(a,n)=1$. For prime $p$, $\phi(p)=p-1$, giving Fermat's little theorem for $p\nmid a$; the form $a^p\equiv a\pmod p$ also covers $p\mid a$.

If $a\equiv b\pmod p$, induction and the binomial theorem show

$$
a^{p^n}\equiv b^{p^n}\pmod{p^{n+1}}.
$$

Indeed, write $a^{p^n}=b^{p^n}+cp^{n+1}$ and raise to the $p$th power; every nonleading binomial term gains enough powers of $p$.

Fix $a>1$ and choose any odd prime $p\nmid a^2-1$. Put

$$
N_p=\frac{a^{2p}-1}{a^2-1}=1+a^2+\cdots+a^{2(p-1)}.
$$

Fermat's theorem gives $N_p\equiv1\pmod p$, and $N_p$ is odd, so $2p\mid N_p-1$. Also $a^{2p}\equiv1\pmod{N_p}$, hence $a^{N_p-1}\equiv1\pmod{N_p}$. For odd $p$,

$$
N_p=\frac{a^p-1}{a-1}\frac{a^p+1}{a+1}
$$

is composite. This [generalized repunit pseudoprime construction](../../../../../generalized-repunit-pseudoprime-construction.md) gives infinitely many distinct base-$a$ pseudoprimes because the values are unbounded.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
