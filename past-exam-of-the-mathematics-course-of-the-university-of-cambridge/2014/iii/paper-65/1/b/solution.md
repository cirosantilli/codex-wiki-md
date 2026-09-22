<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an extended-real function define its [Fenchel conjugate](../../../../../../convex-conjugate.md) by $f^*(p)=\sup_x(\langle p,x\rangle-f(x))$ and its [biconjugate](../../../../../../biconjugate.md) by $f^{**}(x)=\sup_p(\langle p,x\rangle-f^*(p))$. The [Fenchel-Moreau theorem](../../../../../../fenchel-moreau-theorem.md) states, in the standard proper-envelope setting,

$$
\boxed{f^{**}=\operatorname{cl}\operatorname{conv}f.}
$$

Here the right side is the largest [lower semicontinuous](../../../../../../lower-semicontinuity.md) [convex function](../../../../../../convex-function.md) below $f$, equivalently the function whose [epigraph](../../../../../../epigraph.md) is the closed convex hull of $\operatorname{epi}f$. It is enough to assume $f$ is proper and has an [affine minorant](../../../../../../affine-minorant.md), ensuring this envelope is proper. In particular, for a [proper convex function](../../../../../../proper-convex-function.md) that is [lower semicontinuous](../../../../../../lower-semicontinuity.md), $\boxed{f^{**}=f}$.

First, $\langle p,x\rangle-f^*(p)\leq f(x)$ by the definition of the [convex conjugate](../../../../../../convex-conjugate.md). The [biconjugate](../../../../../../biconjugate.md) is a supremum of continuous affine functions, so it is convex, lower semicontinuous and no greater than $f$. Second, the best intercept for an [affine minorant](../../../../../../affine-minorant.md) with slope $p$ is $-f^*(p)$: $\langle p,x\rangle+a\leq f(x)$ for all $x$ precisely when $a\leq-f^*(p)$. Thus $f^{**}$ is the supremum of all affine minorants.

To prove that no part of the closed convex envelope is missed, set $E=\operatorname{cl}\operatorname{conv}(\operatorname{epi}f)$. The [half-space representation of a closed convex set](../../../../../../half-space-representation-of-a-closed-convex-set.md) from part (a), applied in $\mathbb R^{n+1}$, separates any $(x_0,t_0)\notin E$ from $E$ by an inequality $a\cdot x+bt\leq d$. Because $E$ is upward closed, $b\leq0$. If $b<0$, division by $-b$ gives an [affine minorant](../../../../../../affine-minorant.md) $\ell$ with $\ell(x_0)>t_0$.

A vertical separator has $b=0$. Let $\ell_0$ be an existing [affine minorant](../../../../../../affine-minorant.md). Combine $a\cdot x\leq d$ with $\ell_0(x)\leq t$ to obtain

$$
\ell_0(x)+\frac{a\cdot x-d}{\varepsilon}\leq t\qquad\text{on }E.
$$

Since $a\cdot x_0-d>0$, a sufficiently small positive $\varepsilon$ makes this affine function exceed $t_0$. Thus vertical half-spaces can be approximated by nonvertical epigraph supports. Every point below the envelope is excluded by an [affine minorant](../../../../../../affine-minorant.md), so the supremum of these minorants is exactly the envelope. This is the decisive use of part (a).

Properness and the minorant convention matter for unrestricted extended-real functions. For example, $f(x)=-x^2$ on $\mathbb R$ has no [affine minorant](../../../../../../affine-minorant.md); $f^*\equiv+\infty$ and $f^{**}\equiv-\infty$. With the corresponding improper-envelope convention its closed convex envelope is also $-\infty$. The theorem should not silently describe such an envelope as proper. The identically $+\infty$ function is another degenerate case, handled separately by extended-real conventions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
