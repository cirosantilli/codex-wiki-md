<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose a [uniform random permutation](../../../../../uniform-random-permutation.md) of the $n$ [vertices](../../../../../vertex-graph-theory.md), giving every one of the $n!$ orders the same [probability](../../../../../probability.md). For a fixed [vertex](../../../../../vertex-graph-theory.md) $i$, consider $i$ together with its $d_i$ [graph neighbours](../../../../../neighbour-of-a-vertex.md). The relative order of these $d_i+1$ [vertices](../../../../../vertex-graph-theory.md) is uniform, so each is equally likely to be first. The membership rule for $S(\sigma)$ therefore gives

$$
\boxed{\mathbb P(i\in S(\sigma))=\frac1{d_i+1}.}
$$

Let $I_i$ be the [indicator random variable](../../../../../indicator-random-variable.md) of this event. The [cardinality](../../../../../cardinality.md) is $|S(\sigma)|=\sum_{i=1}^n I_i$, and [linearity of expectation](../../../../../linearity-of-expectation.md) gives

$$
\boxed{\mathbb E|S(\sigma)|=\sum_{i=1}^n\mathbb E I_i=\sum_{i=1}^n\frac1{d_i+1}.}
$$

The [indicator random variables](../../../../../indicator-random-variable.md) are generally dependent; only the [uniform random permutation](../../../../../uniform-random-permutation.md) and [linearity of expectation](../../../../../linearity-of-expectation.md) were needed. An isolated [vertex](../../../../../vertex-graph-theory.md) has $d_i=0$ and is always included, as the formula correctly predicts.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
