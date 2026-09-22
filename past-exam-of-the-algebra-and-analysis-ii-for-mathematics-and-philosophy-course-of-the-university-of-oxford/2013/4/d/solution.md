<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For two moving vertices $p(s),q(s)$, the [integral](../../../../integral-split.md) along their joining segment is

$$
J_{p,q}(s)=\bigl(q(s)-p(s)\bigr)\int_0^1 f\bigl((1-t)p(s)+tq(s)\bigr)\,dt.
$$

The [integral](../../../../integral-split.md) factor is [continuous](../../../../continuous-function.md) in $s$ by the allowed fact, and the other factor is [continuous](../../../../continuous-function.md) because the vertices are [continuous](../../../../continuous-function.md). Thus $J_{p,q}$ is [continuous](../../../../continuous-function.md), including when its two endpoints coincide.

The [integral](../../../../integral-split.md) around the [triangle](../../../../triangle.md) is exactly

$$
I(s)=J_{a,b}(s)+J_{b,c}(s)+J_{c,a}(s).
$$

Each term is [continuous](../../../../continuous-function.md), so their sum is [continuous](../../../../continuous-function.md) at zero and

$$
\boxed{\lim_{s\to0}\int_{\Delta_s}f(z)\,dz=\int_{\Delta_0}f(z)\,dz.}
$$

No holomorphicity is used here. [Compactness](../../../../compact-space.md) of the fixed containing [triangle](../../../../triangle.md) also gives a direct proof of the allowed fact through [uniform continuity](../../../../uniform-continuity.md) of $f$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../../algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
