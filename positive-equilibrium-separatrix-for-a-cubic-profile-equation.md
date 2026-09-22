# Positive-equilibrium separatrix for a cubic profile equation

↑ **Parent:** [First integral](first-integral.md)

Multiply the [ordinary differential equation](ordinary-differential-equation.md) by $f'$ and integrate. A solution approaching the positive [equilibrium](equilibrium-point-of-a-dynamical-system.md) $a$ has $f'\to0$: this follows from the equation and convergence of $f$, since a nonzero limiting derivative or energy would preclude convergence. Its [first integral](first-integral.md) is therefore

$$
\frac12(f')^2=\frac14(f^2-a^2)^2.
$$

The branch tending to $a$ at positive infinity obeys $f'=(a^2-f^2)/\sqrt2$. Separation yields

$$
f(\eta)=a\frac{1-Ae^{-\sqrt2a\eta}}{1+Ae^{-\sqrt2a\eta}}.
$$

The constant solution is $A=0$. For $A>0$ this is a translated [hyperbolic tangent](hyperbolic-tangent.md); for $-1<A<0$ it is a regular [hyperbolic cotangent](hyperbolic-cotangent.md) branch on $\eta\geq0$. The condition $A>-1$ excludes both an interior pole and a divergent value at the finite endpoint. The opposite sign in the first integral moves away from the positive [equilibrium](equilibrium-point-of-a-dynamical-system.md) as $\eta$ increases, except at the constant solution.

A useful integral consequence is

$$
\int_0^\infty[a-f(\eta)]\,d\eta=\sqrt2\log(1+A).
$$

Indeed the integrand is $2aAe^{-\sqrt2a\eta}/(1+Ae^{-\sqrt2a\eta})$, the negative of $\sqrt2$ times the derivative of $\log(1+Ae^{-\sqrt2a\eta})$. An integral deficit can therefore fix the translation parameter uniquely, even when the differential equation and far value leave it free.

## ↑ Ancestors (7)

1. [First integral](first-integral.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2008/b/8/solution.md)
