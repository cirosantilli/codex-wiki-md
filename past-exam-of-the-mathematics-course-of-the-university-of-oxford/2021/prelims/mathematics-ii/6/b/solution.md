<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [Rolle's theorem](../../../../../../rolle-theorem.md) on each $[x_i,x_{i+1}]$. This gives $n$ ordered zeros of the [derivative](../../../../../../derivative.md) $f'$ strictly between the original $n+1$ zeros of $f$. Apply [Rolle's theorem](../../../../../../rolle-theorem.md) to $f'$ between each consecutive pair of its zeros to obtain $n-1$ ordered zeros of $f''$. Continue in this way.

To justify the iteration, for $j<n$, the [derivative](../../../../../../derivative.md) $f^{(j)}$ is [differentiable](../../../../../../differentiable-function.md) throughout $(a,b)$ and hence [continuous](../../../../../../continuous-function.md) there by [differentiability implies continuity](../../../../../../differentiability-implies-continuity.md). Every new closed [interval](../../../../../../interval-mathematics.md) lies strictly inside $(a,b)$, so [Rolle's theorem](../../../../../../rolle-theorem.md) applies at each step. After $j$ steps there are $n+1-j$ zeros of $f^{(j)}$. At $j=n$ this gives

$$
\boxed{\exists c\in(a,b):\quad f^{(n)}(c)=0.}
$$

This is the distinct-zero case of the [Rolle root count with multiplicities](../../../../../../rolle-root-count-with-multiplicities.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
