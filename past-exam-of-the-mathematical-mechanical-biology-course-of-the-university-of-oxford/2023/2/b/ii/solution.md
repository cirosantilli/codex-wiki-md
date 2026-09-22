<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here a prime denotes $d/d\sigma$. It is useful to retain terms through $O(\epsilon^2)$ in the normal [mechanical equilibrium](../../../../../mechanical-equilibrium.md) equation, even though only first-order shape corrections are sought. The undeformed [elastic membrane](../../../../../elastic-membrane.md) is tensionless, so a first-order change of [curvature](../../../../../curvature.md) contributes to normal force only at second order.

The geometric equations written in reference [arc length](../../../../../arc-length.md) are

$$
r'=s'\cos\theta,\qquad z'=-s'\sin\theta.
$$

Their first-order [Taylor expansions](../../../../../taylor-expansion.md) give

$$
\epsilon r_1'=-\epsilon\theta_1+O(\epsilon^2),\qquad
-1+\epsilon z_1'=-1-\epsilon s_1'+O(\epsilon^2),
$$

and hence

$$
\theta_1=-r_1',\qquad s_1'=-z_1'.
$$

The [principal stretches](../../../../../principal-stretch.md) and the first-order [constitutive equation](../../../../../constitutive-equation.md) are

$$
\lambda_s=1+\epsilon s_1'+O(\epsilon^2),\qquad
\lambda_\varphi=1+\epsilon\frac{r_1}{a_0}+O(\epsilon^2),
\qquad
\boxed{t_1=-Az_1'+\frac B{a_0}r_1.}
$$

Because $t_s=t_\varphi=t$ exactly, the tangential [mechanical equilibrium](../../../../../mechanical-equilibrium.md) equation gives $\partial_s t=0$. Thus both $t_1$ and $t_2$ are spatial constants: $t_1'=t_2'=0$.

Expand the geometric factors in the normal balance:

$$
\frac{\partial\theta}{\partial s}=\epsilon\theta_1'+O(\epsilon^2),\qquad
\frac{\sin\theta}{r}=\frac1{a_0}-\epsilon\frac{r_1}{a_0^2}+O(\epsilon^2).
$$

Consequently

$$
\epsilon p=\epsilon\frac{t_1}{a_0}
+\epsilon^2\left(t_1\theta_1'+\frac{t_2}{a_0}-\frac{t_1r_1}{a_0^2}\right)
+O(\epsilon^3).
$$

Matching the first-order coefficient gives the requested relation

$$
\boxed{p=\frac{t_1}{a_0},\qquad t_1=a_0p.}
$$

Since the prescribed [pressure](../../../../../pressure-split.md) has no second-order term, and $\theta_1'=-r_1''$, its second-order coefficient gives

$$
-t_1r_1''+\frac{t_2}{a_0}-\frac{t_1r_1}{a_0^2}=0.
$$

A closed [boundary value problem](../../../../../boundary-value-problem-split.md) for the three requested unknowns is therefore

$$
\boxed{\begin{aligned}
p a_0^2 r_1''+p r_1&=t_2,\\
A z_1'&=\frac B{a_0}r_1-a_0p,\\
t_2'&=0,
\end{aligned}\qquad
r_1(0)=r_1(L)=0,\quad z_1(0)=z_1(L)=0.}
$$

The first equation has order two, the second order one, and the last order one, so the four [boundary conditions](../../../../../boundary-condition.md) match the total order. The unknown constant $t_2$ is selected by the axial endpoint constraint, rather than by an additional specified [traction](../../../../../traction.md).

For $p\ne0$, an equivalent formulation eliminates $z_1$ and displays that constraint as an [integral](../../../../../integral-split.md):

$$
r_1''+\frac{r_1}{a_0^2}=\frac{t_2}{p a_0^2},\qquad
r_1(0)=r_1(L)=0,\qquad
\int_0^L r_1\,d\sigma=\frac{a_0^2pL}{B}.
$$

After solving this system, recover $z_1$ by [integration](../../../../../integral-split.md) from $z_1(0)=0$. No second derivatives of the unspecified function $f$ are required: they enter the next-order shape corrections through the second-order [constitutive equation](../../../../../constitutive-equation.md), whereas the displayed normal balance already determines the leading shape. The case $p=0$ has the undeformed solution $r_1=z_1=t_2=0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical mechanical biology course of the University of Oxford](../../../../split.md)
6. [Mathematical mechanical biology course of the University of Oxford](../../../../../mathematical-mechanical-biology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
