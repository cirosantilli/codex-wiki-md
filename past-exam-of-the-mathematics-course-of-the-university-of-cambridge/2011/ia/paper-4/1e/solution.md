<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

An [inverse function](../../../../../inverse-function.md) of $f:X\to Y$ is a function $h:Y\to X$ satisfying both

$$
h\circ f=\operatorname{id}_X,\qquad f\circ h=\operatorname{id}_Y.
$$

These are two-sided inverse identities. If $f(x)=f(x')$, apply $h$ to get $x=x'$, so $f$ is [injective](../../../../../injective-function.md). For every $y\in Y$, the identity $f(h(y))=y$ supplies a preimage, so $f$ is [surjective](../../../../../surjective-function.md). Thus $f$ is a [bijection](../../../../../bijection.md).

Conversely, if $f$ is a [bijection](../../../../../bijection.md), each $y\in Y$ has exactly one preimage. Define $h(y)$ to be that preimage. Then $f(h(y))=y$ and $h(f(x))=x$, giving both identities. Hence **a function has a two-sided inverse exactly when it is a bijection**. This also makes its [inverse function](../../../../../inverse-function.md) unique.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
