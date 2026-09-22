<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For this question use the normalized [magnetic scalar potential](../../../../../magnetic-scalar-potential.md) $\mathcal U$ defined by $\mathbf B=(\mu_0/4\pi)\nabla\mathcal U$. The previous question instead includes $\mu_0/4\pi$ in its scalar potential; its $U$ equals $(\mu_0/4\pi)\mathcal U$. This normalization change in the paper must be kept separate from the kernel calculation.

Take the radial component of the [Geselowitz formula](../../../../../geselowitz-formula.md). On the spherical boundary, $\mathbf n'$ is parallel to $\mathbf r'$, and

$$
[\mathbf n'\times(\mathbf r-\mathbf r')]\cdot\widehat{\mathbf r}=0.
$$

Thus the surface-current term contributes no radial [magnetic field](../../../../../magnetic-field.md). The primary [Biot-Savart law](../../../../../biot-savart-law.md) term gives, along a fixed direction $\widehat{\mathbf r}$,

$$
\partial_r\mathcal U
=\left[\mathbf Q\times\frac{\mathbf r-\mathbf r_0}{|\mathbf r-\mathbf r_0|^3}\right]\cdot\widehat{\mathbf r}
=-\frac{(\mathbf Q\times\mathbf r_0)\cdot\widehat{\mathbf r}}
{|r\widehat{\mathbf r}-\mathbf r_0|^3}.
$$

Choose $\mathcal U\to0$ at infinity. Integrating this equation fixes the full potential along every ray, giving

$$
\mathcal U=(\mathbf Q\times\mathbf r_0)\cdot\widehat{\mathbf r}
\int_r^\infty\frac{ds}{|s\widehat{\mathbf r}-\mathbf r_0|^3}.
$$

To express it as a source-position derivative, define

$$
\phi(\mathbf r;\mathbf r_0)=\int_r^\infty\frac{ds}{s|s\widehat{\mathbf r}-\mathbf r_0|}.
$$

With $\mathbf W=\mathbf Q\times\mathbf r_0$, differentiating the integrand gives

$$
\mathbf W\cdot\nabla_{\mathbf r_0}\frac1{|s\widehat{\mathbf r}-\mathbf r_0|}
=\frac{s\mathbf W\cdot\widehat{\mathbf r}}{|s\widehat{\mathbf r}-\mathbf r_0|^3},
$$

so $\mathcal U=\mathbf W\cdot\nabla_{\mathbf r_0}\phi$ as required.

Let $b=|\mathbf r_0|$ and $P=|\mathbf r-\mathbf r_0|$. An elementary antiderivative gives the [spherical current-dipole logarithmic kernel](../../../../../spherical-current-dipole-logarithmic-kernel.md)

$$
\boxed{\phi(\mathbf r;\mathbf r_0)=\frac1b\log\frac{r+P+b}{r+P-b}.}
$$

For $r>a>b$, both logarithm arguments are positive. Its radial derivative is $-1/(rP)$ and its limit at infinity is zero, which verifies the preceding integral. At $b=0$ use the continuous limit $\phi=1/r$.

For a direct check, differentiating along $\mathbf W$ leaves $b$ unchanged and gives $\mathbf W\cdot\nabla_{\mathbf r_0}P=-\mathbf W\cdot\mathbf r/P$. Since

$$
F=rP^2+P\mathbf r\cdot(\mathbf r-\mathbf r_0)
=\frac P2[(r+P)^2-b^2],
$$

one obtains

$$
\boxed{\mathcal U=\frac{(\mathbf Q\times\mathbf r_0)\cdot\mathbf r}{F}.}
$$

Its gradient is the [Sarvas formula](../../../../../sarvas-formula.md). The sphere radius and [electrical conductivity](../../../../../electrical-conductivity.md) disappear from this exterior magnetic result because spherical symmetry removed the radial contribution of the return currents. The original derivation and spherical-conductor assumptions are discussed in [Sarvas's paper](https://pubmed.ncbi.nlm.nih.gov/3823129/).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
