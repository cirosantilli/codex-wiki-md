<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat each row as a set $A_i$ of attributes with response one. The binary option computes the [Jaccard distance](../../../../../../jaccard-distance.md), rather than counting matches at joint absences. For a pair of rows, let $a$ count coordinates equal to one in both, $b$ count $(1,0)$, $c$ count $(0,1)$, and $d$ count $(0,0)$. Then

$$
\boxed{d_{ij}=1-\frac{a}{a+b+c}=\frac{b+c}{a+b+c}.}
$$

The denominator counts coordinates present in at least one row; joint absences do not contribute. If both rows have no presences, use distance zero. This differs from [normalized Hamming distance](../../../../../../normalized-hamming-distance.md), which would divide $b+c$ by all ten coordinates.

For Philip and Chad, four attributes are present in both and eight in at least one, giving [Jaccard distance](../../../../../../jaccard-distance.md) $4/8=0.50$. Graham and Tim differ in one of eight coordinates present in their union, giving $1/8=0.125$, printed as $0.12$. Fred and Gbenga have identical profiles, hence distance zero despite being different students. The resulting [dissimilarity matrix](../../../../../../dissimilarity-matrix.md) is symmetric with zero diagonal; `dist2full` restores the other half and the diagonal from the stored pairwise entries. The display rounds entries for readability; the [agglomerative hierarchical clustering](../../../../../../agglomerative-hierarchical-clustering.md) uses the original unrounded distances.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
