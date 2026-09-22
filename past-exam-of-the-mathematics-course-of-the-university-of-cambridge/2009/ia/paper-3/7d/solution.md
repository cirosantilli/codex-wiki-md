<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Use the existing [cross-ratio](../../../../../cross-ratio.md) convention

$$
[a_0,a_1,a_2,z]=\frac{(z-a_1)(a_0-a_2)}{(z-a_2)(a_0-a_1)}.
$$

Values involving infinity are defined by limits. More uniformly, represent each point by a nonzero homogeneous vector $u=(u_0,u_1)$ and put $D(u,v)=u_0v_1-u_1v_0$. Then the same value is $D(z,a_1)D(a_0,a_2)/[D(z,a_2)D(a_0,a_1)]$, interpreted in the [Riemann sphere](../../../../../riemann-sphere.md). Rescaling any representative cancels out. The first three points are distinct, so numerator and denominator cannot simultaneously vanish. The fourth point may coincide with one of them, giving the values $1,0,\infty$ at $a_0,a_1,a_2$, respectively.

With $a_0,a_1,a_2$ fixed, this is a nonconstant [Möbius transformation](../../../../../mobius-transformation.md) $f$. For finite first three points, write $C=(a_0-a_2)/(a_0-a_1)\ne0$; then

$$
f(z)=C\frac{z-a_1}{z-a_2},\qquad
\boxed{f^{-1}(w)=\frac{wa_2-Ca_1}{w-C}.}
$$

The [determinant](../../../../../determinant.md) of this fractional-linear map is nonzero because $a_1\ne a_2$. Its inverse is defined at every point of the sphere, including poles and infinity, so each $w$ has exactly one preimage. The same conclusion follows directly from the homogeneous formula when an $a_i$ is infinity.

[Möbius transformations](../../../../../mobius-transformation.md) preserve [generalized circles](../../../../../generalized-circle-under-a-mobius-transformation.md). To verify the fact used here, affine complex changes preserve ordinary circles and lines, while a generalized circle has an equation $A|z|^2+Bz+\overline B\overline z+D=0$ with $A,D$ real. Substitution $z=1/w$ and multiplication by $|w|^2$ gives another equation of the same form. Every non-affine Möbius map is a composition of affine maps and $z\mapsto1/z$, so the claim follows. Consequently

$$
S=f^{-1}(\mathbb R\cup\{\infty\})
$$

is a generalized circle. It contains the three distinct $a_i$, so it is their unique ordinary circle, or their line together with infinity when they are collinear. This is the [real cross-ratio criterion for a generalized circle](../../../../../real-cross-ratio-criterion-for-a-generalized-circle.md).

Let $c(w)=\overline w$, with $c(\infty)=\infty$. The defining equation for $J$ now gives the [cross-ratio construction of generalized-circle reflection](../../../../../cross-ratio-construction-of-generalized-circle-reflection.md):

$$
\boxed{J=f^{-1}\circ c\circ f.}
$$

This is well-defined by bijectivity of $f$, and $J^2=f^{-1}c^2f$ is the identity. Moreover $J(z)=z$ precisely for $z\in S$.

If the first three points lie on the extended real line, the normalization map has real coefficients, so $f(\overline z)=\overline{f(z)}$. Hence $J(z)=\overline z$. For a second triple $b_0,b_1,b_2$ on the same generalized circle, write its normalization as $g=Mf$. Each $f(b_i)$ is real or infinity, and the unique Möbius map taking this real triple to $1,0,\infty$ has real coefficients. Thus $M$ commutes with $c$, giving

$$
g^{-1}cg=f^{-1}M^{-1}cMf=f^{-1}cf.
$$

Therefore **$J$ depends only on the generalized circle, not on the three selected points**. For an ordinary circle with centre $q$ and radius $R$, it is [inversion in a circle](../../../../../inversion-in-a-circle.md), $J(z)=q+R^2/(\overline z-\overline q)$; for a straight line it is the corresponding Euclidean reflection, extended to infinity.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
