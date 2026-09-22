<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The concern is that the rapid-decay assumptions need not be preserved by the dynamics. In a constant-density [incompressible flow](../../../../../../incompressible-flow.md), the divergence of the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) gives the [pressure Poisson equation for incompressible flow](../../../../../../pressure-poisson-equation-for-incompressible-flow.md), with $\pi=p/\rho$:

$$
\nabla^2\pi=-\partial_i\partial_j(u_iu_j).
$$

For a localized eddy, inversion with the free-space [Green function](../../../../../../green-s-function.md) and two integrations by parts yield

$$
\pi(\boldsymbol r)=\frac1{4\pi}\int u_i(\boldsymbol y)u_j(\boldsymbol y)
\partial_{y_i}\partial_{y_j}\frac1{|\boldsymbol r-\boldsymbol y|}d^3y.
$$

At large separation the differentiated kernel has leading form $(3n_in_j-\delta_{ij})/r^3$. Thus an anisotropic stress moment of an individual eddy produces a quadrupolar [fluid pressure](../../../../../../fluid-pressure.md) of order $r^{-3}$, even if the [velocity](../../../../../../velocity.md) source is spatially localized. Correlating that [fluid pressure](../../../../../../fluid-pressure.md) with local $u_x^2$ allows $\langle u_x^2p'\rangle=O(r^{-3})$. Isotropy may cancel a mean multipole but does not automatically cancel such a mixed fourth-order statistic.

The triple-correlation evolution contains a pressure-gradient term of the form $-\langle u_x^2\partial_{x'}\pi'\rangle$, so these [long-range pressure correlations in turbulence](../../../../../../long-range-pressure-correlations-in-turbulence.md) can generate a longitudinal triple-correlation tail $K\sim ar^{-4}$. With $L=0$, part (ii) then gives $\dot I=8\pi u^3a$, which need not vanish. This is the substance of the objection to deducing exact conservation from initially short [velocity](../../../../../../velocity.md) correlations. Batchelor and Proudman's original long-range calculation concerned anisotropic turbulence; extending it to isotropic decay requires the appropriate higher-order correlations and allows cancellations. A permitted tail is not a proof that its coefficient stays appreciable in fully developed turbulence.

This possibility appealed to workers constructing heuristic [turbulence closures](../../../../../../turbulence-closure.md). A closure that generated a changing low-wavenumber $k^4$ coefficient and a decay exponent different from $10/7$ could then be viewed as representing a pressure-mediated effect, rather than as automatically violating a universal invariant. The closure's far-field coefficient still needs physical validation; closure-generated nonconservation does not itself prove the true dynamics nonconserving.

For evidence available before this exam, [the 2006 simulations of Ishida, Davidson and Kaneda](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/on-the-decay-of-isotropic-turbulence/72E017B53646320E97C378A2F6B94C0E) found that $I$ approached an approximately constant value after a transient when the box was much larger than the [integral scale of turbulence](../../../../../../integral-scale-of-turbulence.md) and the [Reynolds number](../../../../../../reynolds-number.md) was large. The energy decay was correspondingly close to $u^2\sim t^{-10/7}$. **The observed conclusion was approximate late-time conservation in that regime**, indicating weak net long-range triple-correlation transfer, rather than exact conservation for every initial condition, box size or Reynolds number.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
