<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Adjoin $\mu_{n+1}=\mu_n$. At the origin the stable direction is the $x$ axis, with [Floquet multiplier](../../../../floquet-multiplier.md) zero, while the $y$ and parameter directions have [Floquet multiplier](../../../../floquet-multiplier.md) one. By the [centre manifold theorem for a discrete dynamical system](../../../../centre-manifold-theorem-for-a-discrete-dynamical-system.md), write the [extended centre manifold](../../../../extended-centre-manifold-for-a-parameter.md) as

$$
x=h(y,\mu),\qquad h(0,0)=0,\qquad Dh(0,0)=0.
$$

On it the scalar map is $Y=(1+\mu)y-\mu h(y,\mu)+y^3$. Its discrete [centre-manifold invariance equation](../../../../centre-manifold-invariance-equation.md) is

$$
h(Y,\mu)=\mu y.
$$

Put $h=h_2+O(\rho^3)$ with $\rho=|y|+|\mu|$. Since $Y=y+O(\rho^2)$, the quadratic equation is simply $h_2(y,\mu)=\mu y$. Thus

$$
\boxed{x=\mu y+O(\rho^3).}
$$

In particular, setting the stable variable identically to zero would lose the leading parameter correction. The reduced map through total degree three is

$$
\boxed{y_{n+1}=y_n+\mu y_n-\mu^2y_n+y_n^3+O(\rho^4).}
$$

In the natural [pitchfork bifurcation](../../../../pitchfork-bifurcation-normal-form.md) scaling $\mu=O(y^2)$ this has leading form $y_{n+1}=y_n+\mu y_n+y_n^3$. Its nonzero [fixed points](../../../../fixed-point.md) satisfy $y^2\sim-\mu$, and their reduced [fixed-point multipliers](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) satisfy $1-2\mu+O(\mu^2)>1$ for small $\mu<0$. The transverse [Floquet multiplier](../../../../floquet-multiplier.md) remains inside the [unit circle](../../../../complex-unit-circle.md). Therefore **the [bifurcation](../../../../bifurcation.md) at $\mu=0$ is a [subcritical pitchfork bifurcation](../../../../subcritical-pitchfork-bifurcation.md): the origin attracts for small negative $\mu$, each nonzero branch is a [saddle fixed point of a map](../../../../saddle-fixed-point-of-a-map.md), and the origin is a [saddle fixed point of a map](../../../../saddle-fixed-point-of-a-map.md) for small positive $\mu$**.

An exact check uses the full [Jacobian matrix](../../../../jacobian-matrix.md) on either nonzero branch. Its [trace](../../../../matrix-trace.md) is $T_*=1-2\mu+3\mu^2$ and its [determinant](../../../../determinant.md) is $D_*=\mu^2$. Thus

$$
p_*(1)=1-T_*+D_*=2\mu(1-\mu)<0
$$

whenever a nonzero branch exists. Also $p_*(0)=\mu^2>0$, so one real [Floquet multiplier](../../../../floquet-multiplier.md) lies in $(0,1)$ and the other in $(1,\infty)$. This proves that each nonzero branch is a [saddle fixed point of a map](../../../../saddle-fixed-point-of-a-map.md) throughout $\mu<0$ and $\mu>1$, in particular near the requested [bifurcation](../../../../bifurcation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the nonlinear systems course of the University of Oxford](../../../split.md)
5. [Nonlinear systems course of the University of Oxford](../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
