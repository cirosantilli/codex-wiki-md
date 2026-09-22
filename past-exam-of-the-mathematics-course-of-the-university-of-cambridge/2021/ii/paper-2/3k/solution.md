<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

For a [binary symmetric channel](../../../../../binary-symmetric-channel.md) with crossover probability $p$, the capacity is

$$
C=1-H_2(p),
$$

where $H_2$ is the [binary entropy](../../../../../binary-entropy.md). [Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) says that for every transmission rate $R<C$ and every $\epsilon>0$, sufficiently long block codes exist with rate at least $R$ and decoding-error probability below $\epsilon$; conversely, a sequence of codes whose error tends to zero cannot have limiting rate above $C$.

For the general channel let $X$ and $Y$ be its input and output. Every conditional output distribution is a permutation of $(p_1,\ldots,p_n)$, hence

$$
H(Y\mid X)=-\sum_{i=1}^np_i\log p_i
$$

for every input distribution. Since $H(Y)\leq\log n$,

$$
I(X;Y)\leq\log n+\sum_i p_i\log p_i.
$$

The uniform input makes every output probability equal to $1/n$: the column-permutation assumption and the total sum imply that all column sums are equal to one. It therefore attains $H(Y)=\log n$, proving

$$
\boxed{C=\log n+\sum_i p_i\log p_i}.
$$

In the displayed four-output channel each row is a permutation of

$$
\left(\frac13,\frac13,\frac16,\frac16\right).
$$

With base-two logarithms,

$$
\begin{aligned}
C
&=2+\frac23\log\frac13+\frac13\log\frac16\\
&=2-\log3-\frac13
=\boxed{\frac53-\log3}.
\end{aligned}
$$

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
