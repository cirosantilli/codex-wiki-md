<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Decompose the original [scalar field](../../../../../../scalar-field.md) as $\Phi=\phi+\widehat\phi$, where $\widetilde\phi(p)$ has support in $|p|\leq\Lambda'$ and $\widetilde{\widehat\phi}(p)$ has support in $\Lambda'<|p|\leq\Lambda$. This is a [momentum-shell decomposition of a scalar field](../../../../../../momentum-shell-decomposition-of-a-scalar-field.md). The two collections of integration variables are disjoint. Define the lower-scale [Wilsonian effective action](../../../../../../wilsonian-effective-action.md) by integrating out the second collection:

$$
\boxed{e^{-S_{\Lambda'}^{\mathrm{eff}}[\phi]}=\int_{\mathrm{shell}}\mathcal D\widehat\phi\,e^{-S_\Lambda^{\mathrm{eff}}[\phi+\widehat\phi]}.}
$$

A field-independent normalization may be retained as a vacuum term or absorbed into the measure. Integrating this identity over the low modes recovers the original [Euclidean path integral](../../../../../../euclidean-path-integral.md), so it preserves all observables depending only on those modes.

Put $\Delta S=S_\Lambda^{\mathrm{eff}}[\phi+\widehat\phi]-S_\Lambda^{\mathrm{eff}}[\phi]$. The quadratic cross terms integrate to zero: in [Fourier transform](../../../../../../fourier-transform.md) variables each pairs a low momentum with its negative, which cannot be a shell momentum. Expanding the interaction therefore gives

$$
\boxed{\Delta S=\int d^4x\left\{\frac12(\partial\widehat\phi)^2+\frac12m^2\widehat\phi^2+\frac g{24}\left(4\phi^3\widehat\phi+6\phi^2\widehat\phi^2+4\phi\widehat\phi^3+\widehat\phi^4\right)\right\}.}
$$

Factoring $e^{-S_\Lambda^{\mathrm{eff}}[\phi]}$ out of the shell integral and taking minus its logarithm yields

$$
\boxed{S_{\Lambda'}^{\mathrm{eff}}[\phi]=S_\Lambda^{\mathrm{eff}}[\phi]-\log\int_{\mathrm{shell}}\mathcal D\widehat\phi\,e^{-\Delta S[\phi,\widehat\phi]}.}
$$

This definition is a [Wilsonian effective action](../../../../../../wilsonian-effective-action.md), rather than a Legendre transform generating only [one-particle-irreducible Feynman diagrams](../../../../../../one-particle-irreducible-feynman-diagram.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
