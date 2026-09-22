<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each pair of inputs, define the joint probabilities

$$
\boxed{P(x,y|a,b)=\frac14[1+xyf(\theta(a,b))]},
\qquad x,y\in\{-1,1\}.
$$

They are nonnegative because $|f|\leq1$, sum to one, and have the required correlation:

$$
\sum_{x,y}xyP(x,y|a,b)=f(\theta(a,b)).
$$

Both marginals are uniform,

$$
\sum_yP(x,y|a,b)=\frac12,
\qquad
\sum_xP(x,y|a,b)=\frac12,
$$

independently of the remote input. The device is thus a [no-signalling box](../../../../../../no-signalling-box.md): its superquantum correlation does not by itself transmit a message, so it is compatible with [relativistic causality](../../../../../../relativistic-causality.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
