<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathbf n=\mathbf R/R$. The first [sphere](../../../../../../sphere.md)'s leading [velocity field](../../../../../../velocity-field.md) is $\mathbf u_0=a^3\boldsymbol\Omega_0\times\mathbf x/r^3$. Taking its [curl](../../../../../../curl.md) gives

$$
\boldsymbol\omega_0(\mathbf x)=\frac{a^3}{r^3}\bigl[3\widehat{\mathbf x}(\widehat{\mathbf x}\cdot\boldsymbol\Omega_0)-\boldsymbol\Omega_0\bigr].
$$

The second [sphere](../../../../../../sphere.md) is [torque-free](../../../../../../torque-free.md), so

$$
\boxed{\boldsymbol\Omega_R\sim\frac{a^3}{2R^3}\bigl[3\mathbf n(\mathbf n\cdot\boldsymbol\Omega_0)-\boldsymbol\Omega_0\bigr].}
$$

Its own [force-free](../../../../../../force-free.md) and [torque-free](../../../../../../torque-free.md) motion emits no [Stokeslet](../../../../../../stokeslet.md) or [rotlet](../../../../../../rotlet.md); further reflections are smaller at large separation. In particular it spins in the opposite direction for a primary rotation perpendicular to the line of centers, and in the same direction with twice that magnitude for a parallel rotation.

Now isolate the additional interaction caused by the applied [force](../../../../../../force.md) $\mathbf F$. Its leading [Stokeslet](../../../../../../stokeslet.md) produces at the first center the incident [velocity](../../../../../../velocity.md) $(I+\mathbf n\mathbf n)\mathbf F/(8\pi\mu R)$. The [Stokes drag law](../../../../../../stokes-s-law.md) makes the increment of the [force](../../../../../../force.md) required to hold that [sphere](../../../../../../sphere.md) fixed

$$
\boxed{\mathbf F_0\sim-\frac{3a}{4R}(I+\mathbf n\mathbf n)\mathbf F,\qquad |\mathbf F_0|=O(a|\mathbf F|/R).}
$$

The sign opposes the incident [velocity](../../../../../../velocity.md). This holding [force](../../../../../../force.md) acts on the fluid and generates a reflected [Stokeslet](../../../../../../stokeslet.md). A [Stokeslet](../../../../../../stokeslet.md) of [force](../../../../../../force.md) $\mathbf F_0$ has [vorticity](../../../../../../vorticity.md) $\mathbf F_0\times\mathbf x/(4\pi\mu r^3)$. Evaluating half that [vorticity](../../../../../../vorticity.md) at $\mathbf R$ gives

$$
\delta\boldsymbol\Omega_R\sim\frac{\mathbf F_0\times\mathbf n}{8\pi\mu R^2}=\boxed{\frac{3a}{32\pi\mu R^3}\mathbf n\times\mathbf F}.
$$

Thus its magnitude is $O[(|\mathbf F|/(\mu a^2))(a/R)^3]$, as required. This is [forced-sphere rotation reflected from a held sphere](../../../../../../forced-sphere-rotation-reflected-from-a-held-sphere.md). Longitudinal forcing has zero leading spin by [symmetry](../../../../../../symmetry-physics.md). Finite-size multipoles and the [couple](../../../../../../couple-mechanics.md) correction needed to preserve the first [sphere](../../../../../../sphere.md)'s prescribed spin are smaller than this force-monopole reflection by order $(a/R)^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
