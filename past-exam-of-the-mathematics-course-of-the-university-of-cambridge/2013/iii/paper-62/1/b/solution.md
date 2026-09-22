<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) and [biconjugate](../../../../../../biconjugate.md) are

$$
f^*(p)=\sup_x\{\langle p,x\rangle-f(x)\},\qquad
f^{**}(x)=\sup_p\{\langle p,x\rangle-f^*(p)\}.
$$

The [Fenchel-Moreau theorem](../../../../../../fenchel-moreau-theorem.md) says that every [proper convex function](../../../../../../proper-convex-function.md) which is [lower semicontinuous](../../../../../../lower-semicontinuity.md) equals its [biconjugate](../../../../../../biconjugate.md). More generally, if a proper extended-real $f$ has an [affine minorant](../../../../../../affine-minorant.md), then

$$
\boxed{f^{**}=\operatorname{cl\,conv}f,}
$$

where the right side is the greatest [lower semicontinuous](../../../../../../lower-semicontinuity.md) [convex](../../../../../../convex-function.md) minorant. This is [biconjugation as closed convexification](../../../../../../biconjugation-as-closed-convexification.md). The affine-minorant hypothesis ensures that the closed convexification is proper; an unqualified statement including arbitrary improper functions would need separate conventions.

Here are the essential proof steps. The [Fenchel–Young inequality](../../../../../../fenchel-young-inequality.md) gives $f^{**}\leq f$. Every term in the supremum defining $f^{**}$ is an [affine minorant](../../../../../../affine-minorant.md) of $f$, and conversely any affine minorant $\langle p,x\rangle+a\leq f(x)$ has $a\leq-f^*(p)$. Thus $f^{**}$ is exactly the supremum of all affine minorants, hence is convex and lower semicontinuous.

Put $g=\operatorname{cl\,conv}f$. Its [epigraph](../../../../../../epigraph.md) is the closed convex hull of the epigraph of $f$. Applying the [half-space representation of a closed convex set](../../../../../../half-space-representation-of-a-closed-convex-set.md) in $\mathbb R^{n+1}$ recovers that epigraph from its containing half-spaces. A containing half-space written

$$
\langle v,x\rangle+q t\leq a
$$

has $q\leq0$, since epigraphs extend upwards. If $q<0$, it is precisely the epigraph inequality of an affine minorant, $t\geq(\langle v,x\rangle-a)/(-q)$.

Vertical half-spaces with $q=0$ must also be accounted for. Choose one affine minorant $\ell_0$ of $g$, which exists because $g$ is proper and closed: strictly separate $(x_0,g(x_0)-1)$ from its epigraph for a finite domain point $x_0$; the separating coefficient of $t$ cannot be zero, since that would not distinguish points with the same $x_0$. If a vertical containing inequality is $\langle v,x\rangle\leq a$, then

$$
\ell_0(x)+L(\langle v,x\rangle-a),\qquad L\geq0,
$$

is still an affine minorant on the domain of $g$. At a point violating the vertical inequality, these minorants tend to infinity as $L\to\infty$. Thus vertical domain restrictions are also recovered by the supremum of affine minorants.

Consequently $g$ equals that supremum. Every affine minorant of $g$ is below $f$, while the epigraph of any affine minorant of $f$ contains its closed convex epigraph hull. Therefore $f$ and $g$ have the same affine minorants, completing $g=f^{**}$. **The theorem in the previous solution supplies the geometric separation step behind biconjugation.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
