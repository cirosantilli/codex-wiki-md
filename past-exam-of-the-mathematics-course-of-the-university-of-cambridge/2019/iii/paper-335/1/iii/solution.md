<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The boundary identity gives a numerical route to [shape recovery from a Herglotz boundary identity](../../../../../../shape-recovery-from-a-herglotz-boundary-identity.md). First recover an admissible density $g$ from measured [far-field patterns](../../../../../../far-field-pattern.md), enforcing the supplied [Herglotz pairing with an obstacle far field](../../../../../../herglotz-pairing-with-an-obstacle-far-field.md) for available incident directions:

$$
\int_{S^2}f_\infty(\widehat{\mathbf r},\widehat{\mathbf r}_0,k)\overline{g(\widehat{\mathbf r})}\,dS=\frac1k.
$$

Then evaluate its [Herglotz wave function](../../../../../../herglotz-wave-function.md) throughout a search region and find a smooth positive radial profile satisfying

$$
\boxed{v_g(h(\theta)\widehat{\mathbf r}(\theta,\phi))+\frac{e^{-ikh(\theta)}}{kh(\theta)}=0.}
$$

The same $h(\theta)$ must work for every azimuth $\phi$, expressing the assumed axial symmetry. In practice expand $g$ and $h$ in basis functions, enforce these equations at collocation points, and minimize the complex residual together with the far-field-data residual. The exclusion of an interior Dirichlet eigenvalue ensures uniqueness of the interior [Dirichlet problem](../../../../../../dirichlet-problem.md) for the trial boundary data. Use [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) to control measurement error and unstable density components; neither uniqueness nor numerical stability follows merely from writing the residual equations.

For rich incident-direction data, the conjugated pairing constraints form an adjoint far-field integral equation for $g$. For only one fixed incidence, the displayed pairing is a single complex scalar constraint and cannot by itself determine an arbitrary density. Additional data or a joint constrained shape fit is then needed; the trace condition supplies the actual geometric information.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
