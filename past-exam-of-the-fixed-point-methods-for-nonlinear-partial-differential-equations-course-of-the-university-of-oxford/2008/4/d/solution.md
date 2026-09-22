<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $u,w\in M$ both solve the [variational inequality](../../../../variational-inequality.md). Test the inequality for $u$ with $w$ and the one for $w$ with $u$, then add. Writing $d=u-w$ gives

$$
2\int_0^la|d'|^2\,dx\leq-\gamma\int_0^l(\cos u-\cos w)d\,dx\leq\gamma\|d\|_2^2,
$$

since [cosine](../../../../cosine.md) is [Lipschitz](../../../../lipschitz-continuity.md) with constant one. Since $d(0)=0$, the [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md) and [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) give $|d(x)|\leq\sqrt l\,\|d'\|_2$; integrating gives $\|d\|_2^2\leq l^2\|d'\|_2^2$. Therefore

$$
(2c_0-\gamma l^2)\|d'\|_2^2\leq0.
$$

For $\boxed{0<\gamma<2c_0/l^2}$, the coefficient is positive, so $d'=0$ and the zero boundary value gives $d=0$. This proves uniqueness with an explicit sufficient smallness condition. More generally any [Poincaré inequality](../../../../poincare-inequality.md) constant $C_P$ gives the condition $\gamma C_P^2<2c_0$; optimizing that constant is unnecessary for the requested conclusion. The underlying principle is [uniqueness for a strongly monotone variational inequality](../../../../uniqueness-for-a-strongly-monotone-variational-inequality.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
