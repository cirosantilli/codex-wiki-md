<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [open matter-dominated Friedmann solution](../../../../../../open-matter-dominated-friedmann-solution.md), write $\Omega=\Omega_{m,0}$, so $0<\Omega<1$. The present [Friedmann equation](../../../../../../friedmann-equations.md) gives $-K=H_0^2(1-\Omega)$. With $A=H_0^2\Omega$ and $B=H_0^2(1-\Omega)>0$, the expanding equation becomes

$$
\dot a^2=\frac Aa+B,\qquad
dt=\frac1{\sqrt B}\sqrt{\frac a{a+A/B}}\,da.
$$

Choose the [hyperbolic substitution](../../../../../../hyperbolic-substitution.md)

$$
a=\frac AB\sinh^2\frac\eta2
=\frac A{2B}(\cosh\eta-1),\qquad \eta\geq0.
$$

Then $da=(A/(2B))\sinh\eta\,d\eta$ and $\sqrt{a/(a+A/B)}=\tanh(\eta/2)$. Their product gives

$$
\frac{dt}{d\eta}=\frac A{2B^{3/2}}(\cosh\eta-1)
=\frac a{\sqrt B}.
$$

Take the [Big Bang](../../../../../../big-bang.md) to be $t=0$, $\eta=0$, and integrate. The **parametric solution** is

$$
\boxed{a(\eta)=\frac{\Omega}{2(1-\Omega)}(\cosh\eta-1),
\qquad
t(\eta)=\frac{\Omega}{2H_0(1-\Omega)^{3/2}}(\sinh\eta-\eta).}
$$

The parameter is determined explicitly by

$$
\boxed{\eta=2\operatorname{arsinh}\sqrt{\frac{(1-\Omega)a}{\Omega}},
\qquad \eta=\sqrt{-K}\int_0^t\frac{dt'}{a(t')}.}
$$

Thus $\eta$ is [conformal time](../../../../../../conformal-time.md) multiplied by $\sqrt{-K}$, with its origin at the [Big Bang](../../../../../../big-bang.md); it is not equal to unscaled [cosmic time](../../../../../../cosmic-time.md). In particular today $\eta_0=\operatorname{arcosh}(2/\Omega-1)$. Small $\eta$ gives $a\propto\eta^2$ and $t\propto\eta^3$, hence $a\propto t^{2/3}$. Large $\eta$ gives $a/t\to H_0\sqrt{1-\Omega}=\sqrt{-K}$, in agreement with the [curvature-dominated universe](../../../../../../curvature-dominated-universe.md) limit.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
