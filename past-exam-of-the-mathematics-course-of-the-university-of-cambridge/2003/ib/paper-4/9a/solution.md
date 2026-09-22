<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

For a standard collinear [Lorentz boost](../../../../../lorentz-boost.md), put $\beta=v/c$ and $\Gamma=(1-\beta^2)^{-1/2}$. Its equations are $x'=\Gamma(x-\beta ct)$ and $ct'=\Gamma(ct-\beta x)$. Define the [rapidity](../../../../../rapidity.md) $\phi=\operatorname{arctanh}\beta$. Since $\cosh^2\phi-\sinh^2\phi=1$ and $\cosh\phi>0$, $\cosh\phi=\Gamma$ and $\sinh\phi=\Gamma\beta$. Therefore

$$
\boxed{x'=x\cosh\phi-ct\sinh\phi,\qquad
ct'=-x\sinh\phi+ct\cosh\phi}.
$$

Adding and subtracting, and using $\cosh\phi\mp\sinh\phi=e^{\mp\phi}$, gives

$$
\boxed{x'+ct'=e^{-\phi}(x+ct),\qquad x'-ct'=e^\phi(x-ct)}.
$$

A second boost multiplies these factors by $e^{\mp\phi'}$, so the combined [rapidity](../../../../../rapidity.md) is $\phi+\phi'$. The [hyperbolic tangent](../../../../../hyperbolic-tangent.md) addition formula then gives the [relativistic velocity addition](../../../../../velocity-addition-formula.md) law

$$
\boxed{v''=c\tanh(\phi+\phi')=\frac{v+v'}{1+vv'/c^2}}.
$$

Velocities are signed along the common axis, so this formula also covers oppositely directed boosts.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
