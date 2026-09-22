<h1 id="s7/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $m$ be the ice mass for which the stated drag coefficients are defined, $K=k_1+k_2$ and $f=2\Omega\sin\ell$. With stationary water, the steady horizontal ice equations are

$$
0=mf v_y+k_1v_{a,x}-Kv_x,\qquad0=-mf v_x+k_1v_{a,y}-Kv_y.
$$

The [linear system](../../../../../system-of-linear-equations.md) gives

$$
v_y=\frac{k_1}{K^2+(mf)^2}\left(Kv_{a,y}-mf v_{a,x}\right).
$$

For fixed wind speed $V=10\,\mathrm{m\,s^{-1}}$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) minimizes this component when

$$
\boxed{\mathbf v_a=\frac{V}{\sqrt{K^2+(mf)^2}}(mf,-K),\qquad v_{y,\min}=-\frac{k_1V}{\sqrt{K^2+(mf)^2}}.}
$$

Thus the wind must blow towards a direction east of south by $\tan^{-1}(mf/K)$ in the northern hemisphere, west of south in the southern hemisphere, and due south at the equator. This compensates the [Coriolis force](../../../../../coriolis-force.md); at the optimum $v_x=0$ and the ice moves due south. If the drag coefficients are per unit mass, replace $K/m$ by the corresponding total drag rate. “Blows towards” avoids the opposite convention used when naming winds by their origin.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [S7](../../../s7.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
