<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $D=\mathbb H\setminus K$. By definition of a [compact H-hull](../../../../../../compact-h-hull.md), $D$ is a proper [simply connected domain](../../../../../../simply-connected-domain.md), and it agrees with the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) outside a sufficiently large disc. The [Riemann mapping theorem](../../../../../../riemann-mapping-theorem.md) supplies a [conformal isomorphism](../../../../../../biholomorphism.md) $f:D\to\mathbb H$. Choose its boundary normalization so that the [prime end](../../../../../../prime-end.md) at infinity maps to infinity. This [prime end](../../../../../../prime-end.md) is unambiguous because the domain has an ordinary straight real boundary near infinity.

The [Schwarz reflection principle](../../../../../../schwarz-reflection-principle.md), applied there in the coordinate $1/z$, extends $f$ across the real boundary near infinity. It has a simple pole there, with [Laurent series](../../../../../../laurent-series.md)

$$
f(z)=az+b+\frac{c}{z}+O(z^{-2}),\qquad a>0,\quad b,c\in\mathbb R.
$$

The pole is simple because the reflected map is locally conformal at infinity; its leading coefficient is positive because it maps the upper side to the upper side. Postcomposing with the half-plane automorphism $w\mapsto(w-b)/a$ gives

$$
g_K(z)=z+O(1/z),\qquad\boxed{g_K(z)-z\longrightarrow0.}
$$

This is [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md).

If $g_1,g_2$ both satisfy it, $g_2\circ g_1^{-1}$ is a [conformal automorphism of the upper half-plane](../../../../../../conformal-automorphism-of-the-upper-half-plane.md). The asymptotics force it to fix infinity, so it has the form $w\mapsto\alpha w+\beta$ with $\alpha>0$ and $\beta\in\mathbb R$. The same asymptotics force $\alpha=1$, $\beta=0$. Hence **the normalized [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) exists and is unique**. The argument requires reflection only outside a large disc, not regularity of the hull's entire boundary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
