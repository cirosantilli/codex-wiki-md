<h1 id="3k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a chosen coordinate and symbol $\varepsilon\in\{0,1\}$, the [shortened code](../../../../../../shortened-code.md) retains the words having that symbol in the chosen coordinate and then deletes that coordinate. For the last coordinate,

$$
\overline C_\varepsilon
=\{(x_1,\ldots,x_{n-1}):(x_1,\ldots,x_{n-1},\varepsilon)\in C\}.
$$

At least one of the two coordinate fibres contains at least $\lceil m/2\rceil$ words. Choose that fibre and, if necessary, discard surplus words. Because all retained words agree in the deleted coordinate, their mutual distances do not change. Hence one can always obtain

$$
\boxed{\overline C\text{ with guaranteed parameters }
[n-1,\lceil m/2\rceil,d]}.
$$

Without discarding words, its size is that of the chosen fibre and its minimum distance is at least $d$.

For the final calculation, the given code is the whole space $\mathbb F_2^3$, so its parity extension is the length-four [even-weight binary code](../../../../../../even-weight-binary-code.md). In a [binary symmetric channel](../../../../../../binary-symmetric-channel.md), parity fails to notice a nonzero error exactly when an even number of bits flips. The possible error weights are therefore two and four. Their total probability is

$$
\boxed{
\binom42p^2(1-p)^2+p^4
=6p^2(1-p)^2+p^4
}.
$$

This excludes the weight-zero event, since it is not an [undetected error](../../../../../../undetected-error.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3K](../../3k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
