# Conditional expectations for maximum cut

↑ **Parent:** [Method of conditional probabilities](method-of-conditional-probabilities.md)

Let $G=(V,E)$ be a finite undirected [simple graph](simple-graph.md), with $n=|V|$ [vertices](vertex-graph-theory.md) and $m=|E|$ [edges](edge-of-a-graph.md). A [cut of a graph](cut-graph-theory.md) assigns each [vertex](vertex-graph-theory.md) a label zero or one; an [edge](edge-of-a-graph.md) crosses precisely when its endpoints have different labels. Its size is the number of crossing [edges](edge-of-a-graph.md). A [maximum cut](maximum-cut.md) maximizes that size.

For the analysis, assign [independent](independent-random-variables.md) fair [bits](bit.md) $X_v$ to the [vertices](vertex-graph-theory.md). For each [edge](edge-of-a-graph.md) $uv$, the [indicator random variable](indicator-random-variable.md) $I_{uv}=\mathbf1_{\{X_u\ne X_v\}}$ has [expected value](expected-value-split.md) $1/2$: exactly two of the four equally likely endpoint assignments cross. Thus [linearity of expectation](linearity-of-expectation.md) gives the [random cut lower bound](random-cut-lower-bound.md):

$$
C=\sum_{uv\in E}I_{uv},\qquad \mathbb E C=\sum_{uv\in E}\frac12=\frac m2.
$$

[Linearity of expectation](linearity-of-expectation.md) does not require the [indicator random variables](indicator-random-variable.md) to be [independent](independent-random-variables.md). What matters here is the stipulated distribution of the endpoint [bits](bit.md).

**Table of contents**

- [Conditional expectation cut formula](conditional-expectation-cut-formula.md)
- [Conditional expectations cut example](conditional-expectations-cut-example.md)
- [Conditional expectations algorithm cost](conditional-expectations-algorithm-cost.md)

## ↑ Ancestors (6)

1. [Method of conditional probabilities](method-of-conditional-probabilities.md)
2. [Derandomization](derandomization.md)
3. [Randomized algorithm](randomized-algorithm.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)
