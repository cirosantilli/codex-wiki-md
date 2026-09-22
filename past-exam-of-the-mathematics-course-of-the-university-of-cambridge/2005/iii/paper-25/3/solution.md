<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a framed embedding $S^{\lambda-1}\times D^{m+1-\lambda}\hookrightarrow M^m$, index-$\lambda$ [surgery on a smooth manifold](../../../../../surgery-on-a-smooth-manifold.md) removes the interior of that region and replaces it by $D^\lambda\times S^{m-\lambda}$. Their common boundary is $S^{\lambda-1}\times S^{m-\lambda}$, along which the framing specifies the gluing. This is a $(\lambda,m+1-\lambda)$ surgery. Its trace is an $(m+1)$-dimensional [cobordism](../../../../../cobordism.md) obtained by attaching the [handle](../../../../../handle.md) $D^\lambda\times D^{m+1-\lambda}$ to $M\times[0,1]$ along the outgoing boundary.

In the present [surface](../../../../../topological-surface.md) case, $\lambda=2$ and $m=2$. The operation removes an annulus around the embedded curve $\gamma$ and caps its two boundary circles by [closed disks](../../../../../closed-disc.md). Since $[\gamma]=pa+qb\ne0$, the curve cannot separate the oriented [torus](../../../../../torus.md): a separating curve is the oriented boundary of one of the complementary subsurfaces and is therefore null-homologous. Thus it is a [nonseparating curve](../../../../../nonseparating-curve.md), and the cut-open [surface](../../../../../topological-surface.md) $F$ is connected with two boundary components. Its [Euler characteristic](../../../../../euler-characteristic.md) is zero, since both the removed annulus and the gluing circles have [Euler characteristic](../../../../../euler-characteristic.md) zero. Capping adds two, so the resulting oriented closed connected [surface](../../../../../topological-surface.md) has $\chi(M)=2$. By the allowed [surface](../../../../../topological-surface.md) classification it is a [sphere](../../../../../sphere.md). Therefore

$$
\boxed{H_0(M;\mathbb Z)=\mathbb Z,\qquad H_1(M;\mathbb Z)=0,\qquad H_2(M;\mathbb Z)=\mathbb Z,\qquad H_i(M;\mathbb Z)=0\ (i>2).}
$$

Equivalently the classification shows that $F$ is a cylinder. The argument is conditional on the asserted embedding existing; it does not assign a surgery [manifold](../../../../../topological-manifold.md) to a nonexistent embedded curve.

Choose an arc in this connected cylinder joining its two boundary circles and close it by an arc crossing the removed annulus. After smoothing the joints, its closed curve $\delta$ meets $\gamma$ transversely exactly once. If $[\delta]=ra+sb$, then their [algebraic intersection number of curves on an oriented surface](../../../../../algebraic-intersection-number-of-curves-on-an-oriented-surface.md) is

$$
[\gamma]\cdot[\delta]=ps-qr=\pm1.
$$

This proves that $[\gamma]$ is a [primitive homology class](../../../../../primitive-homology-class.md) and forces $\gcd(p,q)=1$.

Conversely, if $\gcd(p,q)=1$, the map

$$
\mathbb R/\mathbb Z\longrightarrow(\mathbb R/\mathbb Z)^2,\qquad t\longmapsto(pt,qt)
$$

is an immersion with the required [homology](../../../../../homology-split.md) class. If its values at $t,s$ coincide, then $p(t-s)$ and $q(t-s)$ are integers; [Bézout's identity](../../../../../bezout-identity.md) gives $t-s\in\mathbb Z$. It is therefore injective and, by compactness, an embedded circle. An explicit annular thickening is

$$
\iota(t,u)=(pt-q\delta u,\ qt+p\delta u)\pmod{\mathbb Z^2},\qquad u\in[-1,1],\quad0<\delta<\frac1{2(p^2+q^2)}.
$$

The determinant of its coordinate derivatives is $\delta(p^2+q^2)\ne0$. If two image points coincide, solving for the difference in the normal coordinate shows that $\delta(u-u')$ is an integer multiple of $1/(p^2+q^2)$. The strict choice of $\delta$ forces that integer to be zero, so $u=u'$ and then $t=t'$ modulo one. This supplies the actual required embedding, not just a [homology](../../../../../homology-split.md) class. Hence

$$
\boxed{\text{a positive }(p,q)\text{-curve exists if and only if }\gcd(p,q)=1.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
