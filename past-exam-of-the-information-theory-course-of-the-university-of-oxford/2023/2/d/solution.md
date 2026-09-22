<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First, the binary translation of a quaternary [prefix code](../../../../prefix-code.md) is still a [prefix code](../../../../prefix-code.md): every translated [codeword length](../../../../codeword-length.md) is even, and a binary prefix relation would split into complete two-[bit](../../../../bit.md) blocks, giving a prefix relation between the original quaternary [codewords](../../../../codeword.md). Binary [Huffman coding](../../../../huffman-coding.md) is optimal among binary [prefix codes](../../../../prefix-code.md), so

$$
\mathbb E|c_B(X_1)|\leq\mathbb E|c_{QB}(X_1)|.
$$

For the other direction, let $\ell_i=|c_B(x_i)|$ and round these binary [codeword lengths](../../../../codeword-length.md) to quaternary lengths $k_i=\lceil\ell_i/2\rceil$. The [Kraft inequality](../../../../kraft-mcmillan-inequality.md) gives

$$
\sum_i4^{-k_i}=\sum_i2^{-2\lceil\ell_i/2\rceil}
\leq\sum_i2^{-\ell_i}\leq1.
$$

The quaternary converse of the [Kraft inequality](../../../../kraft-mcmillan-inequality.md) supplies a quaternary [prefix code](../../../../prefix-code.md) with lengths $k_i$. Optimality of the [quaternary Huffman code](../../../../quaternary-huffman-coding.md) then implies

$$
\begin{aligned}
\mathbb E|c_{QB}(X_1)|
&=2\mathbb E|c_Q(X_1)|
\leq2\sum_i p_i\left\lceil\frac{\ell_i}2\right\rceil\\
&\leq\sum_i p_i(\ell_i+1)
=\mathbb E|c_B(X_1)|+1.
\end{aligned}
$$

Thus **binary translation of an optimal quaternary code costs at most one extra bit per source symbol**:

$$
\boxed{\mathbb E|c_B(X_1)|\leq\mathbb E|c_{QB}(X_1)|\leq\mathbb E|c_B(X_1)|+1.}
$$

The [quaternary Huffman code](../../../../quaternary-huffman-coding.md) uses the usual adjustment of adding zero-weight dummy leaves when needed. If the [alphabet](../../../../alphabet.md) has one symbol, both optimal codes may use the empty [codeword](../../../../codeword.md), giving the trivial endpoint.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
