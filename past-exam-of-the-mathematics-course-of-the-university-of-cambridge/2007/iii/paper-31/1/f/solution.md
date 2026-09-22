<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the uniform 27-symbol model, $s=\lceil\log_2 27\rceil=5$. The [uniform-source Huffman length distribution](../../../../../../uniform-source-huffman-length-distribution.md) gives

$$
\boxed{n_4=32-27=5,\qquad n_5=54-32=22.}
$$

Thus five symbols receive four-bit [codewords](../../../../../../codeword.md) and the other 22 receive five-bit [codewords](../../../../../../codeword.md). To realize these lengths, start with all 32 binary words of length five and collapse any five disjoint sibling pairs into their four-bit parents. This leaves exactly five leaves at depth four and 22 at depth five. All source letters have the same probability, so which five letters receive the shorter [codewords](../../../../../../codeword.md) is arbitrary.

The [expected codeword length](../../../../../../expected-codeword-length.md) is

$$
\boxed{L=\frac{5\cdot4+22\cdot5}{27}=\frac{130}{27}\approx4.815\text{ bits per symbol}.}
$$

The 27 symbols may represent 26 letters and a space, but this idealization keeps them equiprobable; it is not an empirical frequency model of English.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
