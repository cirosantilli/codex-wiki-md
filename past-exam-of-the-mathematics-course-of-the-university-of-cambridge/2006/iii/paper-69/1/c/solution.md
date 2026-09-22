<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the transverse displacement as $\mathbf s$ and take the common line-of-sight interval to be $[0,L]$. The [rotation measure](../../../../../../rotation-measure.md) is a line integral of the [magnetic field](../../../../../../magnetic-field.md), so its [correlation](../../../../../../pearson-correlation-coefficient.md) is

$$
C_{\mathrm{RM}}(\mathbf s)=a_0^2n_e^2\int_0^L dz\int_0^L dz'\,C_{zz}(\mathbf s,z-z').
$$

Substitute the [Fourier inversion](../../../../../../fourier-inversion-theorem.md) of the [solenoidal isotropic spectral tensor](../../../../../../solenoidal-isotropic-spectral-tensor.md). Keeping the finite observation length gives the exact windowed expression

$$
C_{\mathrm{RM}}(\mathbf s)=a_0^2n_e^2\int\frac{d^3k}{(2\pi)^3}H(k)\left(1-\frac{k_z^2}{k^2}\right)e^{i\mathbf k_\perp\cdot\mathbf s}\left|\int_0^L e^{ik_z z}\,dz\right|^2.
$$

The allowed extension of the longitudinal displacement integral to the whole real line is the [long-path projection of a magnetic correlation](../../../../../../long-path-projection-of-a-magnetic-correlation.md). It applies when $L$ is much larger than the [correlation length](../../../../../../correlation-length.md): equivalently, the squared window becomes $2\pi L\delta(k_z)$ inside the [integral](../../../../../../integral.md). The [Dirac delta function](../../../../../../dirac-delta-function.md) sets $k_z=0$, leaving

$$
\boxed{C_{\mathrm{RM}}(s)\simeq a_0^2n_e^2L\int\frac{d^2k_\perp}{(2\pi)^2}H(k_\perp)e^{i\mathbf k_\perp\cdot\mathbf s}.}
$$

[Statistical isotropy](../../../../../../statistical-isotropy.md) makes this a function of $s=|\mathbf s|$. The displayed two-dimensional relation is the intended long-path approximation; the preceding windowed formula accounts for finite-length edge effects.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
