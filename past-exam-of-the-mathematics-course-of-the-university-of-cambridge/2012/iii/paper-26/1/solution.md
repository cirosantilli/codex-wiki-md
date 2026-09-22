<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $C=\bigcup_{r\geq1}\mathbb Q(\mu_{p^r})$, where $\mu_{p^r}$ is the group of $p^r$th [roots of unity](../../../../../root-of-unity.md). The compatible [Galois groups](../../../../../galois-group.md) of the [cyclotomic fields](../../../../../cyclotomic-field.md) give

$$
\operatorname{Gal}(C/\mathbb Q)
\cong\varprojlim_r(\mathbb Z/p^r\mathbb Z)^\times
=\mathbb Z_p^\times.
$$

For odd $p$, the [Teichmüller character](../../../../../teichmuller-character.md) gives

$$
\mathbb Z_p^\times=\mu_{p-1}\times(1+p\mathbb Z_p).
$$

The [p-adic logarithm](../../../../../p-adic-logarithm.md) identifies $1+p\mathbb Z_p$ with $p\mathbb Z_p$, which is topologically isomorphic to $\mathbb Z_p$. More explicitly, $a\mapsto(1+p)^a$ is an [isomorphism](../../../../../isomorphism.md) from the additive [p-adic integers](../../../../../p-adic-integer.md) onto $1+p\mathbb Z_p$: the logarithm of $1+p$ has [valuation](../../../../../valuation.md) one and generates $p\mathbb Z_p$. Take the fixed field of $\mu_{p-1}$ in $C$.

For $p=2$, use instead

$$
\mathbb Z_2^\times=\{\pm1\}\times(1+4\mathbb Z_2).
$$

The [p-adic logarithm](../../../../../p-adic-logarithm.md) identifies the second factor with $4\mathbb Z_2$, and $a\mapsto5^a$ identifies it with $\mathbb Z_2$. The fixed field of $\{\pm1\}$ in $C$ is the union of the maximal real subfields of the [cyclotomic fields](../../../../../cyclotomic-field.md) of $2$-power conductor. Thus in both cases the **cyclotomic Zp-extension** exists:

$$
\boxed{\mathbb Q[p^\infty]=C^{\Delta_p},\qquad
\operatorname{Gal}(\mathbb Q[p^\infty]/\mathbb Q)\cong\mathbb Z_p,}
$$

where $\Delta_p=\mu_{p-1}$ for odd $p$ and $\Delta_2=\{\pm1\}$.

The closed subgroup $p^n\mathbb Z_p$ is the unique subgroup of index $p^n$, so the [Galois correspondence](../../../../../galois-correspondence.md) supplies the unique degree-$p^n$ field $\mathbb Q[p^n]$. In the odd case it is the $\Delta_p$-fixed field in $\mathbb Q(\mu_{p^{n+1}})$; in the even case it is the real subfield of $\mathbb Q(\mu_{2^{n+2}})$. These finite layers are all [totally real number fields](../../../../../totally-real-number-field.md).

Now set $A=\mathbb Q[p^n]$, $B=\mathbb Q[p^m]$, and let $H_A$ be the ordinary [Hilbert class field](../../../../../hilbert-class-field.md) of $A$. Thus $H_A/A$ is abelian, unramified at finite primes, and split at every real place, with degree $h(A)$. If $m=n$ there is nothing to prove. Otherwise the unique prime over $p$ is totally ramified in $B/A$, by the permitted total-ramification fact and multiplicativity of the [ramification index](../../../../../ramification-index.md). Any nontrivial intermediate field of $B/A$ is ramified at that prime. Hence

$$
H_A\cap B=A.
$$

It follows that the two extensions are [linearly disjoint field extensions](../../../../../linear-disjointness.md), and

$$
[BH_A:B]=[H_A:A]=h(A).
$$

Unramified extensions remain unramified after base change. The real places also remain split: $H_A$ and $B$ are totally real, so their compositum is totally real. Therefore $BH_A/B$ lies inside the ordinary [Hilbert class field](../../../../../hilbert-class-field.md) $H_B/B$. Its degree divides $[H_B:B]=h(B)$, proving

$$
\boxed{h(p^n)\mid h(p^m).}
$$

This is [class number divisibility with split real places](../../../../../class-number-divisibility-with-split-real-places.md); using a class-field statement restricted to imaginary fields would unnecessarily omit the present real layers.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
