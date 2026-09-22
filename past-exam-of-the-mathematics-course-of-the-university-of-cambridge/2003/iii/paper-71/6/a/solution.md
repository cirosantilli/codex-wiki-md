<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The printed diagram and the word “parallel” describe a [Kelvin-Voigt model](../../../../../../kelvin-voigt-model.md), not a series [Maxwell fluid](../../../../../../linear-maxwell-fluid.md). In the depicted model both elements have displacement $x$ and their [forces](../../../../../../force.md) add:

$$
\boxed{F=kx+\mu\dot x.}
$$

For $x=ae^{i\omega t}$ and the convention $G(\omega)=F_{\rm amplitude}/x_{\rm amplitude}$,

$$
\boxed{G(\omega)=k+i\omega\mu,\qquad G'=k,\quad G''=\omega\mu.}
$$

The [storage modulus](../../../../../../storage-modulus.md) and [loss modulus](../../../../../../loss-modulus.md) here are element stiffnesses with units $\mathrm{N\,m^{-1}}$; conversion to stress/[strain](../../../../../../strain.md) moduli requires a geometric factor. If “response” instead denotes displacement per [force](../../../../../../force.md), it is the compliance $1/(k+i\omega\mu)$. Specifying which ratio is used removes that convention ambiguity. The mean dissipated power is $\mu\omega^2|a|^2/2$, confirming the positive loss sign for $e^{i\omega t}$.

For completeness, the actual series [Maxwell fluid](../../../../../../linear-maxwell-fluid.md) analogue has a common [force](../../../../../../force.md) and additive [spring](../../../../../../spring.md)/[dashpot](../../../../../../dashpot.md) extensions. Thus $\dot x=\dot F/k+F/\mu$. With $\tau=\mu/k$,

$$
G_M(\omega)=\frac{k i\omega\tau}{1+i\omega\tau},\qquad G_M'=\frac{k\omega^2\tau^2}{1+\omega^2\tau^2},\qquad G_M''=\frac{k\omega\tau}{1+\omega^2\tau^2}.
$$

These different functions cannot both describe the printed parallel arrangement. The distinction also changes the [elastic beam](../../../../../../elastic-beam.md)'s response to a constant load.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
