<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

For [Shannon-Fano coding](../../../../../shannon-fano-coding.md), order the symbols by decreasing probability and recursively split each current list into two contiguous groups with total probabilities as close as possible. Label the two branches $0$ and $1$; the path to a symbol is its [prefix code](../../../../../prefix-code.md) word. Here the first split is $\{a\}$ of weight $.4$ against $\{b,c,d\}$ of weight $.6$. The latter splits into $\{b\}$ and $\{c,d\}$, each of weight $.3$. One answer is

$$
\boxed{a:0,\qquad b:10,\qquad c:110,\qquad d:111.}
$$

For [Huffman coding](../../../../../huffman-coding.md), repeatedly merge the two least-probable nodes and then read the resulting binary tree from the root. Merge $c,d$ to weight $.3$, merge this node with $b$ to weight $.6$, and merge with $a$. The same displayed [prefix code](../../../../../prefix-code.md) results. Its mean length is $.4+2(.3)+3(.2)+3(.1)=\boxed{1.9\text{ bits per symbol}}$. Choices at ties and exchange of binary labels yield other equivalent codes. [Huffman coding](../../../../../huffman-coding.md) minimizes mean length among binary [prefix codes](../../../../../prefix-code.md); the top-down Shannon-Fano construction does not have that general optimality guarantee.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
