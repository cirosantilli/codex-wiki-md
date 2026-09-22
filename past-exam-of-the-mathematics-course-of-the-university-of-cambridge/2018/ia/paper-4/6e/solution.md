<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

The [Hamming distance](../../../../../hamming-distance.md) satisfies the triangle inequality coordinate by coordinate: if $x_i\ne z_i$, then $x_i\ne y_i$ or $y_i\ne z_i$. Summing these indicator inequalities proves the claim. A word at distance exactly $i$ from $x$ is obtained by choosing the $i$ coordinates to flip, so

$$
\boxed{|B(x,j)|=\sum_{i=0}^j\binom ni.}
$$

For a $k$-code, radius-$k$ balls about codewords are disjoint, giving $|C|\sum_{i=0}^k\binom ni\leq2^n$. Conversely, take a maximal code of minimum distance $2k+1$. Its radius-$2k$ balls cover $Q_n$, since an uncovered word could otherwise be added, so $2^n\leq|C|\sum_{i=0}^{2k}\binom ni$. Maximizing gives the requested coding bounds.

For $(n,k)=(4,1)$, translate a codeword to $0000$. Every other word has weight at least three, but any two distinct length-four words of weight at least three have distance at most two. Thus at most one can accompany $0000$, while $\{0000,1111\}$ works. Hence **$M(4,1)=2$**.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
