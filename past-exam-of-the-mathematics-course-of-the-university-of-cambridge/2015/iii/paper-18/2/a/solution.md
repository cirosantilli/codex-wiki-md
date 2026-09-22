<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use complex-valued smooth [differential forms](../../../../../../differential-form-split.md). The [sheaf of smooth differential forms](../../../../../../sheaf-of-smooth-differential-forms.md) is $\mathcal A^k(U)=\Gamma(U,\bigwedge^k(T^*X\otimes\mathbb C))$, with the usual restriction maps. Dualizing the [type decomposition of the complexified tangent bundle](../../../../../../type-decomposition-of-the-complexified-tangent-bundle.md) and taking [exterior powers](../../../../../../exterior-power.md) decomposes this bundle into the summands

$$
\bigwedge^p(T^{1,0}X)^*\otimes\bigwedge^q(T^{0,1}X)^*,\qquad p+q=k.
$$

Their smooth sections form the [sheaf of differential forms of type (p, q)](../../../../../../sheaf-of-differential-forms-of-type-p-q.md) $\mathcal A^{p,q}$. Locally a section is a sum of $f_{I,J}\,dz_I\wedge d\bar z_J$ with $|I|=p$, $|J|=q$ and smooth coefficients. Holomorphic transition maps preserve types, so the local decompositions agree globally. Hence

$$
\boxed{\mathcal A^k(X)=\bigoplus_{p+q=k}\mathcal A^{p,q}(X).}
$$

The [exterior derivative](../../../../../../exterior-derivative.md) splits as $d=\partial+\bar\partial$, with bidegrees $(1,0)$ and $(0,1)$. Its square being zero gives $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$. The [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md) is therefore

$$
\boxed{H^{p,q}_{\bar\partial}(X)=
\frac{\ker(\bar\partial:\mathcal A^{p,q}(X)\to\mathcal A^{p,q+1}(X))}
{\bar\partial\mathcal A^{p,q-1}(X)}.}
$$

Forms in negative or out-of-range bidegrees are understood to be zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
