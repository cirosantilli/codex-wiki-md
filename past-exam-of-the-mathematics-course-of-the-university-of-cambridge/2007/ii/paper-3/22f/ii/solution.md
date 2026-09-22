<h1 id="22f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a nonsingular plane curve $F(s,t)=0$, at a point with $F_t\ne0$ the [holomorphic implicit function theorem](../../../../../../holomorphic-implicit-function-theorem.md) gives $t=t(s)$ and the chart coordinate $s$. Where $F_s\ne0$, use $t$ and express $s=s(t)$. Nonsingularity ensures at least one choice is available, and the coordinate transition functions and both restricted projections are holomorphic.

Here $F=t^4-P(s)$ with $P(s)=(s^2-1)(s-4)$. A singular point would require $t=0$, $P(s)=0$ and $P'(s)=0$. But $P$ has three distinct roots $-1,1,4$, so this is impossible. Hence **the curve is nonsingular**.

If $t\ne0$, $F_t=4t^3\ne0$, so $s$ is a local coordinate and the projection to $s$ is unramified. At $(s_0,0)$ for $s_0\in\{-1,1,4\}$, use $t$ as coordinate. Since $P'(s_0)\ne0$, solving $P(s)=t^4$ gives $s-s_0=t^4/P'(s_0)+O(t^8)$. Thus

$$
\boxed{\text{ramification points }(-1,0),(1,0),(4,0),\quad v_f=4\text{ at each}.}
$$

These are all the [ramification points](../../../../../../ramification-point-of-a-holomorphic-map.md) on the stated affine curve; no points at infinity belong to $Y\subset\mathbb C^2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [22F](../../22f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
