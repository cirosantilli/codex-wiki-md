<h1 id="10e/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $h(x)$ be the probability that the [simple symmetric random walk](../../../../../../../simple-random-walk-on-the-integer-line.md) starting at $x\in\{0,\ldots,n\}$ hits zero before $n$. The first-step recurrence is

$$
h(x)=\frac12h(x-1)+\frac12h(x+1),
\qquad
h(0)=1,\quad h(n)=0.
$$

The recurrence says that $h$ is affine, and the boundary values determine it:

$$
\boxed{h(x)=\frac{n-x}{n}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [10E](../../../10e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
