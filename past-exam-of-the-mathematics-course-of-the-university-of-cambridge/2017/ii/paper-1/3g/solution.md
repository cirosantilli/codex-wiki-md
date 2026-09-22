<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

The ideal observer performs [maximum a posteriori decoding](../../../../../maximum-a-posteriori-decoding.md): for received word $y$, it maximizes $\Pr(X=c\mid Y=y)$, equivalently $\Pr(X=c)\Pr(Y=y\mid X=c)$. [Maximum-likelihood decoding](../../../../../maximum-likelihood-decoding.md) maximizes the latter conditional likelihood alone. [Minimum-distance decoding](../../../../../minimum-distance-decoding.md) minimizes the [Hamming distance](../../../../../hamming-distance.md) $d(c,y)$. Ties may be resolved arbitrarily among maximizers.

For independent errors in a [binary symmetric channel](../../../../../binary-symmetric-channel.md),

$$
\Pr(Y=y\mid X=c)=p^{d(c,y)}(1-p)^{n-d(c,y)}.
$$

For $0<p<1/2$, its ratio on increasing the distance by one is $p/(1-p)<1$. Thus [maximum-likelihood decoding](../../../../../maximum-likelihood-decoding.md) and [minimum-distance decoding](../../../../../minimum-distance-decoding.md) select exactly the same codewords. At the allowed endpoint $p=0$, they agree on a possible observation $y\in C$; impossible observations have zero likelihood for every codeword, so an arbitrary maximum-likelihood tie rule need not agree with minimum distance. This qualification is needed for the literal assumption $p<1/2$.

For the specified observation, the [Hamming distances](../../../../../hamming-distance.md) from 000 and 111 are two and one. Their likelihoods are $3/64$ and $9/64$, respectively. After multiplying by the priors, their joint probabilities are $12/320$ and $9/320$, so their posterior probabilities are $4/7$ and $3/7$. Therefore

$$
\boxed{\text{ideal observer: }000,\qquad\text{maximum likelihood: }111,\qquad\text{minimum distance: }111}.
$$

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
