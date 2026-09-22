<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The standard primitive-character [multiplicative large sieve inequality](../../../../../../character-large-sieve.md) is

$$
\sum_{q\le Q}\frac q{\varphi(q)}\sum_{\chi\bmod q}^{*}
\left|\sum_{M<n\le M+N}a_n\chi(n)\right|^2
\le C(N+Q^2)\sum_n|a_n|^2,
$$

where the star restricts to [primitive Dirichlet characters](../../../../../../primitive-dirichlet-character.md). This is the form used in analytic arguments for [Linnik's theorem](../../../../../../linnik-s-theorem.md). The prime-power Gauss identities extend to arbitrary primitive conductors by the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md). Thus the [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md) sum is, up to a factor of modulus $q^{-1/2}$, the character-weighted sum of the additive values $A(a/q)=\sum_na_ne(an/q)$ over units $a$. [Orthogonality of Dirichlet characters](../../../../../../orthogonality-of-dirichlet-characters.md), extending the primitive-character summation to all characters, gives

$$
\frac q{\varphi(q)}\sum_{\chi\bmod q}^{*}|\sum_na_n\chi(n)|^2
\le\sum_{(a,q)=1}|A(a/q)|^2.
$$

The additive sieve on the $Q^{-2}$-spaced Farey points proves the displayed bound.

For both prime-interval applications, use the following [large sieve upper bound for sifted intervals](../../../../../../large-sieve-upper-bound-for-sifted-intervals.md). Suppose $S$ is in an interval of length $H$ and avoids one residue modulo every [prime](../../../../../../prime-number.md) $p\le Q$ not dividing a fixed $q$. Then

$$
|S|\le\frac{C(H+Q^2)}{\mathcal L_q(Q)},\qquad
\mathcal L_q(Q)=\sum_{\substack{d\le Q\\(d,q)=1}}\frac{\mu^2(d)}{\varphi(d)}.
$$

To prove it, choose the forbidden [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) residue $r_d$ for each [squarefree](../../../../../../squarefree-integer.md) $d$. The [Ramanujan sum](../../../../../../ramanujan-sum.md) $c_d(n-r_d)$ equals $\mu(d)$ on $S$, since $n-r_d$ is a unit modulo $d$. Therefore [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_{(a,d)=1}\left|\sum_{n\in S}e(an/d)\right|^2\ge\frac{|S|^2}{\varphi(d)}.
$$

Indeed the linear combination with coefficients $e(-ar_d/d)$ has value $\mu(d)|S|$, and these coefficients have squared norm $\varphi(d)$. Sum over the allowed [squarefree](../../../../../../squarefree-integer.md) $d$, apply the additive large sieve, and cancel $|S|$; the empty set is immediate.

Finally $\mathcal L_1(Q)\ge c\log(2Q)$. [Squarefree integers](../../../../../../squarefree-integer.md) have a positive elementary lower density: the nonsquarefree [integers](../../../../../../integer.md) up to $X$ are covered by multiples of $k^2$, and $\sum_{k\ge2}k^{-2}\le3/4$. [Partial summation](../../../../../../abel-s-summation-formula.md) turns this density into the [harmonic](../../../../../../harmonic-function.md) lower bound. Splitting each [squarefree](../../../../../../squarefree-integer.md) $d$ into its factors supported on [primes](../../../../../../prime-number.md) dividing $q$ and its coprime part gives

$$
\mathcal L_1(Q)\le\prod_{p\mid q}\left(1+\frac1{p-1}\right)\mathcal L_q(Q)
=\frac q{\varphi(q)}\mathcal L_q(Q).
$$

Consequently $\mathcal L_q(Q)\ge c\,\varphi(q)\log(2Q)/q$, uniformly in $q$ and $Q$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
