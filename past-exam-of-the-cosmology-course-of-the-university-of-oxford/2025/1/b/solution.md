<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce the positive [dimensionless quantity](../../../../dimensionless-quantity.md) $x=(1-\Omega)a/\Omega$ and the time scale $A=\Omega/[H_0(1-\Omega)^{3/2}]$. The [Friedmann equation](../../../../friedmann-equations.md) gives the separable relation

$$
dt=\frac{da}{aH(a)}=A\sqrt{\frac{x}{1+x}}\,dx.
$$

For $x=(\cosh\theta-1)/2=\sinh^2(\theta/2)$, $\theta\geq0$, the [hyperbolic function](../../../../hyperbolic-function.md) identities give

$$
\sqrt{\frac{x}{1+x}}\,dx
=\tanh\frac\theta2\,\frac{\sinh\theta}{2}\,d\theta
=\frac{\cosh\theta-1}{2}\,d\theta.
$$

Choose the [constant of integration](../../../../constant-of-integration.md) so that $t=0$ at $a=0$. The resulting [parametric equation](../../../../parametric-equation.md) for the [open matter-dominated Friedmann solution](../../../../open-matter-dominated-friedmann-solution.md) is

$$
\boxed{t=\frac{\Omega}{2H_0(1-\Omega)^{3/2}}(\sinh\theta-\theta),\qquad a=\frac{\Omega}{2(1-\Omega)}(\cosh\theta-1).}
$$

For $\theta\ll1$, the [Taylor series](../../../../taylor-series.md) give

$$
t=\frac{\Omega\theta^3}{12H_0(1-\Omega)^{3/2}}[1+O(\theta^2)],\qquad a=\frac{\Omega\theta^2}{4(1-\Omega)}[1+O(\theta^2)].
$$

Eliminating $\theta$ yields $a^{3/2}\simeq(3/2)H_0\sqrt\Omega\,t$, exactly the early [matter-dominated universe](../../../../matter-domination.md) result. For $\theta\gg1$, $\sinh\theta\sim\cosh\theta\sim e^\theta/2$, whereas $\theta/e^\theta\to0$. The [ratio](../../../../ratio.md) of the two parametric expressions tends to $a/t=H_0\sqrt{1-\Omega}$, recovering the [curvature-dominated universe](../../../../curvature-dominated-universe.md) result including its coefficient.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the cosmology course of the University of Oxford](../../../split.md)
5. [Cosmology course of the University of Oxford](../../../../cosmology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
