<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the [stochastic SIR model](../../../../../../stochastic-sir-model.md), the state $(S,I,R)$ is a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) on nonnegative integer triples summing to $N+1$, initially $(N,1,0)$. Its only transitions are

$$
\boxed{(s,i,r)\longrightarrow(s-1,i+1,r)\text{ at rate }\beta si,\qquad(s,i,r)\longrightarrow(s,i-1,r+1)\text{ at rate }\gamma i.}
$$

Rates vanish when a proposed transition would leave the state space. Equivalently, with independent unit-rate [Poisson processes](../../../../../../poisson-process.md) $A,B$, the [Poisson time-change representation of a Markov chain](../../../../../../poisson-time-change-representation-of-a-markov-chain.md) is

$$
S(t)=N-A\left(\int_0^t\beta S(u-)I(u-)\,du\right),\quad R(t)=B\left(\int_0^t\gamma I(u-)\,du\right),\quad I(t)=N+1-S(t)-R(t).
$$

The left limits describe the state immediately before each jump. In the [Gillespie algorithm](../../../../../../gillespie-algorithm.md), wait an [exponential distribution](../../../../../../exponential-distribution.md) time with rate $\beta si+\gamma i$, then choose infection or recovery in proportion to these two rates.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
