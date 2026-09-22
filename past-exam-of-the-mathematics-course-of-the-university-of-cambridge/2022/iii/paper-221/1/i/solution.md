<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [potential outcome](../../../../../../potential-outcome.md) notation, a valid [instrumental variable](../../../../../../instrumental-variable.md) $Z$ must satisfy:

- [Instrument relevance](../../../../../../instrument-relevance.md): the conditional law of $A$ changes with $Z$.
- [Instrumental-variable independence](../../../../../../instrumental-variable-independence.md): $Z$ is independent of the joint collection of potential treatments and outcomes, such as $\{A(z),Y(a):z,a\}$.
- The [exclusion restriction](../../../../../../exclusion-restriction.md): $Y(z,a)=Y(a)$, so $Z$ can affect $Y$ only through $A$.
- [Consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md) and no [interference in causal inference](../../../../../../interference-in-causal-inference.md) connect the potential variables to the observations.

In the graph, $Z_1$ has open noncausal paths to $Y$ that do not pass through $A$, including

$$
Z_1\leftarrow M_1\to C\to Y
\qquad\text{and}\qquad
Z_1\leftarrow S\to Z_3\to Y.
$$

Equivalently, these paths remain after deleting the causal edge $A\to Y$. Thus $Z_1$ is associated with potential outcomes through the latent variables $C$ and $S$, violating [instrumental-variable independence](../../../../../../instrumental-variable-independence.md); it is not a valid marginal instrument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
