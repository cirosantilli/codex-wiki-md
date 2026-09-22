<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

[Shannon-Fano coding](../../../../../shannon-fano-coding.md) orders symbols by decreasing [probability](../../../../../probability.md) and recursively splits each consecutive block into two groups with [probability](../../../../../probability.md) totals as close as possible, appending bits zero and one. [Huffman coding](../../../../../huffman-coding.md) instead repeatedly merges the two least probable nodes, constructs a binary tree upwards, and then assigns the branch bits. Both yield [prefix codes](../../../../../prefix-code.md), so a concatenation can be decoded without separators; [Huffman coding](../../../../../huffman-coding.md) minimizes expected length among binary [prefix codes](../../../../../prefix-code.md).

For the specified [probabilities](../../../../../probability.md), the first [Shannon-Fano coding](../../../../../shannon-fano-coding.md) split is $\{\mu_1\}$ of [mass](../../../../../mass.md) $0.45$ versus the remaining [mass](../../../../../mass.md) $0.55$. Split the latter into $\{\mu_2\}$ of [mass](../../../../../mass.md) $0.25$ and $\{\mu_3,\mu_4,\mu_5\}$ of [mass](../../../../../mass.md) $0.30$, and then split off $\mu_3$. One resulting code is

$$
\boxed{\mu_1:0,\quad\mu_2:10,\quad\mu_3:110,\quad\mu_4:1110,\quad\mu_5:1111.}
$$

Its expected word length is $0.45+2(0.25)+3(0.20)+4(0.05+0.05)=\boxed{1.95\text{ bits}}$.

The [Huffman coding](../../../../../huffman-coding.md) merges are $0.05+0.05=0.10$, $0.10+0.20=0.30$, $0.25+0.30=0.55$, and $0.45+0.55=1$. Reading the resulting tree gives the same code lengths $1,2,3,4,4$, and it may give exactly the displayed code if the branch bits are chosen accordingly. Its expected length is also **$1.95$ bits**. The methods agree here; their agreement on this particular distribution is not a claim that the two procedures always coincide.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
