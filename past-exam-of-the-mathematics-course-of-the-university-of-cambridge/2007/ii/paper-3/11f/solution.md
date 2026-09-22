<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) says that for pairwise coprime positive moduli $m_i$, the map $\mathbb Z/(\prod m_i)\to\prod_i\mathbb Z/m_i$ is an isomorphism; in particular prescribed residues have a unique solution modulo the product.

Write $n=p^e m$, with $e\geq2$ and $(p,m)=1$. Choose $z\equiv1+p^{e-1}\pmod{p^e}$ and $z\equiv1\pmod m$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) supplies $z$. The binomial theorem gives $z^p\equiv1\pmod{p^e}$, since every nonconstant term is divisible by $p^e$; also $z^p\equiv1\pmod m$. Thus $z^p\equiv1\pmod n$, whereas $z\not\equiv1\pmod n$. Its multiplicative order is exactly $p$.

For odd $n=\prod p_i^{e_i}$ define the [Jacobi symbol](../../../../../jacobi-symbol.md) $(a/n)=\prod_i(a/p_i)^{e_i}$, using the [Legendre symbol](../../../../../legendre-symbol.md), with $(a/1)=1$. It is zero if $a$ shares a prime factor with $n$. For example $(2/9)=(2/3)^2=1$, but the square residues modulo nine are $0,1,4,7$, so two is not a square.

For positive odd coprime $u,v$, [Jacobi reciprocity](../../../../../jacobi-reciprocity-law.md) is

$$
\boxed{(u/v)=(-1)^{(u-1)(v-1)/4}(v/u).}
$$

Factor $u=\prod p_i^{a_i}$ and $v=\prod q_j^{b_j}$ and multiply [quadratic reciprocity](../../../../../quadratic-reciprocity.md) for each prime pair. Its sign exponent is $\sum_{i,j}a_i b_j(p_i-1)(q_j-1)/4$. For odd numbers, $(rs-1)/2\equiv(r-1)/2+(s-1)/2\pmod2$, so this exponent has the same parity as $(u-1)(v-1)/4$. Multiplicativity of the [Legendre symbol](../../../../../legendre-symbol.md) gives the two Jacobi products, proving the formula. If $u,v$ are not coprime, both sides of the displayed reciprocity equality are zero.

For the previously constructed $z$, every prime divisor of $n$ sees residue one, so $(z/n)=1$. But $p\nmid(n-1)/2$, because $p\mid n$ and $p$ is odd. The order-$p$ unit therefore has $z^{(n-1)/2}\not\equiv1\pmod n$. This supplies a unit failing the proposed test.

Finally the passing units form the [kernel](../../../../../kernel-of-a-linear-map.md) of the [homomorphism](../../../../../homomorphism.md)

$$
F:(\mathbb Z/n\mathbb Z)^\times\longrightarrow(\mathbb Z/n\mathbb Z)^\times,
\qquad F(a)=a^{(n-1)/2}(a/n)^{-1}.
$$

Multiplicativity makes this a [homomorphism](../../../../../homomorphism.md), and the failing unit shows its [kernel](../../../../../kernel-of-a-linear-map.md) is proper. A proper [subgroup](../../../../../subgroup.md) has index at least two. Hence **the test fails on at least half the units modulo $n$**.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
