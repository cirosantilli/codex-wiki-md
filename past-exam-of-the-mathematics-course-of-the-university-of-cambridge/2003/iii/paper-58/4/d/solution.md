<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Restore the [Fourier transform](../../../../../../fourier-transform.md) integral and the last-scattering distance:

$$
\Theta(\widehat{\mathbf n})=\frac13\int\frac{d^3k}{(2\pi)^3}\Phi_{\mathbf k}
e^{i\mathbf k\cdot\widehat{\mathbf n}\chi_*}.
$$

Insert the [Rayleigh plane-wave expansion](../../../../../../rayleigh-plane-wave-expansion.md) and use [orthogonality](../../../../../../orthogonal-vectors.md) of [spherical harmonics](../../../../../../spherical-harmonic.md) with the complex conjugate on the projection harmonic. The angular integral selects the matching indices, giving

$$
\boxed{a_{\ell m}=\frac{4\pi i^\ell}{3}\int\frac{d^3k}{(2\pi)^3}
\Phi_{\mathbf k}j_\ell(k\chi_*)Y_{\ell m}^*(\widehat{\mathbf k}).}
$$

The complex conjugation is present in the original PDF. If $A_{\mathbf k}=A\,k^{n/2}$ denotes a mode coefficient with its random amplitude and phase included in $A$, substitution of $\Phi_{\mathbf k}=-6A_{\mathbf k}/k^2$ gives the equivalent factor $-8\pi i^\ell A_{\mathbf k}/k^2$ inside the Fourier integral. The monopole and local observer dipole removed in part (b) do not change this formula for $\ell\geq2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
