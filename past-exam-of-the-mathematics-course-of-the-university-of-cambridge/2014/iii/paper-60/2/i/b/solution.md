<h1 id="2/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Shannon second coding theorem](../../../../../../../noisy-channel-coding-theorem.md) states that the operational [channel capacity](../../../../../../../channel-capacity.md) of a finite [discrete memoryless channel](../../../../../../../discrete-memoryless-channel.md) is $C=\max_{p(x)}I(X:Y)$: rates below this maximum admit block codes with error tending to zero, and rates above it cannot have vanishing error. For this channel the preceding calculation gives

$$
I(X:Y)=H(Y)-H(q)\leq\log_2 3-H(q),
$$

using [maximum entropy on a finite alphabet](../../../../../../../maximum-entropy-on-a-finite-alphabet.md). The transition matrix is a [doubly stochastic matrix](../../../../../../../doubly-stochastic-matrix.md). Therefore the uniform input has uniform output: $p(y)=\frac13\sum_xp(y\mid x)=1/3$. It achieves the entropy upper bound, and hence

$$
\boxed{C=\log_2 3-H(q)\quad\text{bits per channel use}.}
$$

Equivalently this is the [weakly symmetric channel capacity](../../../../../../../weakly-symmetric-channel-capacity.md) theorem: permutations of a common row and equal column sums make the uniform input optimal. If $q$ is uniform, the output contains no information about the input and the formula gives zero.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [I](../../i.md)
3. [2](../../../2.md)
4. [Paper 60](../../../../paper-60-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
