<h1 id="differential-equations/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the lower triangular region, the characteristic coordinates obey $-1\leq\xi<\eta\leq1$. Integrating the canonical [wave equation](../../../../../wave-equation-split.md) $u_{\xi\eta}=0$ gives

$$
u(x,y)=F(\xi)+G(\eta).
$$

On the right characteristic edge, $\eta=1$ and $x=(\xi+1)/2$, so its prescribed value gives $F(\xi)+G(1)=-\sin(\pi\xi)$. On the left edge, $\xi=-1$ and $x=(\eta-1)/2$, giving $F(-1)+G(\eta)=\sin(\pi\eta)$. At the common vertex the two values agree and equal zero; hence $F(-1)+G(1)=0$.

Adding the two edge identities and subtracting this vertex identity determines the entire solution:

$$
\boxed{u(x,y)=\sin\bigl(\pi(x-y)\bigr)-\sin\bigl(\pi(x+y)\bigr)
=-2\cos(\pi x)\sin(\pi y),\quad y<0.}
$$

The apparent freedom to add a constant to $F$ and subtract it from $G$ does not change $u$. Every classical lower-region solution has the displayed separated form, so these two characteristic boundary traces determine it uniquely. Substitution into $u_{xx}-u_{yy}=0$ and into both edge values directly verifies existence.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
