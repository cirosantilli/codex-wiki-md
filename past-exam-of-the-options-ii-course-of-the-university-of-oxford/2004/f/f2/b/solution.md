<h1 id="f/f2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Positive definiteness](../../../../../positive-definiteness.md) gives a positive smallest [eigenvalue](../../../../../eigenvalue.md) $c$ with $x^tAx\geq c|x|^2$. Hence the set $x^tAx=y^tAy=1$ is [compact](../../../../../compact-space.md), and $h$ attains a maximum there. Its two constraint gradients are $(2Ax,0)$ and $(0,2Ay)$; they are [linearly independent](../../../../../linear-independence.md) because $x,y$ are nonzero and $A$ is invertible.

Put $s=x^tAy$. At any constrained extremum the multiplier equations are

$$
sAy=\lambda Ax,\qquad sAx=\mu Ay.
$$

Multiplication by $x^t$ and $y^t$ gives $\lambda=\mu=s^2$. If $s=0$ the objective is zero. Otherwise $Ay=sAx$, so $y=sx$ and normalization gives $s^2=1$. Thus every maximum is at most one, and the value one is attained at $x=y$. This proves $\boxed{(x^tAy)^2\leq1}$ on the normalized constraints.

For nonzero arbitrary vectors apply that result to $x/\sqrt{x^tAx}$ and $y/\sqrt{y^tAy}$. If either vector is zero the conclusion is immediate. Therefore

$$
\boxed{(x^tAy)^2\leq(x^tAx)(y^tAy).}
$$

Equality for nonzero vectors holds precisely when they are [linearly dependent](../../../../../linear-dependence.md). This is the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) for the [inner product](../../../../../inner-product-split.md) induced by $A$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
