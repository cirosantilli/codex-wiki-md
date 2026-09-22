<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\xi$ denote [geodesic](../../../../../../geodesic.md) distance from the charge; $R$ is the fixed curvature radius, not the radial variable. In round three-dimensional [hyperbolic space](../../../../../../hyperbolic-space.md), a sphere has area

$$
A(\xi)=4\pi R^2\sinh^2(\xi/R).
$$

Using the convention that [electric flux](../../../../../../electric-flux.md) is $Q/\epsilon_0$, [Gauss's law](../../../../../../gauss-s-law.md) gives the radial orthonormal [electric field](../../../../../../electric-field.md)

$$
\boxed{\mathbf E(\xi)=\frac{Q}{4\pi\epsilon_0R^2\sinh^2(\xi/R)}\,\widehat{\boldsymbol\xi}.}
$$

Its magnitude is $|Q|/A\epsilon_0$, and a negative charge reverses the direction. In rationalized natural units set $\epsilon_0=1$; Gaussian conventions instead use flux $4\pi Q$.

For $\xi\ll R$ this approaches $Q/(4\pi\epsilon_0\xi^2)$. For $\xi\gg R$, $E\sim Qe^{-2\xi/R}/(\pi\epsilon_0R^2)$. This [hyperbolic-space Coulomb field](../../../../../../hyperbolic-space-coulomb-field.md) falls rapidly because the sphere area grows exponentially; conserved [electric flux](../../../../../../electric-flux.md) is unchanged. A potential vanishing at infinity is $V=Q[\coth(\xi/R)-1]/(4\pi\epsilon_0R)$.

The original PDF actually prints $\sin\theta$ rather than $\sin^2\theta$ in the angular [metric tensor](../../../../../../metric-tensor.md). The round angular factor used above is required by its description as [hyperbolic space](../../../../../../hyperbolic-space.md). If the printed angular [metric tensor](../../../../../../metric-tensor.md) is taken literally, the sphere-area coefficient is instead

$$
\Omega_*=2\pi\int_0^\pi\sqrt{\sin\theta}\,d\theta
=2\pi\sqrt\pi\,\frac{\Gamma(3/4)}{\Gamma(5/4)},
$$

and a radial Gauss-law solution has $E=Q/[\epsilon_0\Omega_*R^2\sinh^2(\xi/R)]$. That angular geometry is not a smooth round sphere, so the literal [metric tensor](../../../../../../metric-tensor.md) does not describe the asserted homogeneous [hyperbolic space](../../../../../../hyperbolic-space.md). Both readings retain the same radial area-growth factor; the geometric repair is explicit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
