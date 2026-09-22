<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In a thin [boundary layer](../../../../../boundary-layer.md), take streamwise [velocity](../../../../../velocity.md) and distance to be order one, set $z=\delta\zeta$, and use [incompressibility](../../../../../incompressible-flow.md) to set $w=\delta W$. The streamwise [convective acceleration](../../../../../convective-acceleration.md) is order one, whereas its dominant viscous contribution after division by the [Reynolds number](../../../../../reynolds-number.md) is $\mathrm{Re}^{-1}\delta^{-2}u_{\zeta\zeta}$. Their [dominant balance](../../../../../dominant-balance.md) selects

$$
\boxed{\delta=\mathrm{Re}^{-1/2}.}
$$

With this choice, the exact rescaled [Navier-Stokes equations](../../../../../navier-stokes-equation.md) are

$$
\begin{aligned}
u_x+W_\zeta&=0,\\
u u_x+W u_\zeta&=-p_x+u_{\zeta\zeta}+\delta^2u_{xx},\\
\delta^2(uW_x+WW_\zeta)&=-p_\zeta+\delta^2W_{\zeta\zeta}+\delta^4W_{xx}.
\end{aligned}
$$

Thus the leading [pressure](../../../../../pressure-split.md) is independent of $\zeta$. Matching it to the [outer solution](../../../../../outer-expansion.md) from part (a), evaluated near $z=0$, gives $p=p_*-x^2/2$, hence $-p_x=x$. The leading [boundary-layer equation](../../../../../boundary-layer-equation.md) is therefore

$$
\boxed{u_x+W_\zeta=0,\qquad
u u_x+W u_\zeta=x+u_{\zeta\zeta},\qquad \zeta<0.}
$$

The exact surface [shear stress](../../../../../shear-stress.md) condition rescales to $u_\zeta+\delta^2W_x=\delta\beta x=\gamma x$. Since $W(x,0)=0$ for all $x$, its tangential [derivative](../../../../../derivative.md) also vanishes there. The leading surface [boundary conditions](../../../../../boundary-condition.md) are

$$
\boxed{W(x,0)=0,\qquad u_\zeta(x,0)=\gamma x.}
$$

Matching to the [outer solution](../../../../../outer-expansion.md) requires

$$
u(x,\zeta)\longrightarrow x\quad(\zeta\to-\infty),
\qquad W(x,\zeta)\sim-\zeta\quad(\zeta\to-\infty).
$$

The second matching condition specifies the leading growth of $W$, allowing a constant displacement correction. Requiring $W+\zeta\to0$ would impose an extra condition not supplied by the leading [outer solution](../../../../../outer-expansion.md). This is the [stress-driven stagnation-point boundary layer](../../../../../stress-driven-stagnation-point-boundary-layer.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
