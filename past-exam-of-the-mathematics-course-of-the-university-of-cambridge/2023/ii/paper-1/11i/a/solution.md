<h1 id="11i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [binary symmetric channel](../../../../../../binary-symmetric-channel.md) independently flips each input bit with probability $p$, so, with rows indexed by the input and columns by the output, its channel matrix is

$$
\boxed{
\begin{pmatrix}
1-p&p\\
p&1-p
\end{pmatrix}}
.
$$

If $p>1/2$, complementing every received bit converts the channel into one with crossover probability $1-p<1/2$ without changing its information-carrying ability. The [case $p=1/2$](../../../../../../completely-noisy-binary-symmetric-channel.md) has identical rows and [capacity](../../../../../../binary-symmetric-channel-capacity.md) zero, so it suffices to study $p<1/2$.

The [Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md) states that for every rate below the [channel capacity](../../../../../../channel-capacity.md) there are arbitrarily long codes whose decoding error tends to zero, whereas no sequence of codes with rate above capacity can have vanishing error. It also identifies

$$
C=\max_{P_X}I(X;Y).
$$

For the present channel,

$$
I(X;Y)=H(Y)-H(Y\mid X)=H(Y)-h_2(p).
$$

The output entropy is at most one bit, with equality for a uniform input. Hence the [binary symmetric channel capacity](../../../../../../binary-symmetric-channel-capacity.md) is

$$
\boxed{C=1-h_2(p)}
$$

bits per channel use.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11I](../../11i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
