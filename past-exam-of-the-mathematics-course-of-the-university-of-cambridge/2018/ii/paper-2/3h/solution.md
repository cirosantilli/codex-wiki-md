<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

The [binary symmetric channel](../../../../../binary-symmetric-channel.md) with crossover probability $p$ has channel matrix

$$
\boxed{\begin{pmatrix}1-p&p\\p&1-p\end{pmatrix}.}
$$

[Maximum-likelihood decoding](../../../../../maximum-likelihood-decoding.md) chooses a codeword $c$ maximizing $\mathbb P(Y=y\mid X=c)$, while [minimum-distance decoding](../../../../../minimum-distance-decoding.md) chooses one minimizing the [Hamming distance](../../../../../hamming-distance.md) $d_H(c,y)$. For a block of length $n$ sent through a binary symmetric channel,

$$
\mathbb P(Y=y\mid X=c)
=p^{d_H(c,y)}(1-p)^{n-d_H(c,y)}
=(1-p)^n\left(\frac p{1-p}\right)^{d_H(c,y)}.
$$

When $p<1/2$, the final factor decreases strictly with the distance. Thus **maximum-likelihood and minimum-distance decoding agree**.

For the length-three [repetition code](../../../../../repetition-code.md) $\{000,111\}$, majority decoding is wrong exactly when at least two bits flip. Therefore

$$
\boxed{\mathbb P(\text{error})
=\binom32p^2(1-p)+p^3
=3p^2-2p^3.}
$$

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
