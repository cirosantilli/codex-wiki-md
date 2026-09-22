<h1 id="4/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We first give the common reduction for the three conditions, then prove the cycle from (i) to (ii), from (ii) to (iii), and from (iii) back to (i). Assume here that $\operatorname{char}K\ne p$. The [Galois module of roots of unity](../../../../../../../galois-module-of-roots-of-unity.md) $\mu_p$ fits into the Kummer sequence

$$
1\longrightarrow\mu_p\longrightarrow K_s^\times\xrightarrow{\ p\ }K_s^\times\longrightarrow1,
$$

which is surjective on the right because $p$th-root polynomials are separable. Restrict it to the [absolute Galois group](../../../../../../../absolute-galois-group.md) of any algebraic extension $L/K$. The long exact sequence gives the [Kummer cohomology divisibility criterion](../../../../../../../kummer-cohomology-divisibility-criterion.md)

$$
0\longrightarrow H^n(L,K_s^\times)/pH^n(L,K_s^\times)
\longrightarrow H^{n+1}(L,\mu_p)
\longrightarrow H^{n+1}(L,K_s^\times)[p]\longrightarrow0.
$$

[Continuous cohomology of a profinite group](../../../../../../../continuous-cohomology-of-a-profinite-group.md) in positive degree with discrete coefficients is torsion: a continuous normalized cocycle becomes zero on a sufficiently small open subgroup, and restriction followed by corestriction multiplies its class by the finite index. For an abelian group, [p-primary torsion](../../../../../../../primary-torsion-subgroup-at-a-prime.md) consists of elements killed by powers of $p$, while [p-divisibility](../../../../../../../divisibility-by-a-prime.md) means that multiplication by $p$ is surjective. For a torsion group $A$, $A\{p\}=0$ if and only if $A[p]=0$, because a nonzero element of $p$-power order has a multiple of exact order $p$. Consequently the two conditions on the multiplicative cohomology groups are jointly equivalent to

$$
\boxed{H^{n+1}(L,\mu_p)=0}.
$$

The coefficient module $K_s^\times$ is used with its restricted Galois action as in the question. Purely inseparable algebraic extensions give equivalent [absolute Galois groups](../../../../../../../absolute-galois-group.md); the $\mu_p$ reduction therefore also covers those extensions.

The [cohomological dimension at a prime](../../../../../../../cohomological-dimension-at-a-prime.md) condition $\operatorname{cd}_p(K)\le n$ means that $H^q(G_K,M)=0$ for every discrete $p$-primary torsion [Galois module](../../../../../../../galois-module.md) $M$ and every $q>n$. Cohomological dimension does not increase on a closed subgroup. Since [absolute Galois groups](../../../../../../../absolute-galois-group.md) of algebraic extensions identify with closed subgroups, up to the purely inseparable identification just noted, condition (i) gives $H^{n+1}(L,\mu_p)=0$ for every algebraic $L/K$. The Kummer reduction proves **(i) implies (ii)**.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [2](../../2.md)
3. [4](../../../4.md)
4. [Paper 21](../../../../paper-21-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
