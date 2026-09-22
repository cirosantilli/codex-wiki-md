<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [discrete memoryless channel](../../../../../discrete-memoryless-channel.md) has finite input and output [alphabets](../../../../../alphabet.md) and fixed [conditional probabilities](../../../../../conditional-probability.md) $M_{ij}=\mathbb P(Y=j\mid X=i)$, whose rows [sum](../../../../../sum.md) to one. Memorylessness means that for successive uses, conditional on the input sequence, the output [probabilities](../../../../../probability.md) factor as the product of these one-use [conditional probabilities](../../../../../conditional-probability.md).

Its information [capacity](../../../../../channel-capacity.md) in [bits](../../../../../bit.md) per use is

$$
\boxed{C=\max_{p_X}I(X;Y)=\max_{p_X}\left[H(Y)-\sum_i p_X(i)H(M_{i\cdot})\right].}
$$

The maximization varies the input distribution while keeping the [channel](../../../../../communication-channel.md) [matrix](../../../../../matrix.md) fixed. The output distribution is $p_XM$ in the row-vector convention.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
