<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

The received word $001$ has Hamming distances $1$ from $000$ and $2$ from $111$, so

$$
P(001\mid000)=\frac9{64},\qquad P(001\mid111)=\frac3{64}.
$$

After multiplying by the priors, the unnormalized posterior probabilities are $9/320$ and $12/320$. Thus the [ideal](../../../../../ideal.md) observer decodes as $111$, while maximum-likelihood and [minimum-distance decoding](../../../../../minimum-distance-decoding.md) both choose $000$.

The [ideal](../../../../../ideal.md) observer minimizes average error but needs priors and channel statistics. Maximum likelihood needs the channel law but not priors, and can be suboptimal for unequal codeword probabilities. Minimum distance is simple and agrees with maximum likelihood for a [binary symmetric channel](../../../../../binary-symmetric-channel.md) with crossover probability below $1/2$, but ignores unequal priors and general channel asymmetry.

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
