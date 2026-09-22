<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Bogomolny bound](../../../../../bogomolny-bound.md) expresses a static field energy as nonnegative squares plus a term fixed by the [topological charge](../../../../../topological-charge.md) or boundary data. Setting the squares to zero gives the first-order [Bogomolny equations](../../../../../bogomolny-equations.md). Their solutions minimize the energy in that sector and satisfy the second-order [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md), although a general stationary solution need not attain the bound.

For one real scalar in one spatial dimension, take the [Lagrangian density](../../../../../lagrangian-density.md)

$$
\mathcal L=\frac12\dot\phi^2-\frac12\phi_x^2-\frac12[W'(\phi)]^2.
$$

A [finite-energy field configuration](../../../../../finite-energy-field-configuration.md) in this static sector must approach [scalar-field vacua](../../../../../scalar-field-vacuum.md) $\phi_\pm$ with $W'(\phi_\pm)=0$ at the two ends. [Completing the square](../../../../../completing-the-square.md) gives the [square completion for a one-dimensional kink](../../../../../square-completion-for-a-one-dimensional-kink.md):

$$
E=\frac12\int_{\mathbb R}(\phi_x\mp W')^2dx\pm\int_{\mathbb R}\phi_xW'(\phi)dx
=\frac12\int_{\mathbb R}(\phi_x\mp W')^2dx\pm[W(\phi_+)-W(\phi_-)].
$$

Choose the sign for which the boundary term is nonnegative. Thus

$$
\boxed{E\geq|W(\phi_+)-W(\phi_-)|,\qquad \phi_x=\pm W'(\phi)\text{ at equality}.}
$$

Taking the [derivative](../../../../../derivative.md) of the equality equation gives $\phi_{xx}=W'W''=d([W']^2/2)/d\phi$, the static [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md). The boundary term is invariant under deformations keeping the asymptotic [scalar-field vacua](../../../../../scalar-field-vacuum.md) fixed; it is not a contribution from the local shape of the kink.

For a [phi-four kink](../../../../../phi-four-kink.md), let $c>0$, $W(\phi)=c^2\phi-\phi^3/3$, and select the sector $\phi_-=-c$, $\phi_+=c$. Then $W'=c^2-\phi^2$, and the increasing [Bogomolny equation](../../../../../bogomolny-equations.md) is $\phi_x=c^2-\phi^2$. Separating variables yields

$$
\frac1{2c}\log\frac{c+\phi}{c-\phi}=x-X,
\qquad
\boxed{\phi_K(x)=c\tanh(c(x-X)),\qquad M=\frac{4c^3}{3}.}
$$

The integration constant $X$ is the translational [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md). Directly, $\phi_K'=c^2\operatorname{sech}^2(c(x-X))$ and its [energy density](../../../../../energy-density.md) is $c^4\operatorname{sech}^4(c(x-X))$, whose integral is $4c^3/3$. The decreasing antikink has the reversed boundary values, profile $-\phi_K$, and the same energy. A [Lorentz boost](../../../../../lorentz-boost.md) produces the exact uniformly moving kink $c\tanh[c\gamma(x-X_0-vt)]$, with [Lorentz factor](../../../../../lorentz-factor.md) $\gamma=(1-v^2)^{-1/2}$ and energy $\gamma M$.

In two spatial dimensions, choose the [Abelian Higgs model](../../../../../abelian-higgs-model.md) at [critical coupling](../../../../../critical-coupling.md), with $D_i=\partial_i-iA_i$, $B=\partial_1A_2-\partial_2A_1$, and energy

$$
E=\int_{\mathbb R^2}\left[\frac12B^2+\frac12(|D_1\phi|^2+|D_2\phi|^2)+\frac18(1-|\phi|^2)^2\right]d^2x.
$$

The [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) is used throughout this normalization. [Integration by parts](../../../../../integration-by-parts.md), using $[D_1,D_2]=-iB$, gives $\int|D_i\phi|^2=\int|(D_1+iD_2)\phi|^2+\int B|\phi|^2$, with a vanishing boundary divergence for the decaying vortex fields. Combining this identity with the magnetic and potential terms gives the [Bogomolny square completion for an Abelian Higgs vortex](../../../../../bogomolny-square-completion-for-an-abelian-higgs-vortex.md):

$$
E=\int\left[\frac12|(D_1+iD_2)\phi|^2+\frac12\left(B-\frac{1-|\phi|^2}{2}\right)^2\right]d^2x+\frac12\int B\,d^2x.
$$

[Finite-energy field configurations](../../../../../finite-energy-field-configuration.md) have $|\phi|\to1$ at infinity, and $D_i\phi\to0$ makes the [magnetic flux](../../../../../magnetic-flux.md) equal to the phase winding $2\pi N$. For $N>0$,

$$
\boxed{E\geq\pi N,\qquad(D_1+iD_2)\phi=0,\qquad B=\frac{1-|\phi|^2}{2}.}
$$

These are the [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md) for an [Abelian Higgs vortex](../../../../../nielsen-olesen-vortex.md). Opposite signs give antivortices and the bound $E\geq\pi|N|$. The coefficient $\pi$ follows from the explicit energy normalization above; other conventions can give $2\pi$. Static solutions of fixed positive [vortex number](../../../../../vortex-number.md) have equal energy independent of their positions, giving the [Abelian Higgs vortex moduli space](../../../../../abelian-higgs-vortex-moduli-space.md) used for slow dynamics.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
