<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A newly formed [stellar population](../../../../../../stellar-population.md) inherits the current [gas-phase metallicity](../../../../../../gas-phase-metallicity.md). Eliminate time between locked-mass growth and enrichment:

$$
dM_s=-dM_g,\qquad M_g\,dZ=Y\,dM_s.
$$

For $Y>0$, integration from pristine gas gives $M_g=M_0e^{-Z/Y}$ and hence the [closed-box metallicity distribution](../../../../../../closed-box-metallicity-distribution.md)

$$
\frac{dM_s}{dZ}=\frac{M_0}{Y}e^{-Z/Y}.
$$

To obtain numbers rather than mass, specify a fixed [initial mass function](../../../../../../initial-mass-function.md) and count a long-lived tracer population. Let $\eta$ be its number of surviving [stars](../../../../../../star.md) per unit locked stellar mass. At the final [gas-phase metallicity](../../../../../../gas-phase-metallicity.md) $Z_f$,

$$
\boxed{\frac{dN}{dZ}=\frac{\eta M_0}{Y}e^{-Z/Y},\qquad 0\le Z\le Z_f,}
$$

with zero density outside that interval. The cumulative count is $N(<Z)=\eta M_0(1-e^{-Z/Y})$ within the interval, and the normalized [metallicity distribution function](../../../../../../metallicity-distribution-function.md) is

$$
p(Z)=\frac{e^{-Z/Y}}{Y(1-e^{-Z_f/Y})}.
$$

These equations do not use $\psi(t)$: any positive [star formation rate](../../../../../../star-formation-rate.md) gives the same distribution under the same chemical assumptions. If the tracer number is instead normalized per gross formed mass, replace $\eta$ by that normalization divided by $1-F$. Short-lived [stars](../../../../../../star.md) require an age-dependent survival factor and generally do not follow this number distribution. In a [logarithmic metallicity distribution](../../../../../../logarithmic-metallicity-distribution.md), $dN/d\log_{10}Z=(\ln10)Z\,dN/dZ$; its interior peak is at $Z=Y$, whereas the distribution per linear interval decreases from $Z=0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
