<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $f,F$ are [continuously differentiable](../../../../../../../continuously-differentiable-function.md) near the point and $F_z\ne0$. The [implicit function theorem](../../../../../../../implicit-function-theorem.md) supplies a local [function](../../../../../../../function-split.md) $z(x,y)$ with

$$
z_x=-F_x/F_z,\qquad z_y=-F_y/F_z.
$$

At an interior [extremum](../../../../../../../maximum-and-minimum.md) of $g(x,y)=f(x,y,z(x,y))$, the [multivariable chain rule](../../../../../../../multivariable-chain-rule.md) gives

$$
0=g_x=f_x-f_zF_x/F_z,\qquad0=g_y=f_y-f_zF_y/F_z.
$$

Multiply these identities by $F_y$ and $F_x$, respectively, and subtract. The terms containing $f_z$ cancel, giving

$$
\boxed{f_xF_y-f_yF_x=0.}
$$

No assumption $f_z\ne0$ is needed for this elimination; dividing by $f_z$ would unnecessarily exclude valid cases. If $F_z=0$, this particular local graph argument is unavailable and a different chart or the full [Lagrange multiplier](../../../../../../../lagrange-multiplier.md) condition is needed.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
