<h1 id="11f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [Galton-Watson process](../../../../../../galton-watson-process.md), condition on the number $K$ of children of the initial individual. The descendants of these children over the next $n$ generations are independent copies of $X_n$. The [probability generating function](../../../../../../probability-generating-function.md) of their total, conditional on $K=k$, is $G_n(s)^k$. Averaging over the family-size law gives

$$
G_{n+1}(s)=\mathbb E[G_n(s)^K]=\boxed{G(G_n(s))},\qquad G_0(s)=s.
$$

This is the [branching-process generating-function iteration](../../../../../../branching-process-generating-function-iteration.md). Conditioning instead on the last generation gives $G_n(G(s))$; both orders agree because $G_n$ is the $n$th iterate of the same function $G$. The argument holds on the usual [PGF](../../../../../../probability-generating-function.md) domain $|s|\leq1$, with larger domains available when the corresponding expectations converge.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
