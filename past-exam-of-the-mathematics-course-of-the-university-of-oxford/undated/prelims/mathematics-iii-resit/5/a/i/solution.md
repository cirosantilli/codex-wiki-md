<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the homogeneous [linear recurrence relation](../../../../../../../linear-recurrence-relation.md), try $u_n=r^n$. Its [characteristic equation of a linear recurrence](../../../../../../../characteristic-equation-of-a-linear-recurrence.md) is

$$
r^2+3r-4=(r-1)(r+4)=0.
$$

The distinct [roots of a polynomial](../../../../../../../root-of-a-polynomial.md) $1,-4$ give the complementary terms $A+B(-4)^n$. A constant cannot absorb the forcing because $1$ is already a [root of a polynomial](../../../../../../../root-of-a-polynomial.md) of the characteristic equation; try a [particular solution](../../../../../../../particular-solution.md) $cn$. Substitution gives $c=-4c+1$, hence $c=1/5$. The [general solution](../../../../../../../general-solution.md) is $u_n=A+B(-4)^n+n/5$.

The [initial conditions](../../../../../../../initial-condition.md) give $A+B=0$ and $A-4B=4/5$. Hence $A=4/25$, $B=-4/25$, and

$$
\boxed{u_n=\frac n5+\frac4{25}\bigl(1-(-4)^n\bigr),\qquad n\ge0.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
