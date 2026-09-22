<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the aspect ratio and the thickness-based [Reynolds number](../../../../../reynolds-number.md) by

$$
\boxed{\varepsilon=\frac{h_0}{L}\ll1,\qquad
\mathrm{Re}=\frac{\rho U_0h_0}{\mu}.}
$$

Use the [nondimensionalization](../../../../../nondimensionalization.md)

$$
x=Lx_*,\quad z=h_0z_*,\quad t=\frac L{U_0}t_*,\quad
u=U_0u_*,\quad w=\varepsilon U_0w_*,\quad
p=p_a+\rho gh_0\sin\alpha\,p_*.
$$

The small transverse [velocity](../../../../../velocity.md) scale follows from [incompressibility](../../../../../incompressible-flow.md). Dropping stars, the base fields become $\bar u=2z-z^2$ and $\bar p=(1-z)\cot\alpha$. Before subtracting the base state, the dimensionless [Navier-Stokes equation](../../../../../navier-stokes-equation.md) reads

$$
\begin{aligned}
u_x+w_z&=0,\\
\mathrm{Re}\,\varepsilon(u_t+uu_x+wu_z)
&=-2\varepsilon p_x+u_{zz}+\varepsilon^2u_{xx}+2,\\
\mathrm{Re}\,\varepsilon^2(w_t+uw_x+ww_z)
&=-2p_z+\varepsilon(w_{zz}+\varepsilon^2w_{xx})-2\cot\alpha.
\end{aligned}
$$

For example, division of the downslope momentum equation by $\mu U_0/h_0^2$ makes the inertial coefficient $\rho U_0h_0^2/(\mu L)=\mathrm{Re}\,\varepsilon$ and the [pressure gradient](../../../../../pressure-gradient.md) coefficient $2\varepsilon$. The transverse equation has been divided instead by $\mu U_0/h_0^2$ after using its smaller [velocity](../../../../../velocity.md) scale; this gives the displayed $\mathrm{Re}\,\varepsilon^2$ coefficient.

Now substitute $u=\bar u+\hat u$, $w=\hat w$, $p=\bar p+\hat p$. Since $\bar u_{zz}+2=0$, $\bar p_z=-\cot\alpha$, and the base fields have no $x$ or $t$ dependence, subtraction gives

$$
\boxed{\begin{aligned}
\hat u_x+\hat w_z&=0,\\
\mathrm{Re}\,\varepsilon[\hat u_t+(\bar u+\hat u)\hat u_x+\hat w(\bar u_z+\hat u_z)]
&=-2\varepsilon\hat p_x+\hat u_{zz}+\varepsilon^2\hat u_{xx},\\
\mathrm{Re}\,\varepsilon^2[\hat w_t+(\bar u+\hat u)\hat w_x+\hat w\hat w_z]
&=-2\hat p_z+\varepsilon(\hat w_{zz}+\varepsilon^2\hat w_{xx}).
\end{aligned}}
$$

These are nonlinear equations for the deviations; small [amplitude](../../../../../wave-amplitude.md) has not been assumed. The later [asymptotic expansion](../../../../../asymptotic-expansion-split.md) takes $\mathrm{Re}=O(1)$ as $\varepsilon\to0$, or more generally requires the retained inertial correction to remain small.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
