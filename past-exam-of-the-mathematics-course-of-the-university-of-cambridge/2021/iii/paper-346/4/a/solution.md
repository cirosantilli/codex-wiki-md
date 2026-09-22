<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a statistically homogeneous and isotropic density contrast,

$$
\boxed{
\xi(r)=\langle\delta(\mathbf x)
\delta(\mathbf x+\mathbf r)\rangle,
\qquad r=|\mathbf r|
}.
$$

Using the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\delta(\mathbf x)=\int\frac{d^3k}{(2\pi)^3}
\delta_{\mathbf k}e^{i\mathbf k\cdot\mathbf x}
$$

and translational invariance gives

$$
\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle
=(2\pi)^3\delta_D(\mathbf k-\mathbf k')P(k),
$$

with

$$
\boxed{
P(k)=\int d^3r\,\xi(r)e^{-i\mathbf k\cdot\mathbf r}
}.
$$

At one point,

$$
\boxed{
\sigma^2=\xi(0)
=\frac1{2\pi^2}\int_0^\infty k^2P(k)\,dk
}.
$$

For a spherical top-hat volume $V=4\pi R^3/3$,

$$
\boxed{
\sigma^2(R)
=\frac1{V^2}\int_Vd^3x_1\int_Vd^3x_2\,
\xi(|\mathbf x_1-\mathbf x_2|)
}.
$$

The overlap of two radius-$R$ balls separated by $r\leq2R$ is

$$
V_{\rm ov}(r)=V\left(
1-\frac{3r}{4R}+\frac{r^3}{16R^3}
\right).
$$

Therefore

$$
\boxed{
\sigma^2(R)
=\frac3{R^3}\int_0^{2R}
r^2\xi(r)
\left(1-\frac{3r}{4R}
+\frac{r^3}{16R^3}\right)dr
}.
$$

For $\xi(r)=(r/r_0)^{-1.8}$,

$$
\sigma^2(R)=J_2\left(\frac{r_0}{R}\right)^{1.8},
\qquad
J_2=\frac{72}
{2^{1.8}(3-1.8)(4-1.8)(6-1.8)}
\simeq1.865.
$$

Thus

$$
\boxed{
\sigma_8
=\sqrt{J_2}\left(\frac58\right)^{0.9}
\simeq0.895
}.
$$

This calculation assumes that the observed galaxies trace the matter field with unit, scale-independent [galaxy bias](../../../../../../galaxy-bias.md), and that the fitted [power law](../../../../../../power-law.md) remains valid throughout the [top-hat](../../../../../../spherical-top-hat-window-function.md) separations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 346](../../../paper-346-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
