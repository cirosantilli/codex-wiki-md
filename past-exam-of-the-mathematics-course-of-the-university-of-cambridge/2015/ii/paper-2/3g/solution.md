<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

The [Shannon entropy](../../../../../information-entropy.md), in bits, is

$$
H(A)=-\sum_ap_a\log_2p_a=\log_2 5-\frac15\approx\boxed{2.121928}.
$$

For a prescribed alphabet distribution and code alphabet, an [optimal code](../../../../../optimal-source-code.md) is a [uniquely decodable code](../../../../../decipherable-code.md) minimizing expected codeword length. [Huffman coding](../../../../../huffman-coding.md) produces an optimal binary [prefix code](../../../../../prefix-code.md), and its minimum is also the minimum among binary [uniquely decodable codes](../../../../../decipherable-code.md).

Two optimal binary [prefix codes](../../../../../prefix-code.md), listing words in the order $a,b,c,d,e$, are

$$
(00,01,10,110,111),\qquad(0,10,110,1110,1111).
$$

Their length vectors are $(2,2,2,3,3)$ and $(1,2,3,4,4)$, and both have **expected length $2.2$ bits**. To verify optimality rather than just equal length, run [Huffman coding](../../../../../huffman-coding.md). First combine $d,e$ into a node of weight $0.2$. Among the resulting three weight-$0.2$ nodes, combining $b,c$ and then combining the remaining weight-$0.2$ node with one weight-$0.4$ node gives the first length vector. Instead combine $c$ with the $d,e$ node, then combine that weight-$0.4$ node with $b$, and finally with $a$; this gives the second. Each step combines two smallest current weights, so both constructions are [Huffman coding](../../../../../huffman-coding.md) trees. Ties therefore allow **different optimal length profiles**.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
