<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Count one transmitted/untransmitted [allele](../../../../../../allele.md) pair per observable parent. A homozygous parent contributes to $a$ or $d$; a heterozygous parent contributes to $b$ or $c$. When two heterozygotes have a heterozygous child, the parent-specific origin is ambiguous, but the combined contribution is unambiguously one to $b$ and one to $c$.

The derived contributions, ordered as $(a,b,c,d)$, are

$$
\begin{array}{c|rrrr}
\text{family}&a&b&c&d\\\hline
1&1&0&0&1\\2&0&2&0&0\\3&0&1&0&1\\4&0&1&1&0\\5&1&0&0&1\\6&0&2&0&0\\7&0&?&?&0\\8&0&0&2&0\\9&0&2&0&0\\10&0&1&0&0\\11&0&1&1&0\\12&0&1&0&1.
\end{array}
$$

In family 7, the observed father's transmission cannot be determined from the heterozygous child without the mother's genotype. In family 10, the homozygous child reveals the father's allele-1 transmission, but not the missing mother's complete transmitted/untransmitted pair.

Keeping only unambiguous observed-parent transmissions and omitting family 7 gives the raw table

$$
\boxed{(a,b,c,d)=(2,11,4,4).}
$$

This bookkeeping convention is not the same as a valid ordinary [transmission disequilibrium test](../../../../../../transmission-disequilibrium-test.md) sampling rule. [Incomplete-trio transmission-selection bias](../../../../../../incomplete-trio-transmission-selection-bias.md) arises if only homozygous children make a missing-parent family usable. The usual complete-trio analysis excludes both families 7 and 10, giving

$$
\boxed{(a,b,c,d)_{\rm complete}=(2,10,4,4).}
$$

Neither assigning family 7 a half transmission each way nor inventing its mother's genotype is justified by the supplied data. A method using all twelve families must model or validly condition on the missing information.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
