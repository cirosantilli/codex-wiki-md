<h1 id="12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $f(x,y)=F(u,v)$ in the proposed local coordinates. The [multivariable chain rule](../../../../../multivariable-chain-rule.md) gives

$$
f_x=2xF_u+2yF_v,\qquad f_y=-2yF_u+2xF_v.
$$

Consequently

$$
yf_x+xf_y=2(x^2+y^2)F_v=0.
$$

Away from the origin the [Jacobian determinant](../../../../../jacobian-determinant.md) is $u_xv_y-u_yv_x=4(x^2+y^2)>0$, so the [inverse function theorem](../../../../../inverse-function-theorem.md) justifies these local coordinates. Therefore $F_v=0$ and the local [general solution](../../../../../general-solution.md) is

$$
\boxed{f(x,y)=\Phi(x^2-y^2).}
$$

Substitution verifies the result: $f_x=2x\Phi'$ and $f_y=-2y\Phi'$, whose weighted sum vanishes.

There is a global qualification. The coordinate map is two-to-one, and a [level set](../../../../../level-set.md) of $x^2-y^2$ has separate [characteristic curve](../../../../../characteristic-curve.md) branches. A single profile on the entire plane does not follow without a branch-identification assumption. For example, take $f=\exp[-1/(x^2-y^2)^2]$ on the wedge $x>0$, $x^2>y^2$, and zero elsewhere. This is smooth, satisfies the equation, and has different values at $(1,0)$ and $(-1,0)$ despite equal $u$. The [characteristic components of a hyperbolic first-order equation](../../../../../characteristic-components-of-a-hyperbolic-first-order-equation.md) explain this obstruction. At the origin the coordinate map is singular and the original equation reads $0=0$; the boxed answer is the intended local form on a regular branch, or a global form under an additional identification of branches.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
