<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The forcing contains $x/y$, so matching it with a single similarity variable requires $\beta=1$. For $u=y^\alpha f(\eta)$, $\eta=x/y$, substitution gives

$$
xu_{xx}-u_y=y^{\alpha-1}[\eta f''+\eta f'-\alpha f].
$$

Matching the source $y^{-1}\eta e^{-\eta}$ selects $\boxed{\alpha=0,\ \beta=1}$ and gives $f''+f'=e^{-\eta}$. Multiplying the first-order equation for $f'$ by $e^\eta$ yields $f'=(\eta+C)e^{-\eta}$, so $f=-(\eta+1+C)e^{-\eta}+D$. The limits at zero and infinity give $D=0$, $C=-1$. Hence

$$
\boxed{u_0(x,y)=-\frac xy e^{-x/y}.}
$$

For fixed positive $x$, the initial limit is also zero because the exponential dominates $x/y$. The function $-\eta e^{-\eta}$ decreases to $-1/e$ at $\eta=1$ and increases thereafter. Therefore

$$
\boxed{\min u_0=-1/e,\qquad\text{attained at every }x=y>0.}
$$

The axis limits are zero, but there is no joint limit at $(0,0)$: approaching along $x=y$ gives $-1/e$. This does not violate any of the printed fixed-variable limits. It is this bounded [similarity solution](../../../../../similarity-solution.md) whose minimum was calculated; the unbounded corner-source additions in (b) need not have the same minimum.

## ↑ Ancestors (13)

1. [D](../d.md)
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
