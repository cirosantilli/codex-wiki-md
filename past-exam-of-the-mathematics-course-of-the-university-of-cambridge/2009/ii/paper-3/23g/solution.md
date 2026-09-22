<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

For a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $D$, let $L(D)=H^0(V,\mathcal O(D))$ and choose a basis of dimension $r+1$. Regarding the basis as sections of the [divisor line bundle](../../../../../divisor-line-bundle.md), evaluation gives $\phi_D:V\to\mathbb P^r$. If the [linear system of divisors](../../../../../linear-system-of-divisors.md) has no base points, at least one section is nonzero at each point, and these homogeneous coordinates define a [morphism](../../../../../morphism.md). If the effective divisor has a fixed part $F$, first divide all sections by their common vanishing factor. The moving divisor $E=D-F$ is base-point-free, has the same section space, and gives the uniquely extended morphism on the smooth curve. Thus effectiveness alone does not make the raw evaluations everywhere nonzero, but cancellation supplies the usual map.

A morphism from a projective integral curve is a [finite morphism](../../../../../finite-morphism.md) onto its image precisely when it is nonconstant, equivalently $r\ge1$: a positive-dimensional fiber of a curve would be the whole curve, while a nonconstant proper map with finite fibers is finite. It is an isomorphism onto its image precisely when its moving complete linear system is [very ample](../../../../../very-ample-line-bundle.md). In section-space terms, putting $h=h^0(E)$, the criteria are

$$
h^0(E-P)=h-1\quad\text{for all }P,\qquad h^0(E-P-Q)=h-2\quad\text{for all }P,Q,
$$

where $Q=P$ is allowed. These express absence of base points, separation of distinct points, and separation of tangent directions. In the base-point-free convention $E=D$.

Now suppose the genus is two. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $\deg K=2$ and $h^0(K)=2$. There cannot be a nonconstant function with only a single simple pole on a positive-genus smooth projective curve: it would give a degree-one map to $\mathbb P^1$, an isomorphism. Hence $h^0(P)=1$ for every point $P$. Applying [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) to $K-P$ gives $h^0(K-P)=h^0(P)=1$, so the canonical linear system has no base point. The resulting map $\phi_K:V\to\mathbb P^1$ has degree $\deg K=2$.

Set $D=K+P_1+P_2$, of degree four. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(D)=3$ and $h^0(D-P)=2$ for every $P$, since the residual divisors have negative degree. Thus $\phi_D$ is a base-point-free map to $\mathbb P^2$ with nondegenerate image $C$. Degree of the pullback of a general line gives

$$
4=(\deg\phi_D)(\deg C).
$$

The image cannot be a line because the three sections are independent. The only alternatives are a birational quartic or a double cover of a conic. In the latter case identify the smooth conic with $\mathbb P^1$. Its hyperplane bundle has degree two, so $D\sim2A$, where $A$ is a degree-two divisor with $h^0(A)\ge2$. Again [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) implies $h^0(K-A)=h^0(A)-1\ge1$. Since $K-A$ has degree zero, it must be linearly equivalent to zero; hence $A\sim K$. This would force $P_1+P_2\sim K$, contrary to the hypothesis. Therefore the image is a plane quartic and the map is birational. A smooth plane quartic has genus $(4-1)(4-2)/2=3$, while its normalization here has genus two. Consequently $\boxed{\phi_D\text{ is birational onto a singular plane quartic}}$.

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
