<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Minkowski metric](../../../../../../minkowski-metric.md) $\eta_{mn}=\operatorname{diag}(-1,1,\ldots,1)$ and units with [speed of light](../../../../../../speed-of-light.md) one. The contractions are $P^2=\eta^{mn}P_mP_n$ and $(TX')^2=T^2\eta_{mn}(X^m)'(X^n)'$; $(X^m)'P_m$ and $\dot X^mP_m$ pair a [vector](../../../../../../vector.md) with a [covector](../../../../../../covector.md) without another metric. The [Lagrange multipliers](../../../../../../lagrange-multiplier.md) impose the two [first-class constraints](../../../../../../first-class-constraint.md)

$$
\mathcal H=\tfrac12(P^2+T^2X'^2)=0,\qquad \mathcal D=X'\cdot P=0.
$$

They generate [worldsheet diffeomorphisms](../../../../../../worldsheet-diffeomorphism.md), so the [phase space](../../../../../../phase-space.md) contains both constrained directions and [gauge redundancy](../../../../../../gauge-redundancy.md). Two [first-class constraints](../../../../../../first-class-constraint.md) remove two [canonical pairs](../../../../../../canonical-pair.md), leaving $D-2$ physical [degrees of freedom](../../../../../../degree-of-freedom.md) per point.

In [Monge gauge](../../../../../../monge-gauge.md), $X^0=t$ and $X^1=\sigma$. Write the transverse [canonical variables](../../../../../../canonical-variables.md) as $\boldsymbol X=(X^2,\ldots,X^{D-1})$ and $\boldsymbol P=(P_2,\ldots,P_{D-1})$. Solving the [first-class constraints](../../../../../../first-class-constraint.md) gives

$$
P_1=-\boldsymbol X'\cdot\boldsymbol P,\qquad
P_0=-\mathcal E,\qquad
\mathcal E=\sqrt{T^2(1+|\boldsymbol X'|^2)+|\boldsymbol P|^2+(\boldsymbol X'\cdot\boldsymbol P)^2}.
$$

The negative root selects positive [energy](../../../../../../energy.md). Substitution into the [phase-space action](../../../../../../phase-space-action.md) gives the [Hamiltonian](../../../../../../hamiltonian.md) reduction

$$
\boxed{I_{\mathrm{red}}=\int dt\int_0^\pi d\sigma\,
\bigl(\dot{\boldsymbol X}\cdot\boldsymbol P-\mathcal E\bigr).}
$$

For a static segment, $\boldsymbol P=0$, its [proper length](../../../../../../proper-length.md) element is $d\ell=\sqrt{1+|\boldsymbol X'|^2}\,d\sigma$, and $\mathcal E\,d\sigma=T\,d\ell$. Thus **the [string tension](../../../../../../string-tension.md) is the [rest energy](../../../../../../rest-energy.md) per unit [proper length](../../../../../../proper-length.md)**. In particular a straight resting segment has $\mathcal E=T$. [Monge gauge](../../../../../../monge-gauge.md) is a local choice on a [string embedding map](../../../../../../string-embedding-map.md) for which $X^1$ is a valid coordinate; it need not cover folded strings or all endpoint configurations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
