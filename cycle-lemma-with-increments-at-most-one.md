# Cycle lemma with increments at most one

↑ **Parent:** [Cycle lemma](cycle-lemma.md)

A standard positive-total form of the [Dvoretzky-Motzkin cycle lemma](cycle-lemma.md) uses a nonempty [sequence](sequence.md) $a=(a_1,\ldots,a_n)$ of [integers](integer-split.md) satisfying

$$
a_i\leq1\quad(1\leq i\leq n),\qquad \sum_{i=1}^{n}a_i=k>0.
$$

Exactly $k$ starting positions have every nonempty [partial sum](partial-sum.md) strictly positive, using the same rotation convention as the sum-one [cycle lemma](cycle-lemma.md). Negative entries can be arbitrarily large in magnitude, and zero entries are allowed. Addario-Berry's proposition 2.2.1 gives an equivalent form with increments at least $-1$ and negative total; reversing the [sequence](sequence.md) and changing all signs gives the form here. [Addario-Berry, Lecture notes: 2021 CRM-PIMS Probability Summer School, proposition 2.2.1, p. 39](https://problab.ca/louigi/notes/ssprob2021.pdf#page=39)

**Four starts, two successes.** For $a=(1,1,1,-1)$, the [sum](sum.md) is $k=2$. Starts $0$ and $1$ give [partial sums](partial-sum.md) $(1,2,3,2)$ and $(1,2,1,2)$, respectively. Start $2$ gives $(1,0,1,2)$ and touches zero; start $3$ gives $(-1,0,1,2)$ and begins below zero. Thus exactly two starts are good. The rotated [sequence](sequence.md) $(-1,1,1,1)$ has the same positive total, but its first start is bad: a positive final lead alone does not control earlier [partial sums](partial-sum.md).

<a id="image-all-four-starts-of-1-1-1-1-the-cycle-lemma-with-increments-at-most-one-counts-precisely-the-two-paths-whose-nonempty-partial-sums-stay-strictly-above-zero"></a>
![](cycle-lemma-good-rotations.png)

**[Figure 5](#image-all-four-starts-of-1-1-1-1-the-cycle-lemma-with-increments-at-most-one-counts-precisely-the-two-paths-whose-nonempty-partial-sums-stay-strictly-above-zero). All four starts of $(1,1,1,-1)$: the cycle lemma with increments at most one counts precisely the two paths whose nonempty partial sums stay strictly above zero**.

**Positions can give identical words.** The [sequence](sequence.md) $(1,1,-1,1,1,-1)$ repeats a block of length three and has [sum](sum.md) two. Its good starts are $0$ and $3$, both giving the same [word](string.md) $(1,1,-1,1,1,-1)$ with [partial sums](partial-sum.md) $(1,2,1,2,3,2)$. Starts $1$ and $4$ touch zero; starts $2$ and $5$ begin negatively. The [cycle lemma with increments at most one](cycle-lemma-with-increments-at-most-one.md) counts two starting positions even though there is only one distinct good rotated [word](string.md). Counting distinct [words](string.md) would lose the multiplicity that makes the statement true.

<a id="image-six-starting-positions-of-the-repeating-sequence-1-1-1-1-1-1-starts-0-and-3-produce-identical-good-words-and-count-twice"></a>
![](cycle-lemma-periodic-start-positions.png)

**[Figure 6](#image-six-starting-positions-of-the-repeating-sequence-1-1-1-1-1-1-starts-0-and-3-produce-identical-good-words-and-count-twice). Six starting positions of the repeating sequence $(1,1,-1,1,1,-1)$: starts $0$ and $3$ produce identical good words and count twice**.

**The upper bound matters.** The one-entry [sequence](sequence.md) $(2)$ has positive [integer](integer-split.md) [sum](sum.md) two, but only one starting position. Thus the sum-$k$ conclusion fails for arbitrary positive increments when $k>1$. The sum-one [cycle lemma](cycle-lemma.md) above needs no such upper bound. Strict positivity also matters: counting paths that merely stay at or above zero would include additional starts in both diagrams.

**From rotation to enumeration.** For a fixed admissible [sequence](sequence.md), a start chosen from a [uniform distribution on a finite set](discrete-uniform-distribution.md) of its $n$ positions is good with [probability](probability.md) $k/n$. More generally, let $\mathcal F$ be any [finite set](finite-set.md) of length-$n$ [sequences](sequence.md) satisfying the increment bound and total $k$, closed under rotation. [Double counting](double-counting-proof-technique.md) pairs consisting of a [sequence](sequence.md) and a good starting position gives

$$
\#\{a\in\mathcal F:\text{all nonempty partial sums of }a\text{ are positive}\}
=\frac{k}{n}|\mathcal F|.
$$

For each good output [sequence](sequence.md) and each of the $n$ positions, inverse rotation gives one such pair, even when several rotated [words](string.md) coincide. For example, the four [sequences](sequence.md) containing three $+1$ votes and one $-1$ vote have exactly $\frac24\binom43=2$ vote orders with a strictly positive running lead: $(1,1,1,-1)$ and $(1,1,-1,1)$. This is how the [cycle lemma with increments at most one](cycle-lemma-with-increments-at-most-one.md) converts many prefix inequalities into a simple counting factor.

## ↑ Ancestors (5)

1. [Cycle lemma](cycle-lemma.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cycle lemma with increments at most one](cycle-lemma-with-increments-at-most-one.md)
