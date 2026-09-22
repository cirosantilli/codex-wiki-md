<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

A [metric space](../../../../../metric-space.md) is a [complete metric space](../../../../../complete-metric-space.md) when every [Cauchy sequence](../../../../../cauchy-sequence.md) converges to a point of that space. It is a [totally bounded space](../../../../../totally-bounded-space.md) when, for every $\varepsilon>0$, finitely many open metric balls of radius $\varepsilon$ cover the space.

With their usual distances, **$\mathbb R$ is complete but not totally bounded**, and **$(0,1)$ is totally bounded but not complete**. The [Cauchy sequence](../../../../../cauchy-sequence.md) $1/n$ in $(0,1)$ has its limit outside the space; no finite collection of balls of a fixed radius covers $\mathbb R$.

For the requested [continuous functions](../../../../../continuous-function.md), take

$$
f:\mathbb R\longrightarrow(0,\infty),\qquad f(x)=e^x,
$$

and

$$
g:(0,1)\longrightarrow(1,\infty),\qquad g(x)=\frac1x.
$$

Both are continuous and onto. The domain of $f$ is a [complete metric space](../../../../../complete-metric-space.md), but its image is not complete because $1/n$ tends to the missing point $0$. The domain of $g$ is a [totally bounded space](../../../../../totally-bounded-space.md), but its unbounded image is not totally bounded. Uniform continuity, unlike mere continuity, would preserve total boundedness.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
