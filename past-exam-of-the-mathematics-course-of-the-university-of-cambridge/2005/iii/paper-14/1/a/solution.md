<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mathcal D=\mathcal K_X^*/\mathcal O_X^*$, the quotient [sheaf of abelian groups](../../../../../../sheaf-of-abelian-groups.md). At a closed point $P$, the [discrete valuation](../../../../../../discrete-valuation.md) gives an [isomorphism](../../../../../../isomorphism.md)

$$
\mathcal D_P=k(X)^*/\mathcal O_{X,P}^*
\xrightarrow{\;\sim\;}\mathbb Z,\qquad [f]\longmapsto v_P(f).
$$

Indeed, a [local parameter on a smooth algebraic curve](../../../../../../local-parameter-on-a-smooth-algebraic-curve.md) has valuation one, and the valuation kernel is precisely the [unit group](../../../../../../unit-group.md) of the [discrete valuation ring](../../../../../../discrete-valuation-ring.md). Thus a local section represented by $f$ determines its local [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md), and changing $f$ by a [regular function](../../../../../../regular-function.md) which is a unit does not change those coefficients.

These local valuations identify $\Gamma(X,\mathcal D)$ with $\operatorname{Div}(X)$. To see that they give finite support, represent a section locally by finitely many [rational functions on an algebraic variety](../../../../../../rational-function-on-an-algebraic-variety.md), using [Noetherian Zariski topology](../../../../../../noetherian-zariski-topology.md) to take a finite cover. Each representative has only finitely many zeros and poles, so their combined support is finite. Conversely, for $D=\sum n_PP$, choose at each support point a [local parameter](../../../../../../local-parameter-on-a-smooth-algebraic-curve.md) $t_P$ and shrink its neighbourhood to exclude every other zero or pole of $t_P$ and every other support point. The local rational equation $t_P^{n_P}$ represents the desired valuations there; on the complement of the support use $1$. On overlaps these equations differ by units, so their classes glue in the quotient [sheaf](../../../../../../sheaf-mathematics.md). Finally, a section with every valuation zero has zero germ everywhere and is the identity section. Hence the identification is both [surjective](../../../../../../surjective-function.md) and [injective](../../../../../../injective-function.md).

The map on [global sections](../../../../../../global-section.md) sends $f\in k(X)^*$ to $\operatorname{div}(f)$. Therefore its [cokernel](../../../../../../cokernel.md) is

$$
\boxed{\operatorname{coker}\bigl(H^0(X,\mathcal K_X^*)\to
H^0(X,\mathcal K_X^*/\mathcal O_X^*)\bigr)
=\operatorname{Div}(X)/\operatorname{Prin}(X)
\cong\operatorname{Cl}(X).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
