<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

For a standard collinear [Lorentz transformation](../../../../../lorentz-transformation.md), put $\beta=v/c$ and $\gamma=(1-\beta^2)^{-1/2}$, with $|v|<c$. Then $x'=\gamma(x-vt)$ and $ct'=\gamma(ct-\beta x)$. Define the [rapidity](../../../../../rapidity.md) $\phi=\operatorname{artanh}\beta$. The identities $\cosh^2\phi-\sinh^2\phi=1$ and $\tanh\phi=\beta$, with $\cosh\phi>0$, give $\cosh\phi=\gamma$ and $\sinh\phi=\gamma\beta$. Substitution proves the desired hyperbolic form.

Adding and subtracting those transformed coordinates uses $\cosh\phi\mp\sinh\phi=e^{\mp\phi}$ and yields

$$
\boxed{x'+ct'=e^{-\phi}(x+ct),\qquad x'-ct'=e^{\phi}(x-ct).}
$$

A second collinear [Lorentz transformation](../../../../../lorentz-transformation.md) of [rapidity](../../../../../rapidity.md) $\phi'$ multiplies these two null coordinates by $e^{-\phi'}$ and $e^{\phi'}$. Their total factors are therefore $e^{-(\phi+\phi')}$ and $e^{\phi+\phi'}$, proving

$$
\boxed{\phi''=\phi+\phi'.}
$$

The hyperbolic tangent addition formula now gives the velocity composition law

$$
\boxed{v''=c\tanh(\phi+\phi')=\frac{v+v'}{1+vv'/c^2}.}
$$

All velocities here are signed along the same axis; the speed is the absolute value if either frame moves in the opposite direction.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
