<h1 id="11a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $E$ to be continuously differentiable everywhere on $\mathbb R^3$, as in the question. Its zero [curl](../../../../../../curl.md) says $\partial_iE_j=\partial_jE_i$. Construct a [potential of a conservative vector field](../../../../../../potential-of-a-conservative-vector-field.md) explicitly by

$$
\phi(x)=-\int_0^1E(tx)\cdot x\,dt.
$$

All segments lie in $\mathbb R^3$. Differentiating under the integral and using the symmetry of the derivatives,

$$
\partial_i\phi=-\int_0^1[E_i(tx)+t x_j\partial_iE_j(tx)]\,dt=-\int_0^1[E_i(tx)+t x_j\partial_jE_i(tx)]\,dt=-\int_0^1\frac{d}{dt}[tE_i(tx)]\,dt=-E_i(x).
$$

Hence **$E=-\nabla\phi$**. This [radial integral potential for a curl-free field](../../../../../../radial-integral-potential-for-a-curl-free-field.md) also works on a star-shaped domain after translating its centre. On an arbitrary domain, zero [curl](../../../../../../curl.md) only guarantees local potentials; the everywhere-on-$\mathbb R^3$ interpretation is important for this global assertion.

For the given field, put $q=e^{-x^2z}$. The three pairs of derivatives entering its [curl](../../../../../../curl.md) are

$$
\partial_yE_z=2x^2yq=\partial_zE_y,\qquad \partial_zE_x=2xy^2(1-x^2z)q=\partial_xE_z,\qquad \partial_xE_y=4xyzq=\partial_yE_x.
$$

Thus the field is [irrotational](../../../../../../irrotational-vector-field.md). To find its potential using $E_y=-\partial_y\phi$, integrate $\partial_y\phi=2yq$ to get $\phi=y^2q+\psi(x,z)$. Comparison with $E_x=-\partial_x\phi$ gives $\psi_x=0$, and comparison with $E_z=-\partial_z\phi$ gives $\psi_z=0$. Therefore

$$
\boxed{\phi(x,y,z)=y^2e^{-x^2z}+C}.
$$

Differentiating this expression reproduces all three components with the required minus sign; the only freedom on the connected domain is the additive constant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
