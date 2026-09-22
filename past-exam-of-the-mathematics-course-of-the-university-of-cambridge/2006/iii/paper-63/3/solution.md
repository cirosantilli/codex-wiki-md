<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [black-hole area theorem](../../../../../hawking-s-area-theorem.md) is a statement about classical future [event horizons](../../../../../event-horizon.md), with both a local focusing condition and global horizon regularity assumptions. Assume the [null energy condition](../../../../../null-energy-condition.md), an appropriately predictable exterior and no future termination of horizon generators before the focusing argument can be applied. Future-complete generators provide a particularly direct sufficient version of the last assumption. [Strong asymptotic predictability](../../../../../strong-asymptotic-predictability.md) is the usual global condition used to exclude the pathological alternatives; the energy condition by itself is not the whole theorem.

On a smooth part of the horizon, choose a future-directed affinely parametrized generator $\ell^a$ and [affine parameter](../../../../../affine-parameter.md) $\lambda$. Its expansion $\theta$ is the fractional rate of change of an infinitesimal transverse area element:

$$
\frac{d}{d\lambda}\log dA=\theta.
$$

The horizon is a null hypersurface, so its generator congruence is hypersurface-orthogonal and has zero twist. The transverse screen metric is positive definite, hence $\sigma_{ab}\sigma^{ab}\geq0$. In four dimensions the [Null Raychaudhuri equation](../../../../../null-raychaudhuri-equation.md) is

$$
\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}
-R_{ab}\ell^a\ell^b.
$$

The [Einstein field equations](../../../../../einstein-field-equations.md) and the [null energy condition](../../../../../null-energy-condition.md) imply the [null convergence condition](../../../../../null-convergence-condition.md) $R_{ab}\ell^a\ell^b\geq0$, so $\theta'\leq-\theta^2/2$.

Suppose $\theta_0<0$ at $\lambda_0$. As long as the congruence remains smooth, integrating $d(1/\theta)/d\lambda\geq1/2$ shows focusing within affine distance at most $2/|\theta_0|$. Equivalently, comparison with the equality solution gives

$$
\theta(\lambda)\leq\frac{\theta_0}{1+\tfrac12\theta_0(\lambda-\lambda_0)}.
$$

Its denominator tends to zero at finite future affine parameter. The corresponding transverse area collapses, giving a [conjugate point to a spacelike surface](../../../../../conjugate-point-to-a-spacelike-surface.md). Beyond a focal point a generator cannot remain on an [achronal boundary](../../../../../achronal-boundary.md), since nearby points can then be joined by a timelike curve. But a regular future [event horizon](../../../../../event-horizon.md) is such a boundary, and its generators cannot leave it to the future. With the stated future-extension assumption this is a contradiction. Therefore $\theta\geq0$ on the smooth horizon.

Following generators from one horizon cross-section to a later one now gives a noncontracting area map. Generators entering at past endpoints or merger crease sets can add area, whereas the global hypotheses exclude generators disappearing from the future horizon. Consequently

$$
\boxed{A_{\rm later}\geq A_{\rm earlier}.}
$$

This is the [future-complete horizon focusing proof of the area theorem](../../../../../future-complete-horizon-focusing-proof-of-the-area-theorem.md). In $D$ spacetime dimensions, the coefficient $1/2$ is replaced by $1/(D-2)$ and the same proof gives a focusing distance at most $(D-2)/|\theta_0|$. It therefore also applies to the three-dimensional horizon cross-sections of the preceding five-dimensional example.

**A [cosmological constant](../../../../../cosmological-constant.md) does not invalidate the local focusing step.** Contract the modified [Einstein field equations](../../../../../einstein-field-equations.md) with the null generator. Since $g_{ab}\ell^a\ell^b=0$, both the scalar-curvature term and the $\Lambda$ term disappear:

$$
\boxed{R_{ab}\ell^a\ell^b=8\pi T_{ab}\ell^a\ell^b\geq0.}
$$

Thus a [cosmological constant preserves null convergence](../../../../../cosmological-constant-preserves-null-convergence.md), whatever its sign. Under suitable global assumptions for the relevant asymptotic region, the black-hole area argument still works. A nonzero $\Lambda$ changes the asymptotic geometry and can introduce cosmological horizons, so the statement concerns the appropriate future black-hole horizon; it is not an assertion that every horizon-like surface automatically obeys the same area ordering.

**A classical real canonical [massless scalar field](../../../../../massless-scalar-field.md) also preserves the area theorem's energy condition.** Its stress tensor has

$$
T_{ab}\ell^a\ell^b
=(\ell^a\partial_a\phi)^2
-\frac12(g_{ab}\ell^a\ell^b)g^{cd}\partial_c\phi\partial_d\phi
=\boxed{(\ell^a\partial_a\phi)^2\geq0.}
$$

This proof is independent of whether the field gradient is spacelike, timelike or null: the metric term vanishes and the remaining real square is nonnegative. It is the [null energy condition for a canonical scalar field](../../../../../null-energy-condition-for-a-canonical-scalar-field.md). Adding this field to other matter satisfying the [null energy condition](../../../../../null-energy-condition.md) retains null convergence. With the same global regularity assumptions, area still cannot decrease; when the derivative along a generator is nonzero, it supplies an additional nonnegative focusing source.

The conclusion uses the given minimally coupled classical stress tensor. A wrong-sign kinetic term or a nonminimal curvature coupling would require another calculation. Likewise, a renormalized quantum [stress-energy tensor](../../../../../stress-energy-tensor.md) need not obey the classical pointwise condition; the quantum radiation considered next is not covered by this classical proof.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
