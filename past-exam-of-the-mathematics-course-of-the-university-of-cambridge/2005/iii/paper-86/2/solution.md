<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the curvature-minus-one normalization of the [hyperbolic metric](../../../../../hyperbolic-metric.md):

$$
\boxed{ds_{\mathbb D}=\lambda(z)|dz|,\qquad\lambda(z)=\frac2{1-|z|^2}.}
$$

The associated distance is $d(z,w)=2\operatorname{artanh}|(z-w)/(1-\overline wz)|$. A connected [Riemann surface](../../../../../riemann-surfaces.md) has its complete canonical [Poincare metric on a Riemann surface](../../../../../poincare-metric-on-a-riemann-surface.md) precisely when its [universal cover](../../../../../universal-cover.md) is conformally the [unit disc](../../../../../unit-disc.md). By the [uniformization theorem](../../../../../uniformization-theorem.md), the other [simply connected](../../../../../simply-connected-space.md) covering types are the complex plane and [Riemann sphere](../../../../../riemann-sphere.md). Disc automorphisms preserve $\lambda(z)|dz|$, as direct differentiation of $(z-a)/(1-\overline az)$ shows; therefore the metric descends through the deck group. This is the uniformization notion of hyperbolicity, not the different potential-theoretic Green-function classification.

First prove the needed [Schwarz lemma](../../../../../schwarz-lemma.md). If $F:\mathbb D\to\mathbb D$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) and $F(0)=0$, then $F(z)/z$ extends holomorphically at zero. On $|z|=r<1$ its modulus is at most $1/r$. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) and $r\uparrow1$ give $|F(z)|\le|z|$ and $|F'(0)|\le1$.

Write $\psi_a(z)=(z-a)/(1-\overline az)$. Conjugating $f$ by the source and target disc automorphisms, $\psi_{f(a)}\circ f\circ\psi_a^{-1}$ fixes zero. Applying the [derivative](../../../../../derivative.md) bound gives

$$
\boxed{\frac{|f'(a)|}{1-|f(a)|^2}\le\frac1{1-|a|^2},\qquad f^*ds_{\mathbb D}\le ds_{\mathbb D}.}
$$

Integrate along any piecewise smooth path and then take the infimum of lengths: $d(f(z),f(w))\le d(z,w)$. This proves the [Schwarz-Pick theorem](../../../../../schwarz-pick-theorem.md). Contraction means nonexpansion, not a uniform Lipschitz constant strictly smaller than one; automorphisms preserve all distances.

If both $R$ and $S$ have disc universal covers, lift $g\circ\pi_R$ to $\widetilde g:\mathbb D\to\mathbb D$ through $\pi_S$. The disc is [simply connected](../../../../../simply-connected-space.md), so the lift exists, and it is [holomorphic](../../../../../complex-differentiability-at-a-point.md) because the [covering maps](../../../../../covering-space.md) are local [biholomorphisms](../../../../../biholomorphism.md). Both [covering maps](../../../../../covering-space.md) are local hyperbolic isometries. The disc contraction therefore descends to $g^*ds_S\le ds_R$ and, by the path-length argument, $d_S(g(p),g(q))\le d_R(p,q)$. If only $S$ is known to have a [hyperbolic metric](../../../../../hyperbolic-metric.md), a nonconstant $g$ forces $R$ to have one too: otherwise lift from the plane or sphere [universal cover](../../../../../universal-cover.md) of $R$ to the disc cover of $S$. A bounded entire function is constant by the [Liouville theorem](../../../../../liouville-theorem.md), and a [holomorphic map](../../../../../holomorphic-map.md) from the compact sphere into the disc is constant by the [maximum modulus principle](../../../../../maximum-modulus-principle.md). Thus **a nonconstant map into a hyperbolic surface is distance-nonincreasing between the canonical hyperbolic metrics; a nonhyperbolic source admits only constant such maps**.

For the prescribed point, [Schwarz-Pick theorem](../../../../../schwarz-pick-theorem.md) gives $|\psi_{w_0}(f(z))|\le|\psi_{z_0}(z)|$. Therefore

$$
h(z)=\frac{\psi_{w_0}(f(z))}{\psi_{z_0}(z)}
$$

is [holomorphic](../../../../../complex-differentiability-at-a-point.md) after filling the [removable singularity](../../../../../removable-singularity.md) at $z_0$, and $|h|\le1$. Inverting the target automorphism proves

$$
\boxed{f(z)=\frac{(z-z_0)h(z)+w_0(1-\overline z_0z)}{\overline w_0(z-z_0)h(z)+(1-\overline z_0z)},\qquad\sup_{\mathbb D}|h|\le1.}
$$

Conversely every [holomorphic](../../../../../complex-differentiability-at-a-point.md) $h$ with this bound gives an admissible disc map: $|\psi_{z_0}(z)h(z)|<1$, its inverse target automorphism remains in the disc, and the denominator cannot vanish.

Fix $z$ and put $r=|\psi_{z_0}(z)|<1$. The possible intermediate values fill $|v|\le r$, since constant choices $h\equiv c$, $|c|\le1$, attain them all. Thus the [one-point value region of a holomorphic disc map](../../../../../one-point-value-region-of-a-holomorphic-disc-map.md) is $|\psi_{w_0}(w)|\le r$. Completing the square in $|w-w_0|^2\le r^2|1-\overline w_0w|^2$ gives its Euclidean centre and radius:

$$
\boxed{C=\frac{(1-r^2)w_0}{1-r^2|w_0|^2},\qquad s=\frac{r(1-|w_0|^2)}{1-r^2|w_0|^2}.}
$$

This closed disc lies strictly inside the [unit disc](../../../../../unit-disc.md) because $r<1$. For $z=z_0$ it degenerates to the single point $w_0$. Its boundary is attainable by unimodular constant $h$; requiring $f$ to map into the open disc does not remove that boundary.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
