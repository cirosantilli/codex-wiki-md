<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a polygonal domain with finite real prevertices $a_j$ and interior angles $\pi\alpha_j$, the [Schwarz-Christoffel formula](../../../../../schwarz-christoffel-mapping.md) has the form

$$
F(z)=C_0+C_1\int^z\prod_j(\zeta-a_j)^{\alpha_j-1}\,d\zeta,
\qquad C_1\neq0,
$$

with branches chosen in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). A prevertex at infinity is interpreted by the corresponding limiting version of the formula. The exponent records the angle because locally $F-F(a_j)$ behaves as $(z-a_j)^{\alpha_j}$.

For a slit from $0$ to $\tau$ in the upper half-plane, put $\vartheta=\arg\tau\in(0,\pi)$. The two approaches to its base are separate boundary vertices with angles $\pi-\vartheta$ and $\vartheta$, and the tip has angle $2\pi$. With ordered prevertices $a<c<b$ mapping respectively to the base, tip and base, the [Schwarz-Christoffel mapping](../../../../../schwarz-christoffel-mapping.md) therefore has

$$
F'(z)=C(z-a)^{-\vartheta/\pi}(z-c)(z-b)^{\vartheta/\pi-1}.
$$

The tip's factor is a simple zero of the boundary derivative, not an interior critical point.

For the specified power product, the principal branches give

$$
\arg g(z)=k\arg(z-1)+(1-k)\arg(z+1)\in(0,\pi)
$$

throughout the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), so $g$ maps into that half-plane. Logarithmic differentiation gives

$$
\boxed{g'(z)=(z-c)(z-1)^{k-1}(z+1)^{-k},\qquad c=1-2k.}
$$

There are no zeros of this [derivative](../../../../../derivative.md) in the upper half-plane, so the map is locally [conformal](../../../../../conformal-map.md) there. Its boundary values are negative real for $x<-1$, positive real for $x>1$, and

$$
g(x)=e^{i\pi k}(1-x)^k(1+x)^{1-k}\qquad(-1<x<1).
$$

The positive scalar factor increases from zero to its maximum at $c$ and then decreases to zero, since its logarithmic derivative is $-k/(1-x)+(1-k)/(1+x)$. Therefore the tip is

$$
\boxed{\tau=g(c)=2k^k(1-k)^{1-k}e^{i\pi k}.}
$$

The real boundary runs from the negative real axis to zero, out to $\tau$, back to zero, and then along the positive real axis.

For completeness, these boundary facts give global injectivity and surjectivity. At infinity,

$$
g(z)=z+1-2k+O(1/z).
$$

Apply the [argument principle](../../../../../argument-principle.md) on a large upper half-disc, indenting the real prevertices by small semicircles. For a fixed $w$ in the upper half-plane off $[0,\tau]$, the limiting image contour is the real boundary with the slit traversed once in each direction, followed by a large upper semicircle. Its [winding number](../../../../../winding-number.md) about $w$ is one. The two slit traversals cancel, so $g(z)-w$ has exactly one zero in the upper half-plane. There are no poles.

Nor can an interior point map onto the open slit. Each point of that slit has two real preimages, one on either side of $c$, with nonzero boundary derivatives. Local continuation across the real line maps the upper half-neighborhoods at these preimages onto the two different sides of the slit. An additional interior preimage would persist for nearby off-slit points and contradict the already proved one-preimage count. The tip cannot be an interior image either: the [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md) would then place nearby open-slit points in the interior image. Finally, $g$ never vanishes inside the half-plane. Thus **$g$ is a conformal bijection onto $S(\tau)$**.

This is the [power-product map to a slit half-plane](../../../../../power-product-map-to-a-slit-half-plane.md). Its derivative is exactly the [Schwarz-Christoffel formula](../../../../../schwarz-christoffel-mapping.md) with $a=-1$, $b=1$, $c=1-2k$, $\vartheta=\pi k$ and $C=1$. The additive constant is fixed by the boundary value $g(1)=0$. Thus the power-product expression is an explicit antiderivative of the corresponding [Schwarz-Christoffel mapping](../../../../../schwarz-christoffel-mapping.md), with this normalization.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
