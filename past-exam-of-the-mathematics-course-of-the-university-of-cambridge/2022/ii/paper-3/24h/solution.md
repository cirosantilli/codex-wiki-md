<h1 id="24h/solution">Solution</h1>

↑ **Parent:** [24H](../24h.md)

Let $X$ be an irreducible variety of dimension $d$. A point $p\in X$ is nonsingular, or smooth, when

$$
\dim T_pX=d,
$$

where $T_pX$ is the [Zariski tangent space](../../../../../zariski-tangent-space.md); it is a [singular point](../../../../../singular-point-of-an-algebraic-variety.md) when $\dim T_pX>d$. Equivalently, the local ring $\mathcal O_{X,p}$ is regular exactly at a nonsingular point.

For an irreducible affine variety $X\subseteq\mathbb A^N$ over a perfect field, the [Jacobian criterion](../../../../../jacobian-criterion.md) expresses the singular locus by the vanishing of the relevant Jacobian minors, so it is [Zariski closed](../../../../../zariski-closed-set.md). At a point where the tangent-space dimension is minimal it equals $d$; equivalently, some $(N-d)$-rowed Jacobian minor is nonzero. Its nonvanishing locus is therefore a nonempty [Zariski-open set](../../../../../zariski-open-set.md) contained in the smooth locus. Every nonempty open subset of an [irreducible topological space](../../../../../irreducible-topological-space.md) is dense, proving the [density of the smooth locus](../../../../../density-of-the-smooth-locus.md).

Assume the ground field has characteristic other than two. For

$$
Q=V(X_0^2+\cdots+X_{n-1}^2)\subseteq\mathbb P^n,
$$

the partial derivatives are $2X_0,\ldots,2X_{n-1},0$. They vanish simultaneously at the unique projective point

$$
\boxed{[0:\cdots:0:1]}.
$$

Thus this point is the singular locus of the projective quadric cone.

For varieties $X,Y$,

$$
T_{(x,y)}(X\times Y)\cong T_xX\oplus T_yY,
\qquad
\dim(X\times Y)=\dim X+\dim Y.
$$

If $Y$ is smooth of dimension $m$, the product point $(x,y)$ is singular exactly when $x$ is singular. Hence

$$
\operatorname{Sing}(X\times Y)=Z\times Y
$$

and

$$
\boxed{\dim\operatorname{Sing}(X\times Y)=k+m}.
$$

This is the [singular locus of a product with a smooth variety](../../../../../singular-locus-of-a-product-with-a-smooth-variety.md).

To construct the requested examples, put $r=n-k>0$. If $r\geq2$, let $Q_r\subseteq\mathbb P^{r+1}$ be an irreducible quadric cone of dimension $r$ with one singular vertex. If $r=1$, use instead the irreducible cuspidal cubic

$$
C=V(Y^2Z-X^3)\subseteq\mathbb P^2,
$$

whose only singular point is $[0:0:1]$. Let $W$ denote the chosen $r$-dimensional variety and embed

$$
W\times\mathbb P^k
$$

in projective space by the [Segre embedding](../../../../../segre-embedding.md). It is irreducible and has dimension $r+k=n$, while its singular locus is the vertex or cusp point times $\mathbb P^k$, which is nonempty and has dimension exactly $k$. This is the [projective variety with a prescribed-dimensional singular locus](../../../../../projective-variety-with-a-prescribed-dimensional-singular-locus.md) construction.

Finally, suppose that the irreducible plane curve $C\subseteq\mathbb P^2$ were smooth of degree $d$. Since it is birational to a smooth projective curve of genus two, its [geometric genus](../../../../../geometric-genus.md) would be two. But the [genus of a smooth plane curve](../../../../../genus-of-a-smooth-plane-curve.md) is

$$
g(C)=\frac{(d-1)(d-2)}2,
$$

and no integer $d$ makes this number equal to two. Therefore $C$ cannot be smooth and must contain a singular point.

## ↑ Ancestors (10)

1. [24H](../24h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
