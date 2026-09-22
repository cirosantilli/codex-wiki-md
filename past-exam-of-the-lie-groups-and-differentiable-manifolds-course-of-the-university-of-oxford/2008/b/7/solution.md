<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For [compact](../../../../compact-space.md) [connected](../../../../connected-space.md) oriented $n$-manifolds without boundary, the degree is characterized by

$$
\int_MF^*\eta=\deg(F)\int_N\eta
$$

for every smooth top-degree form $\eta$. Equivalently, at any [regular value](../../../../regular-value.md) $y$,

$$
\deg(F)=\sum_{x\in F^{-1}(y)}\operatorname{sign}\det D F_x.
$$

The [preimage](../../../../preimage.md) is finite by [compactness](../../../../compact-space.md) and the [inverse function theorem](../../../../inverse-function-theorem.md). Taking a form supported in a small neighbourhood of a [regular value](../../../../regular-value.md) and applying change of variables proves the signed-count formula. The top [de Rham cohomology](../../../../de-rham-cohomology.md) of a [compact](../../../../compact-space.md) [connected](../../../../connected-space.md) oriented [manifold](../../../../topological-manifold-split.md) is one-dimensional, with integration giving its coordinate; [pullback](../../../../pullback-category-theory.md) and [Stokes theorem](../../../../stokes-theorem.md) make the integral characterization independent of the chosen normalized form. Thus this signed count is independent of the [regular value](../../../../regular-value.md). In particular a nonzero degree forces surjectivity, and the number of points in any regular fibre is at least the absolute degree. Degree is invariant under [homotopy](../../../../homotopy-split.md), as follows by applying [Stokes theorem](../../../../stokes-theorem.md) to the [pullback](../../../../pullback-category-theory.md) on $M\times[0,1]$.

For the [polynomial](../../../../polynomial-split.md) assertion take $k\ge1$. The map $P:\mathbb C\to\mathbb C$ extends smoothly to a map of the [Riemann sphere](../../../../riemann-sphere.md) fixing infinity: in reciprocal coordinates its target coordinate is

$$
\frac1{P(1/\zeta)}=\frac{\zeta^k}{1+a_1\zeta+\cdots+a_k\zeta^k}.
$$

The [homotopy](../../../../homotopy-split.md) $P_t(z)=z^k+t(a_1z^{k-1}+\cdots+a_k)$ extends smoothly in the same way. The map $z\mapsto z^k$ has $k$ distinct inverse images of the [regular value](../../../../regular-value.md) one, each [orientation](../../../../orientation-of-a-simplex.md)-preserving, since the real Jacobian of multiplication by a nonzero complex derivative is its squared absolute value. Its degree is $k$, so $\deg P=k\ne0$. It is onto the sphere and must attain zero at a finite point. This proves **every nonconstant complex [polynomial](../../../../polynomial-split.md) has a root**, without assuming the result to count roots of a general [polynomial](../../../../polynomial-split.md).

For a proper smooth $F:\mathbb R^n\to\mathbb R^n$, choose a compactly supported $n$-form $\eta$ with $\int\eta=1$ and define

$$
\deg F=\int_{\mathbb R^n}F^*\eta.
$$

Properness makes its [pullback](../../../../pullback-category-theory.md) compactly supported. If $\eta'$ is another choice, the given result gives $\eta-\eta'=d\beta$ with [compact](../../../../compact-space.md) support. The difference of the defining integrals is $\int d(F^*\beta)=0$, proving [independence](../../../../independent-random-variables.md). Sard's theorem supplies a [regular value](../../../../regular-value.md). A [proper map](../../../../proper-map.md) has finitely many preimages of it, and a sufficiently small neighbourhood has no additional inverse sheets outside the chosen inverse-[function](../../../../function-split.md) neighbourhoods: otherwise a sequence of extra preimages would have a convergent subsequence by properness and limit in that fibre. A normalized form there therefore gives the same finite signed-count formula, proving that the degree is an [integer](../../../../integer-split.md).

Finally $x\mapsto x^k$ is proper for $k\ge1$. For odd $k$, a positive [regular value](../../../../regular-value.md) has one inverse image with positive derivative. For positive even $k$, it has two inverse images with opposite derivative signs. Consequently

$$
\boxed{\deg(x\mapsto x^k)=\begin{cases}1,&k\ge1\text{ odd},\\0,&k\ge2\text{ even}.\end{cases}}
$$

For $k=0$ it is the constant map one, whose inverse image of the [compact](../../../../compact-space.md) singleton $\{1\}$ is all of $\mathbb R$. It is **not proper**, so its degree is not defined by the proper-map construction requested here.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the lie Groups and Differentiable Manifolds course of the University of Oxford](../../../split.md)
5. [Lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
