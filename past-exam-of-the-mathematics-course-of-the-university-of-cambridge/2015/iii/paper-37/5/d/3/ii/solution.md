<h1 id="5/d/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\bar\pi$ be the normalized target and $\bar\pi_{-i}$ its [marginal distribution](../../../../../../../../marginal-distribution.md). A coordinate-$i$ kernel $P_i$ leaves $x_{-i}=x'_{-i}$ and has the joint old-new measure

$$
\bar\pi(dx)P_i(x,dx')=
\bar\pi_{-i}(dx_{-i})\,
\pi_i(x_i\mid x_{-i})\,dx_i\,
\pi_i(x_i'\mid x_{-i})\,dx_i'\,
\delta_{x_{-i}}(dx'_{-i}).
$$

This is symmetric in the old and new state: the common remaining coordinates are fixed and the two conditional factors exchange places. Thus each coordinate kernel satisfies [detailed balance](../../../../../../../../detailed-balance.md). Averaging them with the fixed weights $1/p$ proves

$$
\boxed{\bar\pi(dx)P(x,dx')=\bar\pi(dx')P(x',dx).}
$$

Integrating out the old state proves invariance of $\bar\pi$. The common normalization cancels, so detailed balance can also be written with the unnormalized target. This establishes [detailed balance of a random-scan Gibbs sampler](../../../../../../../../detailed-balance-of-a-random-scan-gibbs-sampler.md) and a [reversible Markov chain](../../../../../../../../reversible-markov-chain.md). Fresh independent random choices make the update a [Markov chain](../../../../../../../../markov-chain.md), as explained above; invariance is not an assertion that an arbitrarily initialized chain starts in stationarity.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [D](../../../d.md)
4. [5](../../../../5.md)
5. [Paper 37](../../../../../paper-37-split.md)
6. [Iii](../../../../../split.md)
7. [2015](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
