<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [instantaneous recycling approximation](../../../../../../instantaneous-recycling-approximation.md) and treat the [interstellar medium](../../../../../../interstellar-medium.md) as well mixed. If [star formation](../../../../../../star-formation.md) initially consumes mass $dM$, returning a fraction $\beta$ leaves locked stellar mass $ds=(1-\beta)dM$. The original metal mass removed from the [interstellar medium](../../../../../../interstellar-medium.md) is $Z_i\,dM$. Of this original material, $\beta fZ_i\,dM$ returns and remains in the [galaxy](../../../../../../galaxy-split.md). In addition, the [stellar yield](../../../../../../stellar-yield.md) produces fresh metal mass $y_i\,ds$, of which the retained part is $fy_i\,ds$. Therefore metal accounting gives

$$
d(gZ_i)=-Z_i\,dM+\beta fZ_i\,dM+fy_i\,ds,
\qquad
\boxed{\frac{d(gZ_i)}{ds}=-\frac{1-\beta f}{1-\beta}Z_i+y_if.}
$$

This is the [retained-ejecta chemical evolution](../../../../../../retained-ejecta-chemical-evolution.md) equation. It assumes that the same retention fraction applies to original and newly synthesized metals. Pristine [galactic gas inflow](../../../../../../galactic-gas-inflow.md) can change $g$ without contributing to $d(gZ_i)$; enriched [galactic gas inflow](../../../../../../galactic-gas-inflow.md) would require an additional metal source. Here $0\leq\beta<1$, and $0\leq f\leq1$.

A [star](../../../../../../star.md) inherits the [gas-phase metallicity](../../../../../../gas-phase-metallicity.md) at its birth. Suppose enrichment is monotone and a fixed [initial mass function](../../../../../../initial-mass-function.md), with an appropriate surviving tracer selection, produces $\kappa$ observable [stars](../../../../../../star.md) per unit locked mass. For two birth abundances $Z_a<Z_b$, the relative count is

$$
N(Z_a<Z_i<Z_b)=\kappa\,[s(Z_b)-s(Z_a)],
\qquad
\boxed{\frac{dN}{dZ_i}=\kappa\frac{ds}{dZ_i}.}
$$

Thus $s(Z_i)$ is proportional to the cumulative [metallicity distribution function](../../../../../../metallicity-distribution-function.md); its derivative gives the differential [metallicity distribution function](../../../../../../metallicity-distribution-function.md). The normalized distribution after final locked mass $s_\infty$ is $s_\infty^{-1}ds/dZ_i$. For logarithmic abundances, the [logarithmic metallicity distribution](../../../../../../logarithmic-metallicity-distribution.md) instead has $dN/d\log_{10}Z_i=(\ln10)Z_i\,dN/dZ_i$.

The fixed [initial mass function](../../../../../../initial-mass-function.md) and survival selection matter: a mass distribution is not automatically the number distribution of every presently observable [star](../../../../../../star.md). If enrichment is nonmonotone, add the contributions $\kappa|ds/dZ_i|$ from all birth-time branches attaining that abundance, rather than using one inverse.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
