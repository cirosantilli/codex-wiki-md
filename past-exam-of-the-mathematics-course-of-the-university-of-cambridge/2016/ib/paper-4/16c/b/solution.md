<h1 id="16c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\kappa=\sqrt{a/b}>0$. Solving the interior [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) and imposing both $V(0)=0$ and $\dot V(0)=0$ yields $V=C(\cosh\kappa t-1)$, with $\lambda=-2aC$. The distance constraint fixes

$$
\boxed{V_{\mathrm{formal}}(t)=\frac{L(\cosh\kappa t-1)}{\sinh(\kappa T)/\kappa-T}.}
$$

The denominator is positive because $\sinh z>z$ for $z>0$. This is the requested solution of the differential equation with the stated initial conditions.

**As a minimum-energy problem with free terminal speed, the printed conditions do not admit a smooth minimizer.** The formal profile has $\dot V(T)=C\kappa\sinh(\kappa T)>0$, violating the natural terminal condition from part (a). Fixing the initial acceleration restricts $\eta'(0)$, but it does not restrict the independently variable $\eta(T)$ and therefore does not remove that condition.

For clarity, without the extra initial-acceleration restriction the actual unique minimizing profile is

$$
\boxed{V_*(t)=\frac{L}{T-\tanh(\kappa T)/\kappa}\left(1-\frac{\cosh[\kappa(T-t)]}{\cosh(\kappa T)}\right).}
$$

It satisfies $V_*(0)=0$, $\dot V_*(T)=0$, the distance constraint and the interior equation, but $\dot V_*(0)>0$. For any perturbation preserving the distance and initial speed, the first variation about $V_*$ is zero, and

$$
E[V_*+\eta]-E[V_*]=\int_0^T(a\eta^2+b\dot\eta^2)\,dt\geq0,
$$

with equality only for $\eta=0$. Its energy is $aL^2/[T-\tanh(\kappa T)/\kappa]$.

This same energy is the unattained infimum under the extra condition $\dot V(0)=0$. Indeed multiply $V_*$ by $1-e^{-t/\varepsilon}$ and rescale by a factor tending to one to restore total distance $L$. These smooth nonnegative profiles have both initial values zero and converge to $V_*$ in value and derivative square integrals as $\varepsilon\downarrow0$. Their energies tend to $E[V_*]$, but uniqueness of $V_*$ precludes attaining it with zero initial acceleration. This is [nonattainment under an initial derivative constraint](../../../../../../nonattainment-under-an-initial-derivative-constraint.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16C](../../16c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
