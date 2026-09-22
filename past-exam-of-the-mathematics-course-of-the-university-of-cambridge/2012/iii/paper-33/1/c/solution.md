<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because each increment is $\pm1$, the event at time $k$ defining $T$ is exactly $\{X_{k-1}=X_k=1\}$. Therefore, for $n\geq2$,

$$
\{T\leq n\}=\bigcup_{k=2}^n\{X_{k-1}=X_k=1\}\in\mathcal F_n,
$$

and for $n<2$ this event is empty. Thus **$T$ is a [stopping time](../../../../../../stopping-time.md)** for the [natural filtration](../../../../../../natural-filtration.md).

On the other hand, $\{U\leq0\}=\{T=2\}=\{X_1=X_2=1\}$. This event has [probability](../../../../../../probability.md) $1/4$, whereas the initial [sigma-algebra](../../../../../../sigma-algebra.md) $\mathcal F_0$ is trivial, even after completion up to null sets. It therefore cannot belong to $\mathcal F_0$. Hence **$U=T-2$ is not a [stopping time](../../../../../../stopping-time.md)**. Subtracting a deterministic delay from a [stopping time](../../../../../../stopping-time.md) can require information from the future.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
