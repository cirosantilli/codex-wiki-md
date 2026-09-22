<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Seek an [even function](../../../../../even-function.md) with isolated contact at $x=0$. On $0\leq x\leq L$, the contact and reflection conditions impose $w(0)=-H$ and $w'(0)=0$, while the free interval still has $w''''=0$. Write

$$
w(x)=-H+A_2x^2+A_3x^3.
$$

The two end [boundary conditions](../../../../../boundary-condition.md) give

$$
A_2L^2+A_3L^3=H,\qquad
2A_2L+3A_3L^2=\alpha,
$$

and therefore the full [displacement field](../../../../../displacement-field-mechanics.md) is

$$
\boxed{w(x)=-H+\frac{3H-\alpha L}{L^2}x^2
+\frac{\alpha L-2H}{L^3}|x|^3.}
$$

The [jump condition](../../../../../jump-condition.md) at zero gives the upward [point force](../../../../../point-force.md)

$$
\boxed{R_0=B[w''']_0=\frac{12B}{L^3}(\alpha L-2H).}
$$

It is nonnegative precisely when $\alpha\geq2H/L$. In that range $A_3\geq0$. Nonpenetration near zero requires $A_2\geq0$, equivalently $\alpha\leq3H/L$. Conversely, when both inequalities hold,

$$
w(x)+H=x^2(A_2+A_3|x|)\geq0,
$$

with strict inequality away from zero. Thus this is an admissible isolated-contact solution throughout

$$
\boxed{\frac{2H}{L}\leq\alpha\leq\frac{3H}{L}.}
$$

At the upper endpoint the contact [curvature](../../../../../curvature.md) $w''(0)=2A_2$ vanishes, and the profile remains above the obstacle for $x\ne0$ because $A_3>0$. Increasing $\alpha$ further would make $A_2<0$, forcing penetration near zero. An interval of contact must then develop.

The admissible solution is unique within this linear model: the bending [elastic energy](../../../../../elastic-energy.md) $B\int(w'')^2/2$ is strictly convex on the [convex set](../../../../../convex-set-split.md) of admissible profiles with the prescribed end data. Integration by parts shows that a solution with nonnegative contact [point forces](../../../../../point-force.md) satisfies the corresponding minimum condition, since every admissible variation lifts a point already on the obstacle. Reflection therefore justifies the assumed [even function](../../../../../even-function.md) also after contact.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
