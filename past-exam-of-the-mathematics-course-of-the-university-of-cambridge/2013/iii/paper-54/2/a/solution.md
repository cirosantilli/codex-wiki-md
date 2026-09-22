<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [razor-thin disk](../../../../../../razor-thin-disk-approximation.md), integrate the delta function in height to get

$$
\Phi_\epsilon(\mathbf R)=-G\int\frac{\Sigma(\mathbf R')\,d^2R'}{\sqrt{|\mathbf R-\mathbf R'|^2+\epsilon^2}}.
$$

The corresponding horizontal force kernel is proportional to $(\mathbf R-\mathbf R')/(|\mathbf R-\mathbf R'|^2+\epsilon^2)^{3/2}$. It removes the short-distance point-force singularity and smooths forces on separations of order $\epsilon$. This is [height-evaluation gravitational softening](../../../../../../height-evaluation-gravitational-softening.md).

To represent finite vertical thickness, choose $\epsilon$ of order the disc [disk scale height](../../../../../../disk-scale-height.md) $H$. There is no universal exact numerical choice: a true vertical [mass density](../../../../../../density.md) profile produces the Fourier reduction factor $\Sigma^{-1}\int\rho(z)e^{-k|z|}dz$, which is not generally $e^{-k\epsilon}$. Matching the long-wave term gives $\epsilon=\langle|z|\rangle_\rho$, the [vertical-profile softening match](../../../../../../vertical-profile-softening-match.md). For an exponential vertical profile this mean is $H$, while its full reduction factor is $(1+kH)^{-1}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
