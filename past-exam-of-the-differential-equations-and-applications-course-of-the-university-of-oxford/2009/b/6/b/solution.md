<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The stated pointwise boundary limits do not imply uniqueness.** A counterexample to homogeneous uniqueness is

$$
\boxed{w(x,y)=\frac{x}{y^2}e^{-x/y}\ne0.}
$$

It is smooth for $x,y>0$. Writing $\eta=x/y$, differentiation gives

$$
xw_{xx}=\frac{\eta(\eta-2)}{y^2}e^{-\eta}=w_y.
$$

For fixed positive $y$, $w\to0$ as $x\to0$ and as $x\to\infty$; for fixed positive $x$, it also tends to zero as $y\downarrow0$. Thus if $u_0$ is one solution, $u_0+Cw$ satisfies the same equation and every printed boundary limit for any constant $C$. Part (d) supplies such a particular solution, so this is a genuine family of distinct solutions, not merely a formal obstruction.

This is [corner-source nonuniqueness for a degenerate parabolic problem](../../../../../corner-source-nonuniqueness-for-a-degenerate-parabolic-problem.md). The peak $w(y,y)=1/(ey)$ diverges towards the missing corner $(0,0)$; pointwise initial limits at each fixed $x>0$ do not exclude it. The preceding maximum argument fails to force uniqueness because a supremum over an entire past strip need not be attained or finite.

A customary bounded-solution condition restores the intended result. If the difference $z$ of two solutions is bounded on every finite time strip, subtract $\delta(1+x+y)$. Its operator $x\partial_x^2-\partial_y$ equals $\delta>0$, excluding a positive past maximum; the linear barrier controls spatial infinity, and the homogeneous initial/boundary values control the [parabolic boundary](../../../../../parabolic-boundary.md). Letting $\delta\downarrow0$ gives $z\leq0$; applying the same argument to $-z$ gives $z=0$. This proves uniqueness in that additional bounded class, which the printed pointwise limits alone do not specify.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
