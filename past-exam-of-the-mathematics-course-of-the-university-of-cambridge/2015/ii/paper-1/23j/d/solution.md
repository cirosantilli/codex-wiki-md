<h1 id="23j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each $x$, $g(x)^n\to0$ if $g(x)<1$, and remains one if $g(x)=1$. Continuity gives pointwise convergence to $f(0)$ off $E=\{x:g(x)=1\}$ and to $f(1)$ on $E$. The functions are measurable and bounded by $\max_{[0,1]}|f|$, an integrable constant on a unit-length interval. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore gives

$$
\boxed{\lim_n\int_0^1f(g(x)^n)dx=(1-|E|)f(0)+|E|f(1)}.
$$

Here $|E|$ is [Lebesgue measure](../../../../../../lebesgue-measure.md). This convex combination belongs to **$[f(0),f(1)]$**, without requiring $f$ to be monotone.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [23J](../../23j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
