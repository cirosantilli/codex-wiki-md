<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the normalized [chordal metric](../../../../../chordal-metric.md)

$$
\boxed{\chi(z,w)=\frac{|z-w|}{\sqrt{1+|z|^2}\sqrt{1+|w|^2}},\qquad\chi(z,\infty)=\frac1{\sqrt{1+|z|^2}},\qquad\chi(\infty,\infty)=0.}
$$

Under [stereographic projection](../../../../../stereographic-projection.md) it is half the Euclidean chord distance on the unit sphere, which proves the metric axioms and the agreement with the usual sphere topology. If $\rho$ is spherical [geodesic](../../../../../geodesic.md) distance, then $\rho=2\arcsin\chi$, so $2\chi\leq\rho\leq\pi\chi$.

A [rational map](../../../../../rational-map-complex-analysis.md) is holomorphic, hence smooth, as a map of [compact](../../../../../compact-space.md) spheres. At a [pole](../../../../../pole.md) use $1/R$ as target coordinate, and at infinity use $1/z$ as source coordinate; neither is a singularity of the sphere map. Its differential in the round metric has a finite maximum norm $L$. Integrating its norm along a minimizing spherical [geodesic](../../../../../geodesic.md) gives $\rho(Rz,Rw)\leq L\rho(z,w)$. The preceding comparisons imply

$$
\boxed{\chi(Rz,Rw)\leq\frac{\pi L}{2}\chi(z,w).}
$$

This proves that the [rational map is Lipschitz in the chordal metric](../../../../../rational-map-is-lipschitz-in-the-chordal-metric.md). For a constant map take constant zero; for a nonconstant map the bound is finite by [compactness](../../../../../compact-space.md). In finite coordinates the differential norm is $R^\#(z)=|R'(z)|(1+|z|^2)/(1+|R(z)|^2)$, with its continuous sphere extension.

Now suppose $R,S$ are [commuting maps](../../../../../commuting-functions.md). We first prove $S(F(R))\subseteq F(R)$. The family $\{R^n\}$ is locally [equicontinuous](../../../../../equicontinuity.md) on $F(R)$, by the normality equivalence in question 1. Commutation and the Lipschitz estimate give, for all $n$,

$$
\chi(R^n(S(x)),R^n(S(x_0)))=\chi(S(R^n(x)),S(R^n(x_0)))\leq C_S\chi(R^n(x),R^n(x_0)).
$$

For $x_0\in F(R)$ choose a source ball within that [open set](../../../../../open-set.md), small enough to make the right side less than any prescribed $\epsilon$ uniformly in $n$. Holomorphic openness makes its image contain a ball about $S(x_0)$. Every point $w$ of that target ball has some preimage $x$ in the chosen source ball, so the same inequality proves [equicontinuity](../../../../../equicontinuity.md) of the iterates of $R$ at $S(x_0)$. Repeating at each point of the image gives local normality on that image. Thus the stated inclusion holds even where $S$ has a [rational critical point](../../../../../critical-point-of-a-rational-map.md).

Carefully state the permitted [Montel theorem](../../../../../montel-s-theorem.md): a family of meromorphic maps on an open domain, all omitting the same three distinct values of the [Riemann sphere](../../../../../riemann-sphere.md), is normal for locally uniform spherical convergence. Since $\deg R\geq2$, question 1 shows that $J(R)$ contains at least three distinct points. The forward inclusion just proved means every iterate of $S$ maps $F(R)$ into itself and therefore omits those three points there. Montel gives $F(R)\subseteq F(S)$. Exchanging the roles, using $\deg S\geq2$, gives the opposite inclusion. Consequently

$$
\boxed{F(R)=F(S),\qquad J(R)=J(S).}
$$

This proves that [commuting rational maps of degree at least two have the same Julia set](../../../../../commuting-rational-maps-of-degree-at-least-two-have-the-same-julia-set.md) without assuming either is an iterate of the other.

For [commuting maps](../../../../../commuting-functions.md) of degree one with different [Julia sets](../../../../../julia-set.md), take

$$
\boxed{R(z)=2z,\quad S(z)=z/2;\qquad J(R)=\{0\},\quad J(S)=\{\infty\}.}
$$

Their two compositions are the identity, and the [Julia sets](../../../../../julia-set.md) follow from the expanding and contracting Möbius cases in question 1.

For equal [Julia sets](../../../../../julia-set.md) without commutation, take

$$
\boxed{R(z)=z/2,\quad S(z)=z/2+1;\qquad J(R)=J(S)=\{\infty\}.}
$$

Both affine maps contract toward their finite [fixed points](../../../../../fixed-point.md) and have a [repelling periodic point](../../../../../repelling-periodic-point.md) at infinity. But $R\circ S=z/4+1/2$, while $S\circ R=z/4+1$, so they do not commute.

Finally the distinct [Chebyshev polynomials](../../../../../chebyshev-polynomial.md)

$$
\boxed{R(z)=2z^2-1,\qquad S(z)=4z^3-3z}
$$

have degrees two and three and neither is a pure power of $z$. Direct expansion gives both compositions equal to $32z^6-48z^4+18z^2-1$. Equivalently $T_m(T_n(z))=T_{mn}(z)$, first seen at $z=\cos\theta$ and then as a [polynomial identity](../../../../../polynomial-identity.md). This provides the requested higher-degree pair.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
