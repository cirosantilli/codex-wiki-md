<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For nonzero finite-dimensional $U$ and $V$, **the intended assertion is true**. Write $a=\dim U$, $b=\dim V$, and replace $W$ by $\operatorname{im}\phi$, of dimension $r$. Injectivity on the stated slices implies $\phi(u\otimes v)\ne0$ whenever $u,v\ne0$. Consequently the [bilinear map](../../../../../../bilinear-map.md) defines a continuous map of [Complex projective spaces](../../../../../../complex-projective-space.md)

$$
F:\mathbb P(U)\times\mathbb P(V)\longrightarrow\mathbb P(\operatorname{im}\phi),\qquad ([u],[v])\longmapsto[\phi(u\otimes v)].
$$

The rank $r$ is at least one, since one such nonzero tensor has nonzero image.

Let $L_U,L_V,L_W$ be the respective [tautological bundles](../../../../../../tautological-bundle.md). Fiberwise, $\phi$ identifies $L_U\otimes L_V$ with $F^*L_W$. For the positive hyperplane classes $x=c_1(L_U^*)$, $y=c_1(L_V^*)$ and $z=c_1(L_W^*)$ (zero when the projective space is a point), the [first Chern class of a tensor product of complex line bundles](../../../../../../first-chern-class-of-a-tensor-product-of-complex-line-bundles.md) gives

$$
F^*z=x+y.
$$

The [Künneth theorem](../../../../../../kunneth-theorem.md), together with part (a), identifies the product [cohomology ring](../../../../../../cohomology-ring.md) with

$$
H^*(\mathbb P(U)\times\mathbb P(V);\mathbb Z)=\mathbb Z[x,y]/(x^a,y^b).
$$

There are no Tor terms because the factor groups are free. In particular, its monomials $x^iy^j$ with $0\leq i<a$, $0\leq j<b$ form an integral additive basis. In top degree,

$$
(x+y)^{a+b-2}=\binom{a+b-2}{a-1}x^{a-1}y^{b-1}\ne0.
$$

If $r\leq a+b-2$, the target relation $z^r=0$ would imply $(x+y)^r=0$ and hence contradict this nonzero top power. Thus

$$
\boxed{\dim_{\mathbb C}\operatorname{im}\phi\geq\dim_{\mathbb C}U+\dim_{\mathbb C}V-1.}
$$

When $a=b=1$, the already-established inequality $r\geq1$ gives the same conclusion. The [complex bilinear dimension bound](../../../../../../complex-bilinear-dimension-bound.md) is sharp: multiplication of complex polynomials of degrees less than $a$ and $b$ has target dimension $a+b-1$, is injective in either nonzero fixed factor, and its image spans every monomial in that target.

**Literal zero-space qualification.** The printed assertion does not explicitly exclude zero vector spaces. If $U=0$, $V=\mathbb C^2$ and $W=0$, its slice-injectivity hypothesis is vacuous, while the claimed inequality would be $0\geq1$. Thus, with zero spaces permitted, this is a counterexample to the assertion exactly as written; the proof above supplies the usual nonzero finite-dimensional interpretation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
