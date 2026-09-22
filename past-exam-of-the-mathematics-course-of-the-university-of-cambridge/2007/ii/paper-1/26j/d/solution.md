<h1 id="26j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a renewal gap $T$ of mean $m$, the equilibrium first-delay density is $\mathbb P(T>t)/m$. Here $m=3/\lambda$ and the [Erlang distribution](../../../../../../erlang-distribution.md) survivor is $e^{-\lambda t}(1+\lambda t+\lambda^2t^2/2)$. The [equilibrium delay of an Erlang renewal process](../../../../../../equilibrium-delay-of-an-erlang-renewal-process.md) is therefore

$$
\boxed{f_0(t)=\frac\lambda3e^{-\lambda t}\left(1+\lambda t+\frac{\lambda^2t^2}{2}\right).}
$$

This is an equal mixture of shapes one, two and three. For each equilibrium stream use this first delay, followed by independent shape-three gaps. A joint stationary version of the cyclic routing is obtained by choosing the initial position in the three-label cycle uniformly at random, independently of the Poisson arrivals. Its marginal streams have the stated equilibrium law, but remain dependent on one another.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [26J](../../26j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
