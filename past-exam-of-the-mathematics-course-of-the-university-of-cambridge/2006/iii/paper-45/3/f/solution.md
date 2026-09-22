<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $D$ for the disease observations and $M$ for the [genetic marker](../../../../../../genetic-marker.md) observations. The [LOD score](../../../../../../lod-score.md) for [complete linkage](../../../../../../complete-genetic-linkage.md) is

$$
\boxed{Z(0)=\log_{10}\frac{P(M\mid D,\theta=0)}{P(M\mid D,\theta=1/2)}.}
$$

The disease marginal cancels because the single-locus disease segregation law does not depend on the [genetic marker](../../../../../../genetic-marker.md)–disease [recombination fraction](../../../../../../recombination-fraction.md). The ten [genetic markers](../../../../../../genetic-marker.md) form one nonrecombining [haplotype](../../../../../../haplotype.md); they do not supply ten independent copies of the [pedigree](../../../../../../pedigree.md)'s segregation evidence.

There is a distinction between [identity by state](../../../../../../identity-by-state.md) and [identity by descent](../../../../../../identity-by-descent.md). The reported observation that affected subjects all have $h/h$ establishes the former. An exact [genetic marker](../../../../../../genetic-marker.md) [likelihood](../../../../../../likelihood-function.md) requires [pedigree founder](../../../../../../founder-in-a-pedigree.md) [haplotype](../../../../../../haplotype.md) frequencies, or the actual [pedigree founder](../../../../../../founder-in-a-pedigree.md) [genotypes](../../../../../../genotype.md) if conditioning on them. Here is an explicit expression using independent [pedigree founder](../../../../../../founder-in-a-pedigree.md) [haplotypes](../../../../../../haplotype.md), with frequency $p$ for the observed [haplotype](../../../../../../haplotype.md) $h$, and linkage equilibrium between [pedigree founder](../../../../../../founder-in-a-pedigree.md) [genetic marker](../../../../../../genetic-marker.md) and disease states. There are eight [genetic marker](../../../../../../genetic-marker.md) copies in the four [pedigree founders](../../../../../../founder-in-a-pedigree.md): the original couple and the two generation-2 outside spouses. For [genetic marker](../../../../../../genetic-marker.md) inheritance configuration $v$, let $K(v)$ be the number of distinct [pedigree founder](../../../../../../founder-in-a-pedigree.md) copies ancestral to the sixteen chromosome copies in the eight selected subjects. Then

$$
R(p)=\sum_v P(v)p^{K(v)}=E[p^K]
$$

is the unlinked [probability](../../../../../../probability.md) that all those copies have state $h$. At [complete linkage](../../../../../../complete-genetic-linkage.md) the affected subjects all inherit the disease [pedigree founder](../../../../../../founder-in-a-pedigree.md) copy twice, and the [probability](../../../../../../probability.md) that this copy has [genetic marker](../../../../../../genetic-marker.md) state $h$ is $p$. Therefore

$$
\boxed{Z(0)=\log_{10}\frac{p}{R(p)}.}
$$

The denominator can be evaluated without an unspecified inheritance sum. Let $B_a=\binom2a p^a(1-p)^{2-a}$ for $a=0,1,2$. If parental [genetic marker](../../../../../../genetic-marker.md) [genotypes](../../../../../../genotype.md) contain $a,b$ copies of $h$, the child count distribution is

$$
Q_0(a,b)=(1-a/2)(1-b/2),\quad
Q_1(a,b)=(a/2)(1-b/2)+(1-a/2)(b/2),\quad
Q_2(a,b)=ab/4.
$$

For a generation-2 couple define

$$
F(a,b)=\prod_{r\in\{1,4,3\}}\left[\sum_{j=0}^2Q_j(a,b)(j/2)^r\right],\qquad
m_a=\sum_{b=0}^2B_bF(a,b).
$$

For a particular generation-3 parent with $j$ [genetic marker](../../../../../../genetic-marker.md) copies, the chance it transmits $h$ to all its $r$ selected offspring is $(j/2)^r$, which explains each factor. Conditional on the original founding couple, its two generation-2 siblings and their independent outside spouses give independent left and right contributions. Thus

$$
R(p)=\sum_{u,v=0}^2B_uB_v\left[\sum_{a=0}^2Q_a(u,v)m_a\right]^2.
$$

Expanding gives

$$
R(p)=\frac{p}{2^{22}}\left(1+388p+38942p^2+480421p^3+1398448p^4+1540264p^5+650576p^6+85264p^7\right).
$$

It satisfies $R(1)=1$, as it must for a monomorphic [haplotype](../../../../../../haplotype.md). This expression supplies a numerical LOD once $p$ is specified; the problem does not specify that frequency.

In the idealized limit where a matching rare [haplotype](../../../../../../haplotype.md) identifies one ancestral copy, the leading coefficient is particularly simple. Dropping restrictions on the eight unaffected subjects, the [probability](../../../../../../probability.md) that all selected subjects are [autozygous](../../../../../../autozygosity.md) for one common copy is

$$
P(H)=4\cdot\frac14\cdot\frac1{64}\cdot\left(\frac14\right)^8=2^{-22}.
$$

Accordingly $R(p)/p\to2^{-22}$ as $p\to0$, and the affected-only [IBD](../../../../../../identity-by-descent.md) calculation gives $Z(0)=22\log_{10}2\simeq6.623$.

If the [genetic marker](../../../../../../genetic-marker.md) observations additionally establish the exact pattern $E$ of part (d), including that the eight unaffected subjects are not [autozygous](../../../../../../autozygosity.md), its idealized [IBD](../../../../../../identity-by-descent.md) [likelihood ratio](../../../../../../likelihood-ratio.md) is instead

$$
Z_E(0)=-\log_{10}P(E)=38\log_{10}2-8\log_{10}3\simeq7.622.
$$

This latter value requires the additional negative [genetic marker](../../../../../../genetic-marker.md) observations. It cannot be inferred merely from [homozygosity](../../../../../../homozygosity.md) in the affected subjects, and neither simplified [IBD](../../../../../../identity-by-descent.md) score is an exact identity-by-state [likelihood](../../../../../../likelihood-function.md) for an unspecified common [haplotype](../../../../../../haplotype.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
