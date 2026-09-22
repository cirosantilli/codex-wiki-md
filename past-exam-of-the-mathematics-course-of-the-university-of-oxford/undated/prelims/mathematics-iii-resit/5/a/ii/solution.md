<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The homogeneous [characteristic equation of a linear recurrence](../../../../../../../characteristic-equation-of-a-linear-recurrence.md) is

$$
r^2+2r+1=(r+1)^2=0.
$$

The [repeated characteristic root of a linear recurrence](../../../../../../../repeated-characteristic-root-of-a-linear-recurrence.md) $-1$ supplies the independent terms $(-1)^n$ and $n(-1)^n$. A constant [particular solution](../../../../../../../particular-solution.md) is $1/2$, since $1/2=-2(1/2)-1/2+2$. Thus $u_n=1/2+(A+Bn)(-1)^n$.

**The scan prints $u_2=0$, not $u_1=0$. These [initial conditions](../../../../../../../initial-condition.md) are consistent.** They give $A=1/2$ from $u_0=1$, then $0=1/2+A+2B$, so $B=-1/2$. Therefore

$$
\boxed{u_n=\frac12+\frac{1-n}{2}(-1)^n.}
$$

In particular $u_1=1/2$ and $u_2=0$. Direct substitution verifies the [recurrence relation](../../../../../../../recurrence-relation.md). This is an example of [nonconsecutive initial values for a linear recurrence](../../../../../../../nonconsecutive-initial-values-for-a-linear-recurrence.md); replacing the printed subscript by 1 would change the answer.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
