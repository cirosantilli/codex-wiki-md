<h1 id="analysis/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Morera's theorem](../../../../../morera-s-theorem.md) states that if $f$ is continuous on an open set $U$ and its integral around every triangle whose interior and boundary lie in $U$ is zero, then $f$ is holomorphic on $U$.

For a proof, choose a disk $B\subseteq U$ and a base point $z_0\in B$. Define $F(z)=\int_{[z_0,z]}f(\zeta)\,d\zeta$ along the straight segment. Convexity keeps every triangle with vertices $z_0,z,z+h$ inside $B$. Its zero boundary integral implies

$$
F(z+h)-F(z)=\int_{[z,z+h]}f(\zeta)\,d\zeta
=h\int_0^1f(z+th)\,dt.
$$

By continuity, the last integral tends to $f(z)$ as $h\to0$, so $F'(z)=f(z)$. Thus $F$ is holomorphic on $B$. The allowed result that the [derivative](../../../../../derivative.md) of a [holomorphic function](../../../../../holomorphic-function-split.md) is holomorphic now gives that $f=F'$ is holomorphic there. Such disks cover $U$, proving

$$
\boxed{f\text{ is holomorphic on }U.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Analysis](../../../analysis.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
