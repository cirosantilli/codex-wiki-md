<h1 id="section-a-ii/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a positive [photoresist](../../../../../../photoresist.md), let $D_r$ be the largest dose retaining the nominal film and $D_c$ the clearing dose. With the conventional [photoresist contrast](../../../../../../photoresist-contrast.md) definition,

$$
\gamma=\left[\log_{10}(D_c/D_r)\right]^{-1},\qquad r=\frac{D_c}{D_r}=10^{1/\gamma}.
$$

For a sinusoidal aerial image, the bright-to-dark dose ratio is $(1+C)/(1-C)$, where $C$ is the [Michelson contrast](../../../../../../michelson-contrast.md). A dose window that clears bright regions while retaining dark regions requires

$$
\frac{1+C}{1-C}\geq r,\qquad
\boxed{C_{\min}=\frac{10^{1/\gamma}-1}{10^{1/\gamma}+1}}.
$$

This assumes a fully modulated input pattern and that the plotted [modulation transfer function](../../../../../../modulation-transfer-function.md) gives the aerial-image contrast. It is a dose-window criterion, not a statement that the resist creates optical information absent from the image.[§2.6.1, equation 2.6: logarithmic resist-dose contrast](../../../../../../contrast-and-important-properties-by-heinrich-kirchauer.md)

The two thresholds are approximately

$$
\gamma=1.05:\ C_{\min}=0.799,\qquad
\gamma=3.72:\ C_{\min}=0.300.
$$

Reading their intersections with the supplied curve gives, to graphical accuracy,

$$
\boxed{\nu_{\max}\simeq0.40\nu_0\quad\text{and}\quad0.60\nu_0}
$$

for the lower- and higher-contrast resists respectively. These are the results independent of the dimensional frequency convention. Their minimum full periods are $P=1/\nu$, and equal line/space widths are half those periods:

$$
\boxed{P_{\min}\simeq\frac{2.50}{\nu_0},\ \frac{1.67}{\nu_0};\qquad
w_{\min}\simeq\frac{1.25}{\nu_0},\ \frac{0.833}{\nu_0}}.
$$

An ArF [excimer laser](../../../../../../excimer-laser.md) uses $\lambda\simeq193\,\mathrm{nm}$. A numerical length requires specifying what the caption's “Rayleigh limit” means. Taking it literally as the reciprocal of the [Rayleigh criterion](../../../../../../rayleigh-criterion.md) point separation gives

$$
R_R=\frac{0.61\lambda}{\mathrm{NA}}=294.3\,\mathrm{nm},\qquad \nu_0=1/R_R,
$$



$$
\boxed{P_{\min}\simeq736,\ 491\,\mathrm{nm};\qquad
w_{\min}\simeq368,\ 245\,\mathrm{nm}}.
$$

If instead the graph uses the common **incoherent-cutoff normalization** $\nu_0=2\mathrm{NA}/\lambda$, the widths are **$302\,\mathrm{nm}$ and $201\,\mathrm{nm}$**, with periods twice those values. The caption does not explicitly provide an equation for $\nu_0$ or define whether “feature size” means period or half-pitch, so these conventions must not be silently mixed. The higher-contrast resist resolves the higher normalized frequency in either convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Section A(ii)](../../../section-a-ii.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
