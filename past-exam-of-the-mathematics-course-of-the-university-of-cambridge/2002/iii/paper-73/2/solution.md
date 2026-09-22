<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Hawking's area theorem](../../../../../hawking-s-area-theorem.md) states that the area of later cross-sections of a classical future [event horizon](../../../../../event-horizon.md) cannot be smaller than that of earlier cross-sections, including the sum over initially disconnected components. Its hypotheses include the [null energy condition](../../../../../null-energy-condition.md), the Einstein equations, and the global regularity/predictability conditions that exclude future naked pathologies of the horizon generators. A convenient sufficient version assumes those generators are future complete. Without the energy and global hypotheses the assertion is not unconditional.

Let $k^a$ be an affinely parametrized null generator, with expansion $\theta$. Because the horizon is a [null hypersurface](../../../../../null-hypersurface.md), the generator congruence has zero [null twist](../../../../../null-twist.md). The [Null Raychaudhuri equation](../../../../../null-raychaudhuri-equation.md) in four dimensions gives

$$
\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}-R_{ab}k^ak^b
\le-\frac12\theta^2.
$$

The [null shear](../../../../../null-shear.md) square is nonnegative and the [null energy condition](../../../../../null-energy-condition.md) makes $R_{ab}k^ak^b=8\pi G T_{ab}k^ak^b\ge0$; a cosmological term has zero null contraction. Suppose $\theta(\lambda_0)<0$. Integration of this inequality forces $\theta\to-\infty$ within affine distance at most $2/|\theta(\lambda_0)|$. This produces a focal point to the initial horizon cross-section. Beyond it the [null geodesic](../../../../../null-geodesic.md) cannot remain on an [achronal boundary](../../../../../achronal-boundary.md), whereas an [event horizon](../../../../../event-horizon.md) is precisely such a boundary. Future completeness, or the corresponding standard predictability condition ensuring continuation over this interval, gives the contradiction. Hence

$$
\theta\ge0,\qquad \frac{d(dA)}{d\lambda}=\theta\,dA\ge0.
$$

This proves the local area increase along every smooth generator bundle. Generators can enter the horizon at past crease points, but cannot leave through future endpoints on a regular horizon under these hypotheses. New generators add area, rather than subtracting it, so the result extends across the nonsmooth merger set and to whole horizon cross-sections. This is the [future-complete horizon focusing proof of the area theorem](../../../../../future-complete-horizon-focusing-proof-of-the-area-theorem.md).

Choose an early cross-section with the two separate components of areas $A_1,A_2$, and a later cross-section of the settled merged hole. Following the old generators forward maps their area elements injectively into the later horizon; a future crossing/focal point would violate the same achronality argument. Each element has nondecreased area. Any additional generators contribute nonnegative area, giving

$$
\boxed{A_3\ge A_1+A_2.}
$$

This is a comparison of event-horizon cross-sections, not an assertion that set containment alone bounds the areas of arbitrary apparent horizons.

For a [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md), $r_h=2Gm/c^2$ and $A=4\pi r_h^2=16\pi G^2m^2/c^4$. Applying the merger inequality to the two equal initial masses and the final Schwarzschild mass gives

$$
\frac{16\pi G^2M^2}{c^4}\ge\frac{32\pi G^2m^2}{c^4},\qquad
\boxed{M\ge\sqrt2\,m.}
$$

For initially well-separated holes at rest, with no extra incoming energy or external work, energy conservation gives $E_{\rm rad}=(2m-M)c^2$. The [area bound on equal-mass Schwarzschild merger radiation](../../../../../area-bound-on-equal-mass-schwarzschild-merger-radiation.md) is consequently

$$
\boxed{E_{\rm rad}\le(2-\sqrt2)mc^2,\qquad
\frac{E_{\rm rad}}{2mc^2}\le1-\frac1{\sqrt2}\simeq29.3\%.}
$$

This is the maximum permitted by the area/energy inequalities, not a demonstration that a dynamical merger attains it. A reversible limiting area change would be needed to saturate the bound. If initial separation, binding energy or external agents change the initial total energy, replace $2mc^2$ by that energy when computing escaped radiation. Quantum evaporation does not contradict the theorem: the classical energy-condition hypotheses are not retained unchanged in that setting.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
