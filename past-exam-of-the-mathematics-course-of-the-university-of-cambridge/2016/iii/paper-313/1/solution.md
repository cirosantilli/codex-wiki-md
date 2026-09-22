<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the orientation selected by the [volume form](../../../../../volume-form.md), and let $\operatorname{vol}_g$ be its normalized [Riemannian volume form](../../../../../riemannian-volume-form.md). The [Euclidean metric](../../../../../euclidean-metric.md) induces an [inner product](../../../../../inner-product.md) on the [exterior algebra](../../../../../exterior-algebra.md) of covectors. The [Hodge star operator](../../../../../hodge-star-operator.md) is the unique map from $p$-forms to $(4-p)$-forms satisfying

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g.
$$

For an oriented orthonormal coframe $e^1,\ldots,e^4$, it sends a basis wedge to the complementary wedge with the sign of the permutation that restores $e^1\wedge\cdots\wedge e^4$. Applying the [Hodge star operator](../../../../../hodge-star-operator.md) twice exchanges blocks of $p$ and $4-p$ covectors, so

$$
*^2=(-1)^{p(4-p)},\qquad\boxed{*^2=1\quad\text{on two-forms}.}
$$

Here the supplied volume is interpreted in the usual metric-normalized sense. If instead one defines the operator with an arbitrary unnormalized $\operatorname{vol}=f\operatorname{vol}_g$, that operator is $f*_g$ and its square on two-forms is $f^2$. The usual self-duality statements use the metric-normalized [Hodge star operator](../../../../../hodge-star-operator.md), with the supplied volume specifying orientation.

The projections $P_\pm=(1\pm*)/2$ give the [Hodge splitting of Euclidean two-forms](../../../../../hodge-splitting-of-euclidean-two-forms.md):

$$
\boxed{\Lambda^2=\Lambda^2_+\oplus\Lambda^2_-,\qquad
\alpha_\pm=\frac12(\alpha\pm*\alpha),\qquad *\alpha_\pm=\pm\alpha_\pm.}
$$

Both spaces have dimension three. With $e^4=dt$, bases are

$$
\Sigma_i^\pm=e^i\wedge dt\ \pm\ \frac12\epsilon_{ijk}e^j\wedge e^k,
\qquad i=1,2,3.
$$

The [Hodge star operator](../../../../../hodge-star-operator.md) is an orthogonal involution on two-forms and therefore is self-adjoint. For a [self-dual two-form](../../../../../self-dual-differential-form.md) $H$ and an [anti-self-dual two-form](../../../../../anti-self-dual-differential-form.md) $G$,

$$
\langle H,G\rangle=\langle *H,G\rangle
=\langle H,*G\rangle=-\langle H,G\rangle=0.
$$

Consequently

$$
\boxed{H\wedge G=\langle H,*G\rangle\operatorname{vol}_g=0.}
$$

This is the [wedge orthogonality of opposite-duality two-forms](../../../../../wedge-orthogonality-of-opposite-duality-two-forms.md).

For the [Yang-Mills action](../../../../../yang-mills-action.md), take an anti-Hermitian [special unitary group](../../../../../special-unitary-group.md) connection and the fundamental matrix [trace](../../../../../matrix-trace.md), so the positive invariant pairing on its [Lie algebra](../../../../../lie-algebra-split.md) is $\langle X,Y\rangle=-\operatorname{tr}(XY)$. Write its [gauge curvature](../../../../../gauge-field-strength.md) as $F=F_++F_-$ using the [Hodge splitting of Euclidean two-forms](../../../../../hodge-splitting-of-euclidean-two-forms.md), and define

$$
\|F_\pm\|^2=-\int\operatorname{tr}(F_\pm\wedge *F_\pm),\qquad
S_{\mathrm{YM}}=-\frac1{g_{\mathrm{YM}}^2}\int\operatorname{tr}(F\wedge*F).
$$

Cross terms vanish by the [wedge orthogonality of opposite-duality two-forms](../../../../../wedge-orthogonality-of-opposite-duality-two-forms.md). Thus

$$
S_{\mathrm{YM}}=\frac{\|F_+\|^2+\|F_-\|^2}{g_{\mathrm{YM}}^2},\qquad
\int\operatorname{tr}(F\wedge F)=-\|F_+\|^2+\|F_-\|^2.
$$

With this anti-Hermitian convention the [Second Chern number](../../../../../second-chern-number.md) is

$$
k=c_2(E)[S^4]=\frac1{8\pi^2}\int\operatorname{tr}(F\wedge F).
$$

For example, this normalization follows by expanding $\det(1+iF/(2\pi))$ and using $\operatorname{tr}F=0$. Interpreting the integral as an integer [Second Chern number](../../../../../second-chern-number.md) on $\mathbb R^4$ assumes the usual decay and gauge behavior that allow extension over the point at infinity. The following norm inequality itself does not require integrality:

$$
\boxed{S_{\mathrm{YM}}\ge\frac{8\pi^2}{g_{\mathrm{YM}}^2}|k|.}
$$

The [Yang-Mills instanton Bogomolny bound](../../../../../yang-mills-instanton-bogomolny-bound.md) is saturated precisely when one component vanishes: $F=*F$ or $F=-*F$. In the stated convention the self-dual case has $k\le0$ and the anti-self-dual case has $k\ge0$. Reversing orientation, or defining topological charge with the opposite sign, reverses this assignment while leaving the absolute-value bound unchanged.

For the [self-dual Yang-Mills equations in temporal gauge](../../../../../self-dual-yang-mills-equations-in-temporal-gauge.md), choose $\operatorname{vol}_g=dx^1\wedge dx^2\wedge dx^3\wedge dt$ and $\epsilon_{123}=1$. The relevant [Hodge star operator](../../../../../hodge-star-operator.md) identities are

$$
*(dt\wedge dx^i)=-\frac12\epsilon_{ijk}dx^j\wedge dx^k,
\qquad *(dx^j\wedge dx^k)=-\epsilon_{ijk}dt\wedge dx^i.
$$

Writing $F=F_{ti}\,dt\wedge dx^i+\tfrac12F_{jk}\,dx^j\wedge dx^k$, the [self-dual Yang-Mills equations](../../../../../self-dual-yang-mills-equations.md) $F=*F$ give

$$
F_{ti}=-\frac12\epsilon_{ijk}F_{jk}.
$$

In [temporal gauge](../../../../../temporal-gauge.md), $A_t=0$, so the [gauge curvature](../../../../../gauge-field-strength.md) component is $F_{ti}=\partial_tA_i-\partial_iA_t+[A_t,A_i]=\partial_tA_i$. Hence

$$
\boxed{\partial_tA_i=-\frac12\epsilon_{ijk}F_{jk},\qquad
F_{jk}=\partial_jA_k-\partial_kA_j+[A_j,A_k].}
$$

The minus sign follows from placing $dt$ last in the orientation and first in the mixed curvature component.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
