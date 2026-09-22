<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [Spatially flat FLRW metric](../../../../../../spatially-flat-flrw-metric.md), neglect metric perturbations and write $\phi=\bar\phi+\delta\phi$. The kinetic invariant is then exactly quadratic in field derivatives:

$$
X=\frac12(\dot{\bar\phi}+\delta\dot\phi)^2-\frac1{2a^2}(\partial_i\delta\phi)^2.
$$

Subtracting $\bar X=\dot{\bar\phi}^{2}/2$ gives **the second-order expansion**

$$
\boxed{\delta X=\dot{\bar\phi}\,\delta\dot\phi+\frac12\delta\dot\phi^2-\frac1{2a^2}(\partial_i\delta\phi)^2.}
$$

In the derivative-dominated approximation, $\delta\phi=-\dot{\bar\phi}\zeta/H$ with $\dot{\bar\phi}/H$ treated as slowly varying. Thus $\delta\dot\phi\simeq-\dot{\bar\phi}\dot\zeta/H$ and

$$
\delta X_1=-\frac{2\bar X}{H}\dot\zeta,\qquad
\delta X_2=\frac{\bar X}{H^2}\left[\dot\zeta^2-\frac{(\partial_i\zeta)^2}{a^2}\right].
$$

This uses the linear flat-to-comoving slicing relation. Differentiating its slowly varying coefficient would add terms involving undifferentiated $\zeta$; it is not an exact nonlinear gauge transformation, and those neglected terms do not alter the leading pure $\dot\zeta^3$ coefficient computed here.

Only $P_{,XX}\delta X_1\delta X_2$ and $P_{,XXX}\delta X_1^3/6$ contribute to the requested three-time-derivative term. Therefore **the directly evaluated cubic coefficient is**

$$
\boxed{C=-\frac{a^3}{H^3}\left(2\bar X^2P_{,XX}+\frac43\bar X^3P_{,XXX}\right)
=\frac{2a^3\bar X^2P_{,XX}}{H^3}\mathcal A,
\quad\mathcal A=-1-\frac{2\bar XP_{,XXX}}{3P_{,XX}}.}
$$

This is the [derivative-cubic coefficient of a noncanonical scalar](../../../../../../derivative-cubic-coefficient-of-a-noncanonical-scalar.md). For a physical $P(X,\phi)$ [scalar field](../../../../../../scalar-field.md) theory, differentiating $\rho=2XP_{,X}-P$ at fixed $\phi$ gives $\rho_{,X}=P_{,X}+2XP_{,XX}$. Its sound speed is consequently

$$
\boxed{c_s^2=\frac{P_{,X}}{P_{,X}+2\bar XP_{,XX}},\qquad
C=\frac{a^3\epsilon}{H}\frac{1-c_s^2}{c_s^2}\mathcal A,
\qquad\epsilon=\frac{\bar XP_{,X}}{H^2}.}
$$

The minus sign printed in the denominator of $c_s^2$ reverses the asserted coefficient identity; it must be a plus. The printed background equation also lacks a power: it is $3H^2=\rho$ in the stated reduced-Planck units. A stable propagating scalar has positive time-kinetic coefficient $P_{,X}+2XP_{,XX}$ and positive gradient coefficient $P_{,X}$, as summarized by [noncanonical scalar kinetic stability](../../../../../../noncanonical-scalar-kinetic-stability.md).

The unfactored expression for $C$ stays meaningful if $P_{,XX}=0$, although $\mathcal A$ separately then need not exist. For a canonical kinetic term with no higher kinetic derivatives, $C=0$. The [cubic curvature action for a P(X, phi) scalar field](../../../../../../cubic-curvature-action-for-a-p-x-phi-scalar-field.md) can include other vertices and gravitational terms; they are outside this requested derivative coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
