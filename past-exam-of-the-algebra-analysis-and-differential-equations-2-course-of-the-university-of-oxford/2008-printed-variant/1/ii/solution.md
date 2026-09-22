<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $N=T-I$. [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md) gives $N^3=0$. Its [minimal polynomial](../../../../minimal-polynomial.md) is therefore $X^k$ for exactly one $k\in\{1,2,3\}$, so the possibilities for that of $T$ are

$$
\boxed{X-1,\quad(X-1)^2,\quad(X-1)^3.}
$$

Let $d=\dim\ker N$, which is the [dimension](../../../../dimension-vector-space.md) of the only [eigenspace](../../../../eigenspace.md). If $d=3$, then $N=0$ and $T=I$.

If $d=2$, [rank-nullity theorem](../../../../rank-nullity-theorem.md) gives $\dim\operatorname{im}N=1$. The restriction of the nilpotent map $N$ to this invariant line is zero, so $N^2=0$. Choose $v_3$ with $v_2=Nv_3\ne0$, and choose $v_1\in\ker N$ independent of $v_2$. Then $v_3\notin\ker N$, so these three vectors form a [basis](../../../../basis.md); its [matrix](../../../../matrix.md) for $T$ is the printed $J_1(1)\oplus J_2(1)$.

If $d=1$, then $\operatorname{im}N$ has [dimension](../../../../dimension-vector-space.md) two, so $N^2$ cannot vanish: otherwise $\operatorname{im}N\subseteq\ker N$. Choose $v_3$ with $N^2v_3\ne0$ and set $v_2=Nv_3$, $v_1=N^2v_3$. Applying $N^2$ and then $N$ to a putative linear relation proves these three vectors independent. The [matrix](../../../../matrix.md) is the printed $J_3(1)$.

These cases exhaust the possible [eigenspace](../../../../eigenspace.md) dimensions. They are pairwise dissimilar because similarity preserves the [eigenspace](../../../../eigenspace.md) [dimension](../../../../dimension-vector-space.md), equivalently the three different minimal [polynomials](../../../../polynomial-split.md). Hence every [matrix](../../../../matrix.md) is similar to **exactly one** of the three displayed forms.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [2008 printed variant](../../../2008-printed-variant-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
