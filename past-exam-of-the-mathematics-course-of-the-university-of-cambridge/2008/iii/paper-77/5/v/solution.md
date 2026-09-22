<h1 id="5/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let the three grid-edge vectors be $v_1=a$, $v_2=b$, $v_3=b-a$, and define the constant-coefficient differential operator $D=\sum_{r=1}^3(v_r\cdot\nabla)^2$. For a stencil at grid spacing $h$, its displacement vectors $\delta$ about the new vertex have vanishing first and third moments by central symmetry. All four stencil types have the same second moment

$$
\sum_{\delta}\omega_\delta\,\delta\delta^T=\frac{h^2}{8}\sum_{r=1}^3v_rv_r^T.
$$

For the old-vertex stencil, each pair $\pm hv_r$ contributes $h^2v_rv_r^T/8$. For an edge parallel to $a$, the endpoint displacements are $\pm ha/2$ with weights $3/8$, and the opposite displacements are $\pm h(b-a/2)$ with weights $1/8$. Their moment is $h^2[aa^T/4+bb^T/4-(ab^T+ba^T)/8]$, precisely the same expression; the other edge orientations follow by symmetry.

If $f$ is a [multivariate polynomial](../../../../../../multivariate-polynomial.md) of total degree at most three, its [Taylor expansion](../../../../../../taylor-expansion.md) is exact through the third-order term. Thus every refined vertex samples the single polynomial

$$
T_h f=f+\frac{h^2}{16}Df.
$$

The [polynomial](../../../../../../polynomial-split.md) $Df$ has degree at most one, so subsequent refinement reproduces it exactly. Starting at unit spacing and successively halving $h$, the limit therefore is

$$
\boxed{f_\infty=f+\frac1{16}\sum_{\ell=0}^\infty4^{-\ell}Df=f+\frac1{12}Df.}
$$

The correction lowers degree by two, leaving the leading homogeneous term unchanged. Hence every sampled polynomial of degree at most three generates a polynomial of that same degree, even though quadratics and cubics need not be reproduced identically. For the extruded cases this gives $y^2\mapsto y^2+1/3$ and $y^3\mapsto y^3+y$.

Degree four is not guaranteed. Extruded data $g_j=j^4$ reduce to the [Cardinal cubic B-spline](../../../../../../cardinal-cubic-b-spline.md) $G(y)=\sum_jj^4M_3(y-j)$, which is piecewise cubic and hence cannot be a single polynomial of degree four. It is not a lower-degree polynomial either: at integer rows, $G(k)=[(k-1)^4+4k^4+(k+1)^4]/6=k^4+2k^2+1/3$, which cannot agree with a cubic at all integers. This counterexample excludes every guaranteed degree $d\ge4$. Consequently

$$
\boxed{d_{\rm same\ degree}=3.}
$$

This distinguishes polynomial generation from exact reproduction and again refers to all polynomials through the stated degree.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [5](../../5.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
