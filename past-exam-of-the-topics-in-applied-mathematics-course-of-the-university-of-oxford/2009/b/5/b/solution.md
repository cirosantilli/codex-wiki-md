<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A genuine [two-cycle](../../../../../period-two-orbit.md) must have the form $(x,y)\mapsto(y,x)$ with $x\ne y$. Hence $a(x-x^3/3)=x+y=a(y-y^3/3)$. Subtracting gives

$$
x^2+xy+y^2=3.
$$

Let $S=x+y$ and $P=xy$. Using $x^3=3x-PS$ in either original equation gives $S(aP/3-1)=0$. The [cubic swap-map two-cycle factorization](../../../../../cubic-swap-map-two-cycle-factorization.md) exhibits two cases, so cancellation of $S$ would lose an actual branch.

If $S\ne0$, then $P=3/a$ and $S^2=3+3/a$. Thus the source's quadratic holds for this family, with

$$
\boxed{A=S=\pm\sqrt{3+3/a},\qquad X_\pm=\frac{A\pm\sqrt{3-9/a}}2.}
$$

There are two reflected genuine cycles for $a>3$, coalescing with the [fixed points](../../../../../fixed-point.md) $p=\pm1$ at $a=3$. For their two-step [Jacobian matrix](../../../../../jacobian-matrix.md), $\operatorname{tr}DF^2=4-a$ and $\det DF^2=-2a^2+3a+9$. The unit-disk necessary inequality $1-\operatorname{tr}DF^2+\det DF^2>0$ fails, since it is $-2(a-3)(a+1)<0$. Therefore **these quadratic-family cycles are unstable for every $a>3$**. For these [unstable asymmetric cycles of a cubic swap map](../../../../../unstable-asymmetric-cycles-of-a-cubic-swap-map.md), their [periodic-orbit multipliers](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are real: one exceeds $1$, while the other crosses $-1$ at $a=(1+\sqrt{29})/2$. They are saddles before that secondary threshold and repelling beyond it. Their presence on the stable side of the fixed-point flip identifies the unstable branch of a subcritical flip.

If $S=0$, then $y=-x$ and the preceding quadratic identity gives $x^2=3$. Hence there is also the exact cycle

$$
\boxed{(\sqrt3,-\sqrt3)\ \longleftrightarrow\ (-\sqrt3,\sqrt3),\qquad\text{for every }a>0.}
$$

This [antipodal cycle of a cubic swap map](../../../../../antipodal-cycle-of-a-cubic-swap-map.md) does not satisfy the printed $P=3/a$ condition: its product is $-3$. Along it the one-step [Jacobian matrix](../../../../../jacobian-matrix.md) is the same [matrix](../../../../../matrix.md) $B=\left(\begin{smallmatrix}0&1\\-2a&-1\end{smallmatrix}\right)$ at both points, so the cycle [periodic-orbit multipliers](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are the squares of the roots of $\lambda^2+\lambda+2a=0$. The [Jury stability criterion](../../../../../jury-stability-criterion.md) conditions give

$$
\boxed{\text{antipodal cycle attracting for }0<a<1/2,\quad\text{repelling for }a>1/2.}
$$

At $a=1/2$ its [periodic-orbit multipliers](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are on the unit circle and [linearization](../../../../../linearization.md) is inconclusive. Its real-to-complex transition occurs at $a=1/8$. Thus the printed assertion about all period-two components is incomplete: it describes only $S\ne0$, whereas the omitted antipodal cycle supplies the actual stable period-two interval.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
