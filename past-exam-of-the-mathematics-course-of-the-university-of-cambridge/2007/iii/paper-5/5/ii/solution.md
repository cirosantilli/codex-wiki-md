<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We next bound the closed [derived series](../../../../../../derived-series.md). For odd $p$, the depth calculation yields

$$
[\mathcal N_m,\mathcal N_m]=\mathcal N_{2m+1}.
$$

For the inclusion from left to right, two series of depth at least $m$ commute modulo $\mathcal N_{2m+1}$: at depth $2m$ the only possible leading pair has equal depths and its coefficient vanishes. For the reverse inclusion, every depth $k\ge2m+1$ can be written $r+s=k$ with $r,s\ge m$ and $r\not\equiv s\pmod p$. Start with $r=m,s=k-m$; if their difference vanishes modulo $p$, replace them by $r=m+1,s=k-m-1$, which is allowed except at $k=2m+1$, where the original difference is already nonzero. The difference changes by $2$, nonzero for odd $p$. [Commutators](../../../../../../commutator.md) thus supply every high [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md), and closed successive coefficient correction fills the tail.

With $\mathcal N^{(0)}=\mathcal N_1$, induction on $n$ gives

$$
\mathcal N^{(n)}=\mathcal N_{2^{n+1}-1},\qquad\log_p[\mathcal N:\mathcal N^{(n)}]=2^{n+1}-2.
$$

For $p=2$ use the standard characteristic-two derived-series collection bound, explicitly stated as an additional result:

$$
\log_2[\mathcal N:\mathcal N^{(n)}]\le C\kappa^n,\qquad\kappa=\frac{1+\sqrt{17}}2<3,
$$

for a fixed constant $C$. One can take a fixed enlarged constant from the tail estimate $\mathcal N^{(n)}\supseteq\mathcal N_{\lceil4\kappa^n\rceil+1}$. The more involved two-coefficient collection is necessary in characteristic two; the exact odd-prime tail formula is not asserted there.

In either case there are constants $C'>0$ and $\lambda<3$ such that $\log_p[\mathcal N:\mathcal N^{(n)}]\le C'\lambda^n$. If an analytic structure existed, its [dimension](../../../../../../dimension-vector-space.md) $d$ would be positive, since a zero-dimensional analytic [pro-p group](../../../../../../pro-p-group.md) is discrete and [compact](../../../../../../compact-space.md), hence finite. The second alternative of the supplied theorem would require

$$
\log_p[\mathcal N:\mathcal N^{(n)}]\ge d\,3^{n-s}
$$

for all sufficiently large $n$, for some fixed $s$. Combining the bounds gives $d3^{-s}\le C'(\lambda/3)^n$, impossible as $n\to\infty$.

The root solution proved hereditary just infiniteness, so the supplied theorem applies. Part (i) excluded its linear alternative, and this calculation excludes its growth alternative. Hence **the [Nottingham group](../../../../../../nottingham-group.md) is not analytic over any pro-$p$ ring**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
