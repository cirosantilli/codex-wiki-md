<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Colour each [edge](../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../complete-graph.md) $K_n$ independently red or blue, with [probability](../../../../../probability.md) $1/2$ for each colour. Every four-element [subset](../../../../../subset.md) $A$ of [vertices](../../../../../vertex-graph-theory.md) determines exactly one copy of $K_4$, containing six [edges](../../../../../edge-of-a-graph.md). These six [edges](../../../../../edge-of-a-graph.md) are all red with [probability](../../../../../probability.md) $2^{-6}$ and all blue with [probability](../../../../../probability.md) $2^{-6}$. The events are [disjoint events](../../../../../disjoint-events.md), so

$$
\mathbb P(A\text{ is monochromatic})=2\cdot2^{-6}=2^{-5}.
$$

Let $I_A$ be the [indicator random variable](../../../../../indicator-random-variable.md) for this event and let $Z=\sum_A I_A$ count the [monochromatic](../../../../../monochromatic-set.md) copies. [Linearity of expectation](../../../../../linearity-of-expectation.md) gives

$$
\mathbb EZ=\sum_A\mathbb E I_A=\binom n4\,2^{-5}.
$$

The [indicator random variables](../../../../../indicator-random-variable.md) for overlapping copies need not be [independent](../../../../../independent-random-variables.md). Averaging over all [edge colorings](../../../../../edge-coloring.md) ensures that at least one has $Z\leq\mathbb EZ$. Thus the [probabilistic method](../../../../../probabilistic-method.md) proves

$$
\boxed{\text{Some two-colour edge coloring has }Z\leq\frac1{32}\binom n4.}
$$

For $0\leq n<4$, both sides are zero and any [edge coloring](../../../../../edge-coloring.md) works. Copies are counted by their four-[vertex](../../../../../vertex-graph-theory.md) [subsets](../../../../../subset.md), rather than by their $4!$ possible labellings.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
