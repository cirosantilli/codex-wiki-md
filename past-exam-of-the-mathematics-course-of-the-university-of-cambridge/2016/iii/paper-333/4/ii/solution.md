<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Q_b=f/H$. At sufficiently small [Rossby number](../../../../../../rossby-number.md), retain advection of this full background [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) while dropping the higher-order advection of $\zeta/H$. For uniform-depth [Sverdrup balance](../../../../../../sverdrup-balance.md), this also requires relative-vorticity advection to be small against planetary-vorticity advection; small [Rossby number](../../../../../../rossby-number.md) alone does not guarantee this when $\beta$ is very small. Multiplying the resulting steady [potential vorticity](../../../../../../potential-vorticity.md) equation by $H$ gives

$$
-\psi_y(Q_b)_x+\psi_x(Q_b)_y=F-r\zeta.
$$

Define the [topographic potential-vorticity pseudovelocity](../../../../../../topographic-potential-vorticity-pseudovelocity.md)

$$
\boxed{\widetilde{\mathbf u}=\widehat{\mathbf z}\times\nabla_h(f/H)=\left(-\partial_y(f/H),\partial_x(f/H)\right).}
$$

Its sign is important: it is opposite to the coefficient vector on the left of the preceding equation. Substituting the [ocean transport streamfunction](../../../../../../ocean-transport-streamfunction.md) expression for [relative vorticity](../../../../../../relative-vorticity.md) yields

$$
\boxed{\widetilde{\mathbf u}\cdot\nabla_h\psi=\frac rH\nabla_h^2\psi-F-r\frac{\nabla_hH\cdot\nabla_h\psi}{H^2}.}
$$

The [pseudovelocity](../../../../../../topographic-potential-vorticity-pseudovelocity.md) follows contours of $f/H$ and is not the fluid velocity; its units are inverse length squared per time because $\psi$ is a transport streamfunction. If $r=F=0$, the [ocean transport streamfunction](../../../../../../ocean-transport-streamfunction.md) is constant along each connected background [potential vorticity](../../../../../../potential-vorticity.md) contour. Locally, at regular points,

$$
\boxed{\psi=\Phi(f/H),}
$$

with arbitrary differentiable $\Phi$. Different disconnected components of a level set may carry different functions until boundary conditions identify them. If $f/H$ is constant over an open region, the leading equation gives no restriction there; critical points similarly require regularity and global matching rather than division by a vanishing gradient.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
