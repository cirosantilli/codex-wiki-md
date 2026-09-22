<h1 id="12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The second equation gives $y=t+x'-x$. Differentiating it gives $y'=1+x''-x'$. Substitution into the first equation cancels the $x'$ terms and the constant forcing, leaving $x''+x=0$. Hence

$$
\boxed{x=A\cos t+B\sin t,\qquad
y=t-A(\sin t+\cos t)+B(\cos t-\sin t).}
$$

This has two independent constants, as expected for the first-order [linear system of differential equations](../../../../linear-system-of-differential-equations.md). At zero, the conditions give $A=0$ and $B=1$. Thus the required particular solution is

$$
\boxed{x=\sin t,\qquad y=t+\cos t-\sin t.}
$$

Checking directly, $x'+y'+x=\cos t+(1-\sin t-\cos t)+\sin t=1$, while $-x'+x+y=t$. This also verifies the signs introduced during elimination.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [12](../../12.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
