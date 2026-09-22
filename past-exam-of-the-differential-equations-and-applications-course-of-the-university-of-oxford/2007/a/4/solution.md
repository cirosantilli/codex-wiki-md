<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

With [diffusion](../../../../diffusion.md) absent, the [characteristic equations for a first-order quasilinear equation](../../../../characteristic-equations-for-a-first-order-quasilinear-equation.md) are $du/dt=0$, $dx/dt=q'(u)$. A [characteristic curve](../../../../characteristic-curve.md) labelled by its starting point $s$ is

$$
\boxed{u=u_0(s),\quad x=s+tq'[u_0(s)],\qquad
u(x,t)=u_0\!\left(x-tq'[u(x,t)]\right).}
$$

This determines a smooth single-valued solution while $s\mapsto x$ is one-to-one. Its [derivative](../../../../derivative.md) is

$$
u_x=\frac{u_0'(s)}{1+tq''[u_0(s)]u_0'(s)}.
$$

All [characteristic curves](../../../../characteristic-curve.md) move right because $q'>0$. Because $q''<0$, increasing portions of the initial profile have slower [characteristic curves](../../../../characteristic-curve.md) ahead than behind, so they steepen. The first positive [gradient catastrophe](../../../../gradient-catastrophe.md) occurs at

$$
\boxed{t_* =\inf_{s:u_0'(s)>0}\frac{-1}{u_0'(s)q''[u_0(s)]}.}
$$

This is a minimum when attained. The numerator at such a point is positive and the denominator decreases to zero from above, so $u_x\to+\infty$.

Resolve the thin transition with $X=(x-x_s(t))/\epsilon$ and $u\simeq U(X)$. The leading balance is $(-c+q'(U))U'=(D(U)U')'$, where $c=\dot x_s$. Integrating once and matching to the state behind gives

$$
\boxed{D(U)U'=F(U)=q(U)-q(u_-)-c(U-u_-).}
$$

Matching the state ahead requires $F(u_+)=0$ and gives the Rankine-Hugoniot speed

$$
\boxed{c=\frac{q(u_+)-q(u_-)}{u_+-u_-}.}
$$

The strictly [concave](../../../../concave-function.md) graph of $F$ has zeros at the two states and lies above its chord, hence is strictly positive between them. Since $D>0$, $U'>0$ through the layer. A heteroclinic profile increasing with $X$ can therefore connect the rear state at $X=-\infty$ to the front state at $X=+\infty$ only when $\boxed{u_-<u_+}$. The [concavity](../../../../concave-function.md) also gives $q'(u_-)>c>q'(u_+)$: [characteristic curves](../../../../characteristic-curve.md) enter the [viscous shock](../../../../viscous-shock.md) from both sides. Reversing the states would demand a decreasing profile, contradicting the sign of $F/D$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
