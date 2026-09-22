<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The pullback of the flat [Euclidean metric](../../../../../euclidean-metric.md) under $x'{}^\mu=x^\mu+\epsilon\omega^\mu(x)$ is

$$
\delta_{\mu\nu}+\epsilon(\partial_\mu\omega_\nu+\partial_\nu\omega_\mu)+O(\epsilon^2).
$$

For a [conformal transformation](../../../../../conformal-map.md) it must be a scalar multiple of $\delta_{\mu\nu}$. Taking the [trace](../../../../../matrix-trace.md) determines that multiple. With $\rho=\partial_\alpha\omega^\alpha$, the necessary and sufficient infinitesimal condition is the [Conformal Killing equation](../../../../../conformal-killing-equation.md)

$$
\boxed{\partial_\mu\omega_\nu+\partial_\nu\omega_\mu=\frac{2\rho}{d}\delta_{\mu\nu}}.
$$

Differentiate its $(\alpha,\beta)$ instance with respect to $x^\gamma$, its $(\alpha,\gamma)$ instance with respect to $x^\beta$, and its $(\beta,\gamma)$ instance with respect to $x^\alpha$. Adding the first two and subtracting the last, commuting [partial derivatives](../../../../../partial-derivative.md), leaves $2\partial_\beta\partial_\gamma\omega_\alpha$. Hence [flat conformal Killing integrability](../../../../../flat-conformal-killing-integrability.md) gives

$$
\boxed{\partial_\beta\partial_\gamma\omega_\alpha=\frac1d(\delta_{\alpha\beta}\partial_\gamma\rho+\delta_{\alpha\gamma}\partial_\beta\rho-\delta_{\beta\gamma}\partial_\alpha\rho)}.
$$

Contracting $\beta$ with $\gamma$ gives $\Delta\omega_\alpha=(2-d)\partial_\alpha\rho/d$. Its [divergence](../../../../../divergence.md) is $\Delta\rho=(2-d)\Delta\rho/d$, so $2(d-1)\Delta\rho=0$: thus $\boxed{\Delta\rho=0\text{ for }d>1}$. Taking instead the $\alpha$ [divergence](../../../../../divergence.md) of the displayed second-derivative identity gives

$$
d\partial_\beta\partial_\gamma\rho=2\partial_\beta\partial_\gamma\rho-\delta_{\beta\gamma}\Delta\rho.
$$

Consequently $\boxed{\partial_\beta\partial_\gamma\rho=0\text{ for }d>2}$.

On a connected flat domain, write $\rho=d\lambda+2d\,b\cdot x$, with constant $\lambda$ and $b$. Integrating the second-derivative identity, and imposing the [Conformal Killing equation](../../../../../conformal-killing-equation.md) on its remaining affine part, gives the complete [Conformal Killing vector field](../../../../../conformal-killing-vector-field.md)

$$
\boxed{\omega^\mu(x)=a^\mu+R^\mu{}_{\nu}x^\nu+\lambda x^\mu+2(b\cdot x)x^\mu-b^\mu x^2},\qquad R_{\mu\nu}=-R_{\nu\mu}.
$$

Indeed the quadratic part has precisely the required [Hessian matrix](../../../../../hessian-matrix.md), while the symmetric part of the remaining linear term must be $\lambda\delta_{\mu\nu}$. The constants generate [translations](../../../../../translation-geometry.md), [rotations](../../../../../rotation-mathematics.md), [dilations](../../../../../uniform-dilation.md) and [special conformal transformations](../../../../../special-conformal-transformation.md), respectively. There are $d$, $d(d-1)/2$, $1$ and $d$ independent parameters, so the full [conformal group](../../../../../conformal-group.md) has dimension

$$
\boxed{\frac{(d+1)(d+2)}2}.
$$

Here “full” means local transformations, or global transformations of the [conformal compactification of Euclidean space](../../../../../conformal-compactification-of-euclidean-space.md); its connected group is locally $SO(d+1,1)$. Requiring every transformation to be nonsingular on all of uncompactified $\mathbb R^d$ would exclude the special [conformal transformations](../../../../../conformal-map.md) with finite poles.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
