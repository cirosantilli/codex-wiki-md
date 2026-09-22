<h1 id="24h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $c$ be the center of the containing disk and take arclength around the closed curve. The periodic function $\Phi(s)=|\gamma(s)-c|^2/2$ has a maximum. At a maximum $s_0$,

$$
0\ge\Phi''(s_0)=1+(\gamma(s_0)-c)\cdot\gamma''(s_0).
$$

By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the containing radius, $1\le|\gamma(s_0)-c|\,|\gamma''(s_0)|\le r|k(s_0)|$. Therefore

$$
\boxed{|k(s_0)|\ge r^{-1}.}
$$

Closedness provides an interior maximum on the periodic parameter domain. Without it, the straight segment $\gamma(s)=(s,0)$ for $-r<s<r$ lies in the disk but has signed [curvature](../../../../../../curvature.md) identically zero, giving the required counterexample.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24H](../../24h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
