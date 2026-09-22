<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $N(u)$ count all jumps of the [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md). Its [Markov-chain entry count](../../../../../../../entry-count-of-a-continuous-time-markov-chain.md) into state $s$ is

$$
N_s(t)=\sum_{0<u\leq t}\mathbf1\{Z(u-)\ne s,\ Z(u)=s\}
=\int_{(0,t]}\mathbf1\{Z(u)=s\}\,dN(u).
$$

Thus

$$
\boxed{E_{rs}(t)=\mathbb E_r\!\left[\int_{(0,t]}\mathbf1\{Z(u)=s\}\,dN(u)\right].}
$$

This is a [Lebesgue-Stieltjes integral](../../../../../../../lebesgue-stieltjes-integration.md) against a [counting process](../../../../../../../counting-process.md), so each jump contributes one. The initial occupation of state $s$ is not counted as an entry. An ordinary time integral of an [indicator random variable](../../../../../../../indicator-random-variable.md) asserting a jump at exactly time $u$ would be zero, since individual jump times have zero [Lebesgue measure](../../../../../../../lebesgue-measure.md). The requested integral must therefore use this counting-measure interpretation. Assume non-explosion and finite expected jump counts on bounded intervals, as holds for a finite-state [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
