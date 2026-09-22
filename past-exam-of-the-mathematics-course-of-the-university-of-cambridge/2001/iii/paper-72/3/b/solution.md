<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Ginzburg criterion](../../../../../../ginzburg-criterion.md) tests whether fluctuations on the scale of one [correlation volume](../../../../../../correlation-volume.md) are small compared with the squared equilibrium [order parameter](../../../../../../order-parameter.md). In the scalar quartic [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) of part (a), the ordered mean-field value is $M^2=|r|/u$, and its longitudinal [correlation length](../../../../../../correlation-length.md) is proportional to $(c/|r|)^{1/2}$.

Average the fluctuation field over a region of size $\xi$. Its smoothing factor selects momenta of order $\xi^{-1}$ or smaller. The Gaussian [correlation function](../../../../../../correlation-function.md) then gives, up to a positive dimension-dependent constant,

$$
\langle(\delta\phi_\xi)^2\rangle
\asymp\int_{|q|\lesssim\xi^{-1}}\frac{d^dq}{(2\pi)^d}\frac1{cq^2+2|r|}
\asymp\frac1c\xi^{2-d}
\asymp c^{-d/2}|r|^{(d-2)/2}.
$$

The last step follows directly by setting $q=\sqrt{|r|/c}\,k$. Dividing by $M^2$ proves the [correlation-volume derivation of the scalar Ginzburg ratio](../../../../../../correlation-volume-derivation-of-the-scalar-ginzburg-ratio.md):

$$
\boxed{\mathcal G=\frac{\langle(\delta\phi_\xi)^2\rangle}{M^2}
\asymp u c^{-d/2}|r|^{(d-4)/2}\ll1.}
$$

For $d<4$, the ratio diverges as the transition is approached, so there is a fluctuation-dominated [critical region of a phase transition](../../../../../../critical-region-of-a-phase-transition.md) in which [mean-field critical exponents](../../../../../../mean-field-critical-exponent.md) cannot be trusted. With $r=r_0t$, an estimate of its width is

$$
|t|\lesssim t_G,\qquad t_G\asymp\frac1{r_0}\left(\frac{u^2}{c^d}\right)^{1/(4-d)},
$$

in fixed microscopic units. Its numerical coefficient depends on the averaging convention and microscopic normalization.

For $d>4$, the ratio tends to zero and the long-distance [mean-field approximation](../../../../../../mean-field-approximation.md) becomes self-consistent. Four is therefore the ordinary quartic [upper critical dimension](../../../../../../upper-critical-dimension.md). At $d=4$ this test is marginal: its thermal power is zero, and the running quartic interaction produces logarithmic corrections. The [marginal Ginzburg criterion](../../../../../../marginal-ginzburg-criterion.md) alone cannot decide those logarithms. Short-distance contributions to an unaveraged variance renormalize the coefficients; they should not be mistaken for the long-wavelength fluctuations used in this criterion. Nor does the criterion by itself prove that a proposed ordered phase exists below its [lower critical dimension](../../../../../../lower-critical-dimension.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
