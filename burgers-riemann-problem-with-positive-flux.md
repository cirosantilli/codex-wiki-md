# Burgers Riemann problem with positive flux

↑ **Parent:** [Inviscid Burgers equation](inviscid-burgers-equation.md)

Consider the [Riemann problem](riemann-problem.md) on $\mathbb R$ with [initial condition](initial-condition.md) $u_0(x)=u_L$ for $x<0$ and $u_0(x)=u_R$ for $x>0$. No endpoint [boundary conditions](boundary-condition.md) are imposed. When $u_L>u_R$, its [entropy solution](entropy-solution.md) is a [shock wave](shock-wave.md) with constant speed $s=(u_L+u_R)/2$. In the original example $u_L=2$, $u_R=0$, the [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) gives

$$
s=\frac{f(u_R)-f(u_L)}{u_R-u_L}=\frac{0-2}{0-2}=1,\qquad u(x,t)=\begin{cases}2,&x<t,\\0,&x>t.\end{cases}
$$

The left [characteristic speed](characteristic-speed.md) is $2$ and the right [characteristic speed](characteristic-speed.md) is $0$, so $2>1>0$: both sides enter the [entropy shock](entropy-shock.md). The [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md) gives an exact smooth family tending to this solution.

Reversing the states to $u_L=0$, $u_R=2$ still gives a [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) speed of $1$, but now [characteristic curves](characteristic-curve.md) move away from the discontinuity. That expansion jump is a [weak solution](weak-solution.md) and fails entropy admissibility. For general $u_L<u_R$, the selected [entropy solution](entropy-solution.md) is the continuous [self-similar solution](similarity-solution.md)

$$
u(x,t)=\begin{cases}u_L,&x\leq u_Lt,\\x/t,&u_Lt<x<u_Rt,\\u_R,&x\geq u_Rt,\end{cases}\qquad t>0.
$$

This [rarefaction wave](rarefaction-wave.md) fills the expanding gap between the two exterior [characteristic curves](characteristic-curve.md). Inside its fan, $u_t=-x/t^2$ and $uu_x=x/t^2$, verifying the [Inviscid Burgers equation](inviscid-burgers-equation.md); its values agree continuously with both exterior states. For $0$ to $2$, the fan occupies $0<x<2t$. If $u_L=u_R$, the solution is constant.[Rarefaction wave, full piecewise solution; expansion-shock example; The entropy condition](riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo/burgers-equation.md)

## ↑ Ancestors (8)

1. [Inviscid Burgers equation](inviscid-burgers-equation.md)
2. [Scalar conservation law](scalar-conservation-law.md)
3. [Transport equation](transport-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Burgers' equation](burgers-equation.md)
- [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md)
