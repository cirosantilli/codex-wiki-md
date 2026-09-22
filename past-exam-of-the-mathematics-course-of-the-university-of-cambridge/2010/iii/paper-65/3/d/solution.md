<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use mean [incompressibility](../../../../../../incompressible-flow.md) to convert advection into momentum-flux divergence:

$$
UU_x+VU_y=\partial_x(U^2)+\partial_y(UV).
$$

Therefore the reduced [Reynolds-averaged momentum equation](../../../../../../reynolds-averaged-momentum-equation.md) gives

$$
\partial_x(U^2)+\partial_y\{UV+\overline{\hat u\hat v}\}=0.
$$

For a localized free jet, $UV$ and the [Reynolds stress](../../../../../../reynolds-stress.md) tend to zero in the quiescent ambient as $y\to\pm\infty$. Assume sufficient decay to differentiate its momentum integral. Integrating across the jet gives

$$
\boxed{\frac d{dx}\int_{-\infty}^{\infty}U^2\,dy
=-[UV+\overline{\hat u\hat v}]_{-\infty}^{\infty}=0.}
$$

Thus $M_0=\int U^2dy$ is constant. It is a specific momentum flux per unit span: multiplication by density gives the momentum flux. A clipped profile with nonzero stress just inside its artificial edge would fail this boundary-flux assumption unless an additional external momentum source were supplied.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
