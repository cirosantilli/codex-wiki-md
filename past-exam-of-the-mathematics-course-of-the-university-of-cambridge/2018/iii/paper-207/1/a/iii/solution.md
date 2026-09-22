<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $i\ne s$, the [Markov property](../../../../../../../markov-property.md) and the definition of [transition intensity](../../../../../../../transition-intensity.md) give

$$
\mathbb P_r\{Z(u)=i,\text{ a jump }i\to s\text{ in }(u,u+du]\}
=p_{ri}(u)q_{is}\,du+o(du).
$$

Summing over the possible pre-jump states gives the density of the expected [Markov-chain entry count](../../../../../../../entry-count-of-a-continuous-time-markov-chain.md):

$$
\boxed{\frac{d}{du}\mathbb E_rN_s(u)=\sum_{i\ne s}p_{ri}(u)q_{is}.}
$$

For a finite-state [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md), the chance of two or more jumps in this short interval is $o(du)$. There is no $q_{ss}$ contribution: diagonal entries of the [infinitesimal generator](../../../../../../../infinitesimal-generator-stochastic-processes.md) encode exit rates, not jumps into the same state. With repeated entries possible, this density is an expected event rate rather than the [probability density function](../../../../../../../probability-density-function.md) of a single normalized random time.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
