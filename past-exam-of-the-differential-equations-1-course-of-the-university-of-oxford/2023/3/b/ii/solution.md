<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every real $r$ and integer $n\geq1$, $|\sin r|\leq\min(1,|r|)$ gives

$$
r\sin^n r\leq |r|\,|\sin r|^n\leq |r|\,|\sin r|\leq r^2.
$$

This estimate covers both even and odd $n$, without any assumption on the sign of $u$. Since $a(t)\geq0$, the [energy estimate](../../../../../energy-estimate.md) from part (i) becomes

$$
E'(t)\leq2a(t)E(t),\qquad E(0)=0.
$$

Equivalently, an [integrating factor](../../../../../integrating-factor.md) gives

$$
\frac d{dt}\left[e^{-2\int_0^t a(s)\,ds}E(t)\right]\leq0.
$$

The bracket is nonnegative and starts at zero, so it vanishes identically. This is also the zero-data case of the [Gronwall inequality](../../../../../gronwall-inequality.md). The vanishing [L2 norm](../../../../../l2-norm.md) and continuity of $u$ imply

$$
\boxed{u(x,t)\equiv0.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
