<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A simply connected plane domain carrying a [hyperbolic metric](../../../../../../hyperbolic-metric.md) is proper. By the [Riemann mapping theorem](../../../../../../riemann-mapping-theorem.md), choose a [biholomorphism](../../../../../../biholomorphism.md) $\phi:\Omega\to\mathbb D$ sending a basepoint to zero. The same distance formula now gives

$$
1-|a_n|=(1+|a_n|)e^{-\rho(w,z_n)}\le2e^{-\rho(w,z_n)},\qquad a_n=\phi(z_n).
$$

Thus the [Blaschke condition](../../../../../../blaschke-condition.md) holds. In particular the $a_n$ have no interior accumulation point: near any such point the quantities $1-|a_n|$ would stay bounded away from zero.

Construct the [Blaschke product](../../../../../../blaschke-product.md)

$$
B(\zeta)=\zeta^m\prod_{a_n\ne0}\frac{|a_n|}{a_n}\frac{a_n-\zeta}{1-\overline{a_n}\zeta},\qquad m\in\{0,1\}.
$$

Here $m=1$ precisely when the sequence contains zero. For $|\zeta|\le r<1$, its normalized [Blaschke factor](../../../../../../blaschke-factor.md) $b_a$ satisfies

$$
1-b_a(\zeta)=\frac{(1-|a|)(1+(|a|/a)\zeta)}{1-\overline a\zeta},\qquad |1-b_a(\zeta)|\le\frac{1+r}{1-r}(1-|a|).
$$

The [Blaschke condition](../../../../../../blaschke-condition.md) therefore makes the [infinite product](../../../../../../infinite-product.md) converge uniformly on every compact subdisk. Away from the prescribed zeros its tail factors tend uniformly to one with summable errors, so their logarithms converge and the product is nonzero. It has exactly the prescribed zeros, and the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) bounds every finite partial product by one, hence $|B|\le1$. Thus **$f=B\circ\phi$ is the required bounded analytic function**, with no extra zeros.

Simple connectivity cannot be dropped. On the punctured disk choose

$$
w=e^{-1},\qquad z_n=e^{-n^2},\qquad n\ge2.
$$

The [hyperbolic metric on the punctured disk](../../../../../../hyperbolic-metric-on-the-punctured-disk.md) is $|dz|/(|z|\log(1/|z|))$. Its [universal covering map](../../../../../../universal-cover.md) $\tau\mapsto e^{i\tau}$ pulls it back to the curvature-minus-one upper-half-plane metric. The imaginary axis is a [geodesic](../../../../../../geodesic.md); the lift from $i$ to $in^2$ has length $\log n^2$, and any other lift differs by a real deck translation and has at least that distance. Therefore

$$
\rho(w,z_n)=2\log n,\qquad \sum_{n\ge2}e^{-\rho(w,z_n)}=\sum_{n\ge2}\frac1{n^2}<\infty.
$$

The [triangle inequality](../../../../../../triangle-inequality.md) again makes the sum finite for every basepoint. However, any bounded [holomorphic function](../../../../../../holomorphic-function.md) on the punctured disk extends over zero by the [Riemann removable singularity theorem](../../../../../../riemann-removable-singularity-theorem.md). These zeros accumulate at zero, so the [identity theorem](../../../../../../identity-theorem.md) makes the extension identically zero. It cannot have exactly the prescribed zero set. This example of [hyperbolic zero sequences on a punctured disk](../../../../../../hyperbolic-zero-sequences-on-a-punctured-disk.md) satisfies the distance condition but not the analytic zero-set condition.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
