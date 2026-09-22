<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To close a depth-integrated bottom-drag model, approximate the bottom horizontal velocity by the depth mean, $\mathbf u_b\simeq\mathbf T/H$. This is the barotropic closure needed to express the stated stress solely in terms of the transport. Define

$$
r=\frac{\gamma}{\rho_0H},\qquad S(y)=\frac{W(y)}{\rho_0}.
$$

The coefficient $\gamma$ in a physical stress law is not itself a drag rate; $r$ has units of inverse time. The [ocean basin equation with bottom drag and lateral viscosity](../../../../../../ocean-basin-equation-with-bottom-drag-and-lateral-viscosity.md) follows by taking curl of the integrated momentum equation and yields the combined [Stommel boundary layer](../../../../../../stommel-boundary-layer.md) and [Munk boundary layer](../../../../../../munk-boundary-layer.md) equation,

$$
\boxed{\beta\bar\psi_x=S-r\nabla_h^2\bar\psi+\nu\nabla_h^4\bar\psi.}
$$

The bottom contribution is negative because the vertically integrated stress difference is surface stress minus bottom stress. Set the constant wall [streamfunction](../../../../../../stream-function.md) to zero. No normal flow and no tangential slip impose $\bar\psi=0$ and $\partial_n\bar\psi=0$ on the walls.

The inviscid interior solution has $\bar\psi_I=S(y)x/\beta+C_0(y)$. In a thin east/west layer, $x$ derivatives dominate the smaller $y$ derivatives. Holding $y$ as a parameter gives

$$
\boxed{\nu\frac{d^4\bar\psi}{dx^4}-r\frac{d^2\bar\psi}{dx^2}-\beta\frac{d\bar\psi}{dx}=-S(y).}
$$

Equivalently the boundary correction $\phi=\bar\psi-\bar\psi_I$ obeys $\nu\phi''''-r\phi''-\beta\phi'=0$. In a stretched inward coordinate $X=x/\delta$ at the west wall and $X=(1-x)/\delta$ at the east wall, this becomes respectively

$$
\frac\nu{\delta^4}\phi_{XXXX}-\frac r{\delta^2}\phi_{XX}-\frac\beta\delta\phi_X=0,
\qquad
\frac\nu{\delta^4}\phi_{XXXX}-\frac r{\delta^2}\phi_{XX}+\frac\beta\delta\phi_X=0.
$$

The first-derivative sign reversal distinguishes east from west. Vanishing $W$ and its derivatives at the north/south boundaries makes leading forcing-dependent solutions compatible with those boundaries, avoiding extra leading meridional layers. These are leading boundary-layer equations, not an exact deletion of every meridional derivative in the full basin PDE.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
