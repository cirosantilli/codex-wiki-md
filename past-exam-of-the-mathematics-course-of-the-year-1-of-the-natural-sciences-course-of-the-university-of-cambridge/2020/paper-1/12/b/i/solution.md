<h1 id="12/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At height $z>0$, the [elliptic paraboloid](../../../../../../elliptic-paraboloid.md) has a circular cross-section $0\le r\le\sqrt z$, of [area](../../../../../../surface-area.md) $\pi z$. The [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) [volume element](../../../../../../volume-element.md) therefore reduces the [volume integral](../../../../../../volume-integral.md) to

$$
K=\int_0^\infty\int_0^{2\pi}\int_0^{\sqrt z}f'(z)r\,dr\,d\theta\,dz
=\pi\int_0^\infty zf'(z)\,dz.
$$

For the specified $f$, the [derivative](../../../../../../derivative.md) is $e^{-z}(z^{-1/2}+\tfrac12z^{-3/2})$. Thus $zf'(z)$ is integrable at zero and decays exponentially at infinity. Apply [integration by parts](../../../../../../integration-by-parts.md) first on a truncated interval and then take the endpoint [limits](../../../../../../limit-of-a-function.md):

$$
K=\pi[zf(z)]_0^\infty-\pi\int_0^\infty f(z)\,dz
=\pi\int_0^\infty\frac{e^{-z}}{\sqrt z}\,dz.
$$

Both boundary terms vanish because $zf(z)=-\sqrt z\,e^{-z}$. With $z=u^2$, [integration by substitution](../../../../../../integration-by-substitution.md) gives the [Gaussian integral](../../../../../../gaussian-integral.md):

$$
\boxed{K=2\pi\int_0^\infty e^{-u^2}\,du=\pi^{3/2}.}
$$

The integrand is singular at the apex but the resulting [improper integral](../../../../../../improper-integral.md) is convergent.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
