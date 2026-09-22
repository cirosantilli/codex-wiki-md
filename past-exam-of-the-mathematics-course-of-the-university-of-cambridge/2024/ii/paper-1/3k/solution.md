<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

Binary [Huffman coding](../../../../../huffman-coding.md) repeatedly merges the two least probable current symbols, assigns opposite bits to the two children of every merge, and reads each original symbol's codeword from the root. The resulting prefix code minimizes expected word length.

The merge weights here may be chosen as

$$
.02+.03=.05,\qquad .04+.04=.08,\qquad
.05+.08=.13,\qquad .12+.13=.25,\qquad
.25+.26=.51,\qquad .49+.51=1.
$$

One corresponding code is

$$
\begin{array}{c|ccccccc}
 &x_1&x_2&x_3&x_4&x_5&x_6&x_7\\ \hline
\text{code}&0&10&110&11110&11111&11101&11100.
\end{array}
$$

Its expected word length is

$$
\boxed{.49+2(.26)+3(.12)+5(.04+.04+.03+.02)=2.02}.
$$

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
