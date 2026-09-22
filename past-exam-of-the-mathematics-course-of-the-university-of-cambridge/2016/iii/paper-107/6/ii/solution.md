<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a [signed power test for a Laplacian eigenfunction](../../../../../../signed-power-test-for-a-laplacian-eigenfunction.md). For $\gamma\geq2$, test the [Dirichlet Laplacian eigenfunction](../../../../../../dirichlet-laplacian-eigenfunction.md) equation with $|u|^{\gamma-2}u$. Its derivative is $(\gamma-1)|u|^{\gamma-2}Du$; at $\gamma=2$ the test function is just $u$. [Integration by parts](../../../../../../integration-by-parts.md) gives the exact [energy estimate](../../../../../../energy-estimate.md)

$$
(\gamma-1)\int_\Omega |u|^{\gamma-2}|Du|^2=\lambda\int_\Omega |u|^\gamma.
$$

Set $v=|u|^{\gamma/2}$. It belongs to the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md) and obeys the [Sobolev chain rule](../../../../../../sobolev-chain-rule.md):

$$
\int_\Omega|Dv|^2=\frac{\gamma^2}{4}\int_\Omega|u|^{\gamma-2}|Du|^2
=\frac{\lambda\gamma^2}{4(\gamma-1)}\int_\Omega|u|^\gamma.
$$

For $\gamma>2$, the power map is $C^1$ with bounded derivative on the bounded range of $u$. For $\gamma=2$, the [absolute value](../../../../../../absolute-value.md) map is Lipschitz, and $D|u|=\operatorname{sgn}(u)Du$ [almost everywhere](../../../../../../almost-everywhere.md); on the zero set, use the fact that a [gradient of a Sobolev function vanishes on a level set](../../../../../../gradient-of-a-sobolev-function-vanishes-on-a-level-set.md). These facts justify the identity even when $u$ changes sign.

Apply the given [Sobolev inequality](../../../../../../sobolev-inequality.md) with the [Sobolev conjugate exponent](../../../../../../sobolev-conjugate-exponent.md) $2\kappa=2n/(n-2)$:

$$
\boxed{\left(\int_\Omega|u|^{\gamma\kappa}\right)^{1/\kappa}
\leq\frac{C(n)\lambda\gamma^2}{4(\gamma-1)}\int_\Omega|u|^\gamma.}
$$

**Testing with a signed power raises the integrability exponent from $\gamma$ to $\gamma\kappa$.** Absorbing the factor $1/4$ into $C(n)$ gives precisely the requested inequality.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
