<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $C_0=[0,1]$. Inductively, replace each component interval of $C_n$ by its two closed end intervals, each of length $\ell_{n+1}:=q_{n+1}/2^{n+1}$. The current component length is $\ell_n=q_n/2^n$. Because $q_{n+1}<q_n$, the removed central gap has positive length

$$
\ell_n-2\ell_{n+1}=\frac{q_n-q_{n+1}}{2^n}.
$$

This is a [generalized Cantor set](../../../../generalized-cantor-set.md) construction. The three required properties are checked in parts [i](i.md), [ii](ii.md) and [iii](iii.md).

The [sets](../../../../set-split.md) are [closed](../../../../closed-set.md), [measurable](../../../../measurability.md), decreasing, and contained in $[0,1]$, which has finite [Lebesgue measure](../../../../lebesgue-measure.md). By [continuity from above of a measure](../../../../continuity-from-above-of-a-measure.md),

$$
\boxed{m(C)=m\!\left(\bigcap_{n=0}^\infty C_n\right)=\lim_{n\to\infty}q_n.}
$$

This limit exists because $(q_n)$ is a bounded decreasing [monotone sequence](../../../../monotone-sequence.md). To exclude a nondegenerate [interval](../../../../interval-mathematics.md) $J\subseteq C$, note that its [connectedness](../../../../connected-space.md) forces it into a single component interval of every $C_n$: crossing two components would cross a removed gap. Its length would therefore be at most $2^{-n}$ for every $n$, which is impossible for a positive-length [interval](../../../../interval-mathematics.md). Thus **$C$ contains no nondegenerate [interval](../../../../interval-mathematics.md)**, even when its [Lebesgue measure](../../../../lebesgue-measure.md) is positive.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
