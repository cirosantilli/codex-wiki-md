<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The basic object for [integration on an oriented manifold](../../../../../integration-on-an-oriented-manifold.md) of dimension $n$ is a top-degree [differential form](../../../../../differential-form-split.md). In an orientation-preserving chart, write $\alpha=f(x)\,dx^1\wedge\cdots\wedge dx^n$. Its integral is the ordinary integral of $f$, and the coordinate [change of variables](../../../../../change-of-variables-formula.md) formula ensures agreement on overlapping oriented charts. A [partition of unity](../../../../../partition-of-unity.md) combines these local integrals into a global one, provided the form has compact support or satisfies appropriate convergence conditions. Reversing orientation reverses the integral. No metric is needed, although a [pseudo-Riemannian metric](../../../../../pseudo-riemannian-metric.md) and orientation supply the volume form $\sqrt{|\det g|}\,dx^1\wedge\cdots\wedge dx^n$. On a nonorientable manifold one instead integrates densities, or appropriately twisted top forms.

A $k$-form is integrated over an oriented $k$-dimensional submanifold by its [pullback](../../../../../pullback-category-theory.md): if $X:C\to M$ is its embedding, $\int_C X^*\alpha$ is defined intrinsically on $C$. The [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md), with the induced boundary orientation, states

$$
\int_C d\beta=\int_{\partial C}\beta.
$$

One way to see why this global formula holds is to use an oriented chart and expand $d\beta$ as a sum of coordinate derivatives. The ordinary fundamental theorem of calculus gives the boundary contributions with their orientation signs. A [partition of unity](../../../../../partition-of-unity.md) reduces the manifold to such charts; the artificial internal boundary contributions cancel, leaving only the actual boundary. Compactness or compact support controls the sums and the boundary at infinity.

This immediately explains how [closed differential forms](../../../../../closed-differential-form.md) yield conservation laws. For a [closed differential form](../../../../../closed-differential-form.md) $\alpha$, cycles $C_1,C_2$ satisfying $C_2-C_1=\partial B$ have equal integrals:

$$
\int_{C_2}\alpha-\int_{C_1}\alpha=\int_Bd\alpha=0.
$$

Thus the integral pairs the [de Rham cohomology](../../../../../de-rham-cohomology.md) class of $\alpha$ with the [homology class](../../../../../homology-class.md) of the cycle. An [exact differential form](../../../../../exact-differential-form.md) integrates to zero on every closed cycle. A closed form need not be exact, and nonzero periods measure the global obstruction. If a spacetime current is represented by a closed $(n-1)$-form $J$, integrating over two [Cauchy surfaces](../../../../../cauchy-surface.md) gives a conserved charge provided no current crosses a lateral boundary. A nonzero boundary flux must be retained in the Stokes calculation rather than silently discarded.

For a genuinely [topological current](../../../../../topological-current.md), closure can follow identically from the field geometry, without the equations of motion. If a field $\phi:M\to N$ pulls back a [closed differential form](../../../../../closed-differential-form.md) $\kappa$ on its target, then

$$
d(\phi^*\kappa)=\phi^*(d\kappa)=0.
$$

For example, for a unit three-component field $\mathbf n:M\to S^2$, the normalized area form is

$$
\kappa=\frac{1}{8\pi}\epsilon_{abc}n^a\,dn^b\wedge dn^c,\qquad \int_{S^2}\kappa=1.
$$

On a closed oriented spatial two-surface $\Sigma$, $Q=\int_\Sigma\mathbf n^*\kappa$ is the integer [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md). Smooth evolution is a [homotopy](../../../../../homotopy.md) and conserves this [topological charge](../../../../../topological-charge.md). Singularities or flux through a spatial boundary can permit the charge to change. This is the [pullback-volume representation of a topological current](../../../../../pullback-volume-representation-of-a-topological-current.md).

A related example is the magnetic flux $\int_C F/(2\pi)$ of a $U(1)$ [principal connection](../../../../../connection-principal-bundle.md), representing a [First Chern class](../../../../../first-chern-class.md) when its normalization is integral. Nonzero flux on a closed cycle requires nontrivial global bundle data or singular sources: if a single smooth global potential exists with $F=dA$, the flux on every closed cycle vanishes. This distinction is important when local differential equations are used to infer global conservation or quantization.

A [brane](../../../../../brane.md) with $p$ spatial dimensions sweeps out an oriented $(p+1)$-dimensional [worldvolume](../../../../../worldvolume.md) $W$, embedded by $X:W\to M$. Its electric coupling to a $(p+1)$-form [gauge potential](../../../../../gauge-field.md) $C$ is the [Wess-Zumino brane coupling](../../../../../wess-zumino-brane-coupling.md)

$$
S_{\mathrm{int}}=q\int_WX^*C
=\frac{q}{(p+1)!}\int d^{p+1}\xi\,\epsilon^{a_0\cdots a_p}
C_{\mu_0\cdots\mu_p}(X)\,\partial_{a_0}X^{\mu_0}\cdots\partial_{a_p}X^{\mu_p}.
$$

It is invariant under orientation-preserving changes of worldvolume coordinates. Its field strength is $H=dC$, unchanged by the [gauge transformation](../../../../../gauge-transformation.md) $C\mapsto C+d\Lambda$ for a $p$-form $\Lambda$. Since the [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) commutes with the [exterior derivative](../../../../../exterior-derivative.md), its gauge variation is

$$
\delta S_{\mathrm{int}}=q\int_Wd(X^*\Lambda)=q\int_{\partial W}X^*\Lambda.
$$

Therefore **a closed brane has a gauge-invariant coupling** under these transformations. For a noncompact worldvolume, support or decay conditions must also eliminate contributions at infinity.

For an open [brane](../../../../../brane.md), the variation does not vanish automatically. If its boundary lies on a manifold carrying a $p$-form $B$, the [gauge invariance of an open-brane coupling](../../../../../gauge-invariance-of-an-open-brane-coupling.md) follows by adding $q\int_{\partial W}X^*B$ and assigning $B\mapsto B-\Lambda$. The two boundary variations cancel exactly with the induced orientation. Alternatively one may restrict the gauge parameter to have vanishing pullback at the boundary, if that is the chosen physical boundary condition. A particle has $p=0$ and couples by $q\int A$; a string has $p=1$ and couples to a two-form; a membrane has $p=2$ and couples to a three-form.

Finally, a gauge potential need not be globally a single differential form. Patchwise potentials and their overlap data define its global holonomy. For a large [gauge transformation](../../../../../gauge-transformation.md) $C\mapsto C+\chi$ with $\chi$ closed but not necessarily exact, quantum gauge invariance requires

$$
\boxed{q\int_WX^*\chi\in2\pi\mathbb Z\quad\text{so that }e^{iS_{\mathrm{int}}}\text{ is unchanged},}
$$

in units $\hbar=1$. This connects the coupling to integral periods and [charge quantization](../../../../../charge-quantization.md). The local Stokes argument and these global period conditions are complementary: closure controls continuous conservation, while global topology controls which charges and gauge transformations are allowed.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
