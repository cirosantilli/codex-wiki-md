<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use time dependence $e^{-i\omega t}$, positive [wavenumber](../../../../../../wavenumber.md) $k$ and [aperture](../../../../../../aperture.md) normal $\mathbf n=\mathbf e_x$. Write $F(y',z')=E_{{\rm inc},y}(0,y',z')$ on the [aperture](../../../../../../aperture.md) and extend $F$ by zero outside it. Define

$$
\widehat F(\nu,\eta)=\int_A F(y',z')e^{-i(\nu y'+\eta z')}\,dy'\,dz',\qquad
\kappa=\sqrt{k^2-\nu^2-\eta^2},\qquad \mathbf q=(\kappa,\nu,\eta).
$$

The outgoing branch has $\kappa\ge0$ for propagating components and $\operatorname{Im}\kappa>0$ for [evanescent](../../../../../../evanescent-wave.md) components.

Fix the [Green function](../../../../../../green-s-function.md) normalization by $G_0(\mathbf r)=e^{ik|\mathbf r|}/(4\pi|\mathbf r|)$, so $(\Delta+k^2)G_0=-\delta$. Its transverse [Fourier transform](../../../../../../fourier-transform.md) satisfies $(\partial_x^2+\kappa^2)\widehat G_0=-\delta(x)$. An outgoing solution on both sides is proportional to $e^{i\kappa|x|}$, and its [derivative](../../../../../../derivative.md) jump fixes $\widehat G_0=i e^{i\kappa|x|}/(2\kappa)$. Thus the [Weyl plane-wave representation](../../../../../../weyl-plane-wave-representation.md) for observation at $x>0$ is

$$
G_0=\frac{i}{2(2\pi)^2}\int_{\mathbb R^2}
\frac{e^{i\kappa x+i\nu(y-y')+i\eta(z-z')}}\kappa\,d\nu\,d\eta.
$$

Since $\mathbf n\times\mathbf E_{\rm inc}=F\mathbf e_z$, the given [aperture](../../../../../../aperture.md) integral becomes a superposition of [curls](../../../../../../curl.md) of $\mathbf e_z e^{i\mathbf q\cdot\mathbf r}$. Each [curl](../../../../../../curl.md) supplies $i\mathbf q\times\mathbf e_z=i(\nu,-\kappa,0)$. Therefore, with the unit prefactor in that integral,

$$
\boxed{\mathbf E(x,y,z)=\frac1{2(2\pi)^2}\int_{\mathbb R^2}
\widehat F(\nu,\eta)\left(-\frac\nu\kappa,1,0\right)
e^{i\kappa x+i\nu y+i\eta z}\,d\nu\,d\eta}.
$$

Every vector amplitude is transverse to $\mathbf q$, as [Maxwell's equations](../../../../../../maxwell-equations.md) require. The [polarizer](../../../../../../polarizer.md) specifies the incident [aperture](../../../../../../aperture.md) field; [diffraction](../../../../../../diffraction.md) can regenerate an $x$ component outside the [aperture](../../../../../../aperture.md). In contrast, its $z$ component remains zero in this representation. [Evanescent](../../../../../../evanescent-wave.md) [plane waves](../../../../../../plane-wave.md) are needed for the complete near field, not just the propagating disk $\nu^2+\eta^2\le k^2$.

The factor $1/2$ follows explicitly from the standard [outgoing Green function for the three-dimensional Helmholtz equation](../../../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md) and the printed unit [curl](../../../../../../curl.md) prefactor. If the intended kernel is the doubled half-space kernel $2G_0$, or the [aperture](../../../../../../aperture.md) formula carries the usual compensating factor $2$, delete that $1/2$. The latter normalization makes the tangential output trace equal to $F$. Keeping the convention explicit avoids silently changing the supplied representation; the angular dependence and [transversality of an electromagnetic plane wave](../../../../../../transversality-of-an-electromagnetic-plane-wave.md) are the same in either normalization. Reversing the specified normal also reverses the overall sign.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
