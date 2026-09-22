# Viscous Burgers travelling shock

↑ **Parent:** [Viscous Burgers equation](viscous-burgers-equation.md)

A [travelling wave](travelling-wave.md) of the [viscous Burgers equation](viscous-burgers-equation.md) can connect constant states $u_L>u_R$ through a smooth decreasing layer. Require $u(x,t)=U(z)$, $z=x-st$, $U(-\infty)=u_L$, $U(+\infty)=u_R$, and $U'\to0$ at both ends. Substitution and one [integration](integral-split.md) give

$$
(U-s)U'=\nu U'',\qquad \nu U'=\frac12(U-u_L)(U-u_R),\qquad s=\frac{u_L+u_R}{2}.
$$

The speed follows by evaluating the integration constant at both end states. It is precisely the [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) for [conservation law flux](conservation-law-flux.md) $f(u)=u^2/2$. Choosing the center $U(0)=s$ gives the displayed [hyperbolic tangent](hyperbolic-tangent.md) profile. Its characteristic width scales as $\nu/(u_L-u_R)$; a smaller positive $\nu$ makes a thinner smooth layer.

For an original worked example in [dimensionless quantities](dimensionless-quantity.md), take $u_L=2$, $u_R=0$ and $s=1$:

$$
u(x,t)=1-\tanh\frac{x-t}{2\nu}=\frac{2}{1+\exp((x-t)/\nu)}.
$$

This is an exact [classical solution](classical-solution.md) on $\mathbb R$ with its own smooth [initial condition](initial-condition.md) $u(x,0)=1-\tanh(x/(2\nu))$ and limiting states $2,0$. It is a family of moving profiles, not the finite-$\nu$ solution starting from an exact discontinuous step. For that different [initial condition](initial-condition.md), the [Cole-Hopf transformation](cole-hopf-transformation.md) supplies the evolution. At $\nu=1/2$, this front starts from the same $1-\tanh x$ profile as the [Burgers characteristic breaking](burgers-characteristic-breaking.md) example: positive [diffusion](diffusion.md) maintains a smooth moving layer while the inviscid profile breaks at $t=1$.

To check the [partial differential equation](partial-differential-equation-split.md) explicitly, set $w=(x-t)/(2\nu)$ and $S=1-\tanh^2w$. Then

$$
u_t=\frac{S}{2\nu},\qquad u_x=-\frac{S}{2\nu},\qquad u_{xx}=\frac{S\tanh w}{2\nu^2},\qquad u_t+uu_x=\frac{S\tanh w}{2\nu}=\nu u_{xx}.
$$

The independent [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) check gives $s=(0-2)/(0-2)=1$, using $f(2)=2$ and $f(0)=0$. At fixed $x\ne t$, the [vanishing viscosity approximation](vanishing-viscosity-approximation.md) tends to the [entropy shock](entropy-shock.md) $2$ for $x<t$ and $0$ for $x>t$. At the center the smooth profiles stay at $1$; changing the value on the discontinuity does not change the limiting [weak solution](weak-solution.md).

<a id="image-exact-viscous-fronts-from-2-to-0-the-speed-stays-1-while-the-layer-narrows-with-viscosity"></a>
![](burgers-viscous-travelling-shock.png)

**[Figure 2](#image-exact-viscous-fronts-from-2-to-0-the-speed-stays-1-while-the-layer-narrows-with-viscosity). Exact viscous fronts from 2 to 0: the speed stays 1 while the layer narrows with viscosity**.

For $u_L<u_R$, the same integrated [ordinary differential equation](ordinary-differential-equation.md) has $U'<0$ between the two states when $\nu>0$, so it cannot supply an increasing connecting front. The inviscid admissible expansion is the [rarefaction wave](rarefaction-wave.md) of the [Burgers Riemann problem with positive flux](burgers-riemann-problem-with-positive-flux.md).

## ↑ Ancestors (7)

1. [Viscous Burgers equation](viscous-burgers-equation.md)
2. [Burgers' equation](burgers-equation.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Burgers' equation](burgers-equation.md)
- [Burgers Riemann problem with positive flux](burgers-riemann-problem-with-positive-flux.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022/section-b/5/d/solution.md)
- [Viscous Burgers equation](viscous-burgers-equation.md)
