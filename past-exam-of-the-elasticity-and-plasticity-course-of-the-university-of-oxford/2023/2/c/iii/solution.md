<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let the contact interval be $[-s,s]$, where $w=-H$. Its [slope](../../../../../slope.md) and [curvature](../../../../../curvature.md) vanish. [Continuity](../../../../../continuous-function.md) of the [displacement field](../../../../../displacement-field-mechanics.md), [slope](../../../../../slope.md) and [bending moment](../../../../../bending-moment.md) at $x=s$ gives

$$
w(s)=-H,\qquad w'(s)=0,\qquad w''(s)=0.
$$

On the free interval $s<x<L$, the cubic [polynomial](../../../../../polynomial-split.md) satisfying these three conditions is $w=-H+C(x-s)^3$. Put $d=L-s$. The end [boundary conditions](../../../../../boundary-condition.md) become

$$
Cd^3=H,\qquad3Cd^2=\alpha.
$$

Consequently

$$
\boxed{d=\frac{3H}{\alpha},\qquad
s=L-\frac{3H}{\alpha},\qquad
C=\frac{H}{d^3}.}
$$

This requires $\alpha\geq3H/L$, with $s=0$ at the transition. The full [displacement field](../../../../../displacement-field-mechanics.md) is

$$
\boxed{w(x)=
\begin{cases}
-H,&|x|\leq s,\\
-H+H\left(\dfrac{|x|-s}{L-s}\right)^3,&s\leq|x|\leq L.
\end{cases}}
$$

It satisfies nonpenetration. In the open contact interval the distributed [normal contact force](../../../../../normal-contact-force.md) is $R=Bw''''=0$, since the obstacle is flat and $p=T=0$. The [normal contact force](../../../../../normal-contact-force.md) is concentrated at the two endpoints. At $x=s$, $w'''$ jumps from zero to $6H/d^3$; at $x=-s$, it jumps from $-6H/d^3$ to zero. Both upward [point forces](../../../../../point-force.md) are therefore

$$
\boxed{R_{-s}=R_s=\frac{6BH}{d^3}>0.}
$$

At $s=0$ they merge into the single midpoint [point force](../../../../../point-force.md) of the preceding regime. These formulae belong to the small-[slope](../../../../../slope.md) model; interpreting arbitrarily large $\alpha$ as a finite physical rotation would exceed its assumptions.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../../split.md)
6. [Elasticity and plasticity course of the University of Oxford](../../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
