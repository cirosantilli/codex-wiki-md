<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work on a [beta plane](../../../../../beta-plane.md) with $f=f_0+\beta y$ and constant depth $H$. Assume a steady, small-[Rossby number](../../../../../rossby-number.md) interior, negligible friction there, small sea-surface displacements, and negligible depth gradients. Taking the vertical [curl](../../../../../curl.md) of momentum gives

$$
\partial_t\zeta+\mathbf u\cdot\nabla\zeta+(\zeta+f)\nabla\cdot\mathbf u+\beta v=(\nabla\times\mathbf W)_z+(\nabla\times\mathbf D)_z.
$$

The constant-depth continuity equation gives $\nabla\cdot\mathbf u=0$. Neglecting relative-vorticity tendency and advection, and the interior dissipation, yields [Sverdrup balance](../../../../../sverdrup-balance.md):

$$
\boxed{\beta v=(\nabla\times\mathbf W)_z.}
$$

Introduce the [ocean transport streamfunction](../../../../../ocean-transport-streamfunction.md) by $Hu=-\psi_y$, $Hv=\psi_x$. Then $\beta\psi_x=H(\nabla\times\mathbf W)_z$. Here $\mathbf W$ has units of acceleration, as in the given momentum equation; for a physical surface [wind stress](../../../../../wind-stress.md) $\boldsymbol\tau$, it would be $\boldsymbol\tau/(\rho H)$.

To obtain the circulation law, use the vector identity $\mathbf u\cdot\nabla\mathbf u=\nabla(|\mathbf u|^2/2)+\zeta\widehat{\mathbf k}\times\mathbf u$. Its gradient term and the sea-surface [pressure gradient](../../../../../pressure-gradient.md) integrate to zero around a closed contour. Thus

$$
\boxed{\partial_t\oint_C\mathbf u\cdot d\mathbf l=-\oint_C(\zeta+f)(\widehat{\mathbf k}\times\mathbf u)\cdot d\mathbf l+\oint_C(\mathbf W+\mathbf D)\cdot d\mathbf l.}
$$

On an impermeable island boundary, velocity is tangent to the coast, so $(\widehat{\mathbf k}\times\mathbf u)\cdot d\mathbf l=0$ pointwise. Consequently its [circulation](../../../../../circulation-physics.md) obeys

$$
\boxed{\partial_t\oint_{C_I}\mathbf u\cdot d\mathbf l=\oint_{C_I}(\mathbf W+\mathbf D)\cdot d\mathbf l.}
$$

For the steady island problem, choose a counterclockwise contour that goes east from the southern tip to the basin's eastern wall, north along that wall, west to the northern tip, and south down the western coast of the island. It avoids the eastern-island and western-basin dissipative layers. In the leading momentum balance, $\widehat{\mathbf k}\times\mathbf u=-\nabla\psi/H$. Integration by parts gives

$$
\oint_C f(\widehat{\mathbf k}\times\mathbf u)\cdot d\mathbf l=\frac1H\oint_C\psi\,df=-\frac{f(y_N)-f(y_S)}H\psi_I.
$$

Here $\psi=0$ on the basin wall and $\psi=\psi_I$ on the island, with constant latitude on the two connecting legs. Equating this integral to the wind forcing gives the [Godfrey island rule](../../../../../godfrey-island-rule.md)

$$
\boxed{\psi_I=-\frac H{\beta(y_N-y_S)}\oint_C\mathbf W\cdot d\mathbf l.}
$$

For the square island, $y_N=R/2$, $y_S=-R/2$, and its west coast is $x=-R/2$. Both horizontal contour legs have length $S+R/2$. With $\mathbf W=\sin(\pi y)\mathbf e_x$,

$$
\oint_C\mathbf W\cdot d\mathbf l=-2(S+R/2)\sin(\pi R/2),
$$

so

$$
\boxed{\psi_I=\frac{2H(S+R/2)}{\beta R}\sin(\pi R/2),\qquad T_{\rm east}=\int_{R/2}^S Hv\,dx=-\psi_I.}
$$

The sign convention makes $T_{\rm east}$ positive northward. For $0<R<2$ it is southward. The total transport includes the island's thin eastern boundary current: omitting that current would leave a latitude-dependent interior transport rather than this constant passage transport.

To quantify the island's effect on the [western boundary current](../../../../../western-boundary-current.md), compare interior streamfunctions west of the island. In its latitude band, the inviscid solution is

$$
\psi_{\rm west}(x,y)=\psi_I+\frac{H\pi}{\beta}\cos(\pi y)(-R/2-x).
$$

Without an island it would be $H\pi\cos(\pi y)(S-x)/\beta$. Since the western basin wall has zero streamfunction, the difference in its required northward boundary-current transport is

$$
\boxed{\delta T_W(y)=\psi_I-\frac{H\pi}{\beta}(S+R/2)\cos(\pi y).}
$$

Thus the island changes the current's strength by redistributing transport across its latitude band. For a square contained in the central positive-cosine band, it weakens the northward current near $y=0$ and strengthens it near the island's northern and southern edges. The change averages to zero over $-R/2<y<R/2$; its local sign follows the formula for other island sizes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
