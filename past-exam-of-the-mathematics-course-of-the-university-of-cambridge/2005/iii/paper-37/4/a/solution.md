<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [discrete memoryless channel](../../../../../../discrete-memoryless-channel.md) is specified by discrete input and output [alphabets](../../../../../../alphabet.md) and a transition [probability](../../../../../../probability.md) $W(y|x)$, with $W(y|x)\geq0$ and $\sum_yW(y|x)=1$. Its successive outputs are conditionally independent given the inputs, with the same transition rule at every use:

$$
\Pr(Y_1=y_1,\ldots,Y_n=y_n\mid X_1=x_1,\ldots,X_n=x_n)
=\prod_{j=1}^nW(y_j|x_j).
$$

Operationally, its [channel capacity](../../../../../../channel-capacity.md) is the supremum of communication rates in [bits](../../../../../../bit.md) per use attainable by increasingly long block codes with decoding error [probability](../../../../../../probability.md) tending to zero. For finite [alphabets](../../../../../../alphabet.md), the equivalent Shannon characterization is

$$
C=\max_{P_X}I(X;Y),\qquad
I(X;Y)=H(Y)-H(Y|X),
$$

where $H$ is [Shannon entropy](../../../../../../information-entropy.md), $H(Y|X)$ is classical [conditional entropy](../../../../../../conditional-entropy.md), and the maximization is over the input [probability distribution](../../../../../../probability-distribution.md).

For the channel in question, the transition [matrix](../../../../../../matrix.md), with input symbols indexing rows, is

$$
W=\begin{pmatrix}
2/3&1/3&0\\
0&2/3&1/3\\
1/3&0&2/3
\end{pmatrix}.
$$

Every row has the same [Shannon entropy](../../../../../../information-entropy.md), namely the [binary entropy](../../../../../../binary-entropy.md) $h_2(1/3)$. Consequently $H(Y|X)=h_2(1/3)$ for every input [probability distribution](../../../../../../probability-distribution.md). Since the output has three symbols, the [maximum entropy on a finite alphabet](../../../../../../maximum-entropy-on-a-finite-alphabet.md) gives

$$
I(X;Y)\leq\log_2 3-h_2(1/3).
$$

Choose a uniform input. Each column of $W$ sums to one, so $P_Y(y)=1/3$ for every output symbol and the upper bound is attained. Finally

$$
h_2(1/3)=-\frac13\log_2\frac13-\frac23\log_2\frac23
=\log_2 3-\frac23.
$$

Thus the [cyclic ternary channel capacity](../../../../../../cyclic-ternary-channel-capacity.md) is

$$
\boxed{C=\frac23\text{ bits per channel use},}
$$

achieved by a uniform input [probability distribution](../../../../../../probability-distribution.md). This is a [weakly symmetric channel capacity](../../../../../../weakly-symmetric-channel-capacity.md) calculation: the [matrix](../../../../../../matrix.md) rows are permutations and the column sums agree. The channel is not the usual ternary symmetric-error channel, since an error has only one possible changed output for each input.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
