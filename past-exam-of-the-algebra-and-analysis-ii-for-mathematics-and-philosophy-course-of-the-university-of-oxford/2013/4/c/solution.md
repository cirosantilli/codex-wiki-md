<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Morera's theorem](../../../../morera-s-theorem.md) states that a [continuous](../../../../continuous-function.md) function on an [open subset](../../../../open-set.md) of $\mathbb C$ is [holomorphic](../../../../holomorphic-function-split.md) if its [integral](../../../../integral-split.md) around every triangular [contour](../../../../complex-integration-contour.md), with [triangle](../../../../triangle.md) and interior contained in that [open set](../../../../open-set.md), is zero.

To prove this, work in any open disk $D$ whose closure lies in $U$, and fix $z_0\in D$. Define

$$
F(z)=\int_{[z_0,z]}f(w)\,dw,
$$

where the segment lies in $D$ by [convexity](../../../../convex-function.md). The zero [integral](../../../../integral-split.md) on the [triangle](../../../../triangle.md) with vertices $z_0,z,z+h$ gives

$$
F(z+h)-F(z)=\int_{[z,z+h]}f(w)\,dw
=h\int_0^1f(z+th)\,dt.
$$

[Continuity](../../../../continuous-function.md) at $z$ implies that the last [integral](../../../../integral-split.md) tends to $f(z)$ as $h\to0$: its difference from $f(z)$ is [bounded](../../../../boundedness.md) by $\sup_{0\leq t\leq1}|f(z+th)-f(z)|$. Therefore $F'=f$ on $D$. The function $F$ is [holomorphic](../../../../holomorphic-function-split.md), and the allowed theorem that a [holomorphic](../../../../holomorphic-function-split.md) [derivative](../../../../derivative.md) is [holomorphic](../../../../holomorphic-function-split.md) implies that $f=F'$ is [holomorphic](../../../../holomorphic-function-split.md) on $D$.

Every point of $U$ lies in such a disk, proving the result throughout $U$:

$$
\boxed{\text{continuity plus vanishing triangle integrals implies holomorphicity}.}
$$

The proof is local and does not require $U$ to be [simply connected](../../../../simply-connected-space.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
