<h1 id="11k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a received word $y$, the ideal-observer rule chooses a message $i$ maximizing the posterior probability

$$
\mathbb P(M=i\mid Y=y).
$$

Maximum-likelihood decoding chooses $i$ maximizing

$$
\mathbb P(Y=y\mid M=i),
$$

and minimum-distance decoding chooses a codeword minimizing its Hamming distance from $y$.

Bayes' formula gives

$$
\mathbb P(M=i\mid Y=y)
\propto \mathbb P(Y=y\mid M=i)\mathbb P(M=i).
$$

Equal message priors therefore make ideal-observer and maximum-likelihood decoding identical. On a [binary symmetric channel](../../../../../../binary-symmetric-channel.md), if $d=d_H(y,c_i)$, then

$$
\mathbb P(Y=y\mid M=i)=p^d(1-p)^{n-d}.
$$

For $p<1/2$, this strictly decreases with $d$, so maximum likelihood and minimum distance agree.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11K](../../11k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
