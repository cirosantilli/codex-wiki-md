<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $E_\lambda=e^{-i\beta(\lambda z-\bar z/\lambda)}$. The [Wirtinger derivatives](../../../../../../wirtinger-derivatives.md) give $(E_\lambda)_z=-i\beta\lambda E_\lambda$ and $(E_\lambda)_{\bar z}=i\beta E_\lambda/\lambda$. Write $W=A\,dz+B\,d\bar z$, where

$$
A=E_\lambda(u_z+i\beta\lambda u),\qquad
B=-E_\lambda(u_{\bar z}-i\beta u/\lambda).
$$

Using the [exterior derivative](../../../../../../exterior-derivative.md), $dW=(B_z-A_{\bar z})dz\wedge d\bar z$. The terms involving $u_z$ and $u_{\bar z}$ cancel, leaving

$$
\boxed{dW=-2E_\lambda(u_{z\bar z}-\beta^2u)\,dz\wedge d\bar z
=iE_\lambda(\Delta u-4\beta^2u)\,dx\wedge dy.}
$$

Because $E_\lambda$ never vanishes for $\lambda\ne0$, $dW=0$ if and only if $u_{z\bar z}-\beta^2u=0$. In real coordinates this is the [modified Helmholtz equation](../../../../../../modified-helmholtz-equation.md) with mass parameter $2\beta$, not $\beta$. In fact any one nonzero spectral parameter suffices for the equivalence; the full family supplies many independent boundary tests.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
