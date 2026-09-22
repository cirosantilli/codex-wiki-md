<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The space $C([a,b])$ with the [supremum norm](../../../../../supremum-norm.md) is a [Banach space](../../../../../banach-space-split.md). Continuity of the kernel makes $K$ a [bounded linear operator](../../../../../continuous-linear-operator.md). Induction on $n$ gives

$$
A^ny=f+Kf+\cdots+K^{n-1}f+K^ny,
$$

so $A^ny-A^nz=K^n(y-z)$. The ordered integration region gives the [factorial bound for a Volterra iterate](../../../../../factorial-bound-for-a-volterra-iterate.md):

$$
|(K^ny)(t)|\leq\frac{M^n(t-a)^n}{n!}\|y\|_\infty.
$$

For completeness, if this holds at $n$, then integrating $M\,M^n(s-a)^n/n!$ from $a$ to $t$ gives the bound at $n+1$; the initial case is the defining integral. Thus

$$
\|A^ny-A^nz\|_\infty\leq\alpha_n\|y-z\|_\infty,\qquad \alpha_n=\frac{[M(b-a)]^n}{n!},
$$

and $\sum_{n\geq1}\alpha_n=e^{M(b-a)}-1<\infty$. Part (b) now gives uniform convergence of every iteration sequence to the unique [fixed point](../../../../../fixed-point.md). Since $y=Ay$ is precisely the [Volterra integral equation](../../../../../volterra-integral-equation.md), this is its unique continuous solution. No restriction $M(b-a)<1$ is needed: the factorial controls all iterates on the whole finite interval.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
