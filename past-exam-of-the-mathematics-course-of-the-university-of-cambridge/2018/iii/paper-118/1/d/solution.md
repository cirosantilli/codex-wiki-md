<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The natural map between [Bott-Chern cohomology](../../../../../../bott-chern-cohomology.md) and [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md) is

$$
\phi:[\alpha]_{BC}\longmapsto[\alpha]_{\bar\partial}.
$$

It is well-defined: a $d$-closed pure-type form is $\bar\partial$-closed, and $\partial\bar\partial\beta=-\bar\partial(\partial\beta)$ is $\bar\partial$-exact.

For surjectivity, choose the unique [harmonic differential form](../../../../../../harmonic-differential-form.md) $h$ representing a [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md) class using [Dolbeault Hodge decomposition](../../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md). The [Kähler Laplacian identity](../../../../../../kahler-laplacian-identity.md) $\Delta_d=2\Delta_{\bar\partial}$ makes $h$ a [harmonic differential form](../../../../../../harmonic-differential-form.md) for $d$, hence $d$-closed. Sending the Dolbeault class to $[h]_{BC}$ consequently gives a right inverse.

For injectivity, the [ddbar lemma](../../../../../../ddbar-lemma.md) says directly that a $d$-closed, $\bar\partial$-exact pure-type form is $\partial\bar\partial$-exact. One can also exhibit its primitive. Let $G_d$ be the [Green operator of the Hodge Laplacian](../../../../../../green-operator-of-the-hodge-laplacian.md), and put $G_{\bar\partial}=2G_d$. If $\alpha$ is $d$-closed and $\bar\partial$-exact, its harmonic projection vanishes and the [Kähler identities](../../../../../../kahler-identities.md) give

$$
\alpha=\bar\partial\bar\partial^*G_{\bar\partial}\alpha
=-i\partial\bar\partial\Lambda G_{\bar\partial}\alpha.
$$

Here $\partial G_{\bar\partial}\alpha=\bar\partial G_{\bar\partial}\alpha=0$ because the Green operator commutes with these differentials, and $\bar\partial^*=-i[\Lambda,\partial]$. Thus $\alpha$ represents zero in [Bott-Chern cohomology](../../../../../../bott-chern-cohomology.md). We have constructed the canonical isomorphism and its harmonic inverse:

$$
\boxed{\phi:H_{BC}^{p,q}(M)\xrightarrow{\sim}H_{\bar\partial}^{p,q}(M),\qquad
\phi^{-1}([\alpha]_{\bar\partial})=[h]_{BC}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
