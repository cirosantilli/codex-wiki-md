<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $D^n_+$ and $D^n_-$ be the two closed hemispheres of the [sphere](../../../../../sphere.md). Use $\gamma$ as the [clutching function](../../../../../clutching-function.md) between the trivial bundles on these hemispheres. The [clutching construction](../../../../../clutching-construction.md) defines

$$
V_\gamma=
\bigl((D^n_+\times\mathbb R^k)\sqcup(D^n_-\times\mathbb R^k)\bigr)/\sim,
\qquad (u,v)_+\sim(u,\gamma(u)v)_-,\quad u\in S^{n-1}.
$$

The projection to $S^n$ is locally a [vector bundle](../../../../../vector-bundle.md). In a collar of the equator, extend the transition function by keeping it constant in the normal coordinate; this gives explicit [vector bundle trivializations](../../../../../vector-bundle-trivialization.md) across the seam. Since the transition matrices lie in the [special orthogonal group](../../../../../special-orthogonal-group.md), the standard fiber [orientations](../../../../../orientation-of-a-simplex.md) and Euclidean [inner products](../../../../../inner-product.md) agree on overlaps. Thus this is an oriented rank-$k$ [vector bundle](../../../../../vector-bundle.md) with a [fiber metric](../../../../../fiber-metric.md).

For $k\ge2$, choose a base point $u_0$ on the equator. A constant change of the negative hemisphere frame replaces $\gamma$ by $\gamma(u_0)^{-1}\gamma$, so we may suppose $\gamma(u_0)=I$. With $e_k$ the last standard unit vector, define the [section obstruction for a clutched vector bundle](../../../../../section-obstruction-for-a-clutched-vector-bundle.md)

$$
\boxed{f_\gamma=[u\longmapsto\gamma(u)e_k]\in\pi_{n-1}(S^{k-1});\qquad r=n-1,\ s=k-1.}
$$

The crucial point is that a [nowhere-zero section](../../../../../nowhere-zero-section.md) can be normalized using the [fiber metric](../../../../../fiber-metric.md). It is then represented by continuous maps $\sigma_\pm:D^n_\pm\to S^{k-1}$ satisfying

$$
\sigma_-(u)=\gamma(u)\sigma_+(u)
$$

on the equator.

If $f_\gamma=0$, the [extension-null-homotopy criterion for a sphere](../../../../../extension-null-homotopy-criterion-for-a-sphere.md) extends $u\mapsto\gamma(u)e_k$ to $D^n_-$. Take this extension as $\sigma_-$ and the constant map $e_k$ as $\sigma_+$. They glue to a [nowhere-zero section](../../../../../nowhere-zero-section.md).

Conversely, suppose such a section exists. Restricting a contraction of $D^n_+$ shows that $\sigma_+|_{S^{n-1}}$ is homotopic to a constant. The target [sphere](../../../../../sphere.md) is path connected, so the constant can be moved to $e_k$. Multiplying this homotopy pointwise by $\gamma(u)$ gives a [homotopy](../../../../../homotopy.md) from $\gamma\sigma_+$ to $\gamma e_k$. The first of these maps equals $\sigma_-|_{S^{n-1}}$ and extends over $D^n_-$, hence is [null-homotopic](../../../../../null-homotopic-map.md). So $\gamma e_k$ is [null-homotopic](../../../../../null-homotopic-map.md) too. A freely null-homotopic based sphere map represents zero in its [homotopy group](../../../../../homotopy-group.md); any change of base point sends the zero class to zero. We have proved both directions:

$$
\boxed{f_\gamma=0\quad\Longleftrightarrow\quad V_\gamma\text{ has a nowhere-zero section}.}
$$

For $n=1$, the same argument reads as the extension criterion for a two-point boundary and uses the trivial set $\pi_0(S^{k-1})$ when $k\ge2$. For $k=1$, the [special orthogonal group](../../../../../special-orthogonal-group.md) $SO(1)$ is trivial, so the [vector bundle](../../../../../vector-bundle.md) is already a [trivial vector bundle](../../../../../trivial-vector-bundle.md); the corresponding constant map to $S^0$ has zero obstruction. These cases require no higher [homotopy group](../../../../../homotopy-group.md) calculation.

If $k>n$, then $n-1<k-1$ and the permitted vanishing of lower [homotopy groups](../../../../../homotopy-group.md) of a [sphere](../../../../../sphere.md) makes $f_\gamma=0$. Normalize the resulting [nowhere-zero section](../../../../../nowhere-zero-section.md) to a unit section $\sigma$, and set

$$
V'_x=\{v\in(V_\gamma)_x:\langle v,\sigma(x)\rangle=0\}.
$$

Local orthonormal frames show that these [orthogonal complements](../../../../../orthogonal-complement.md) form a rank-$(k-1)$ [vector bundle](../../../../../vector-bundle.md). The explicit [vector bundle isomorphism](../../../../../vector-bundle-isomorphism.md)

$$
V'\oplus(S^n\times\mathbb R)\longrightarrow V_\gamma,
\qquad (x,v,t)\longmapsto v+t\sigma(x)
$$

has inverse $w\mapsto(w-\langle w,\sigma\rangle\sigma,\langle w,\sigma\rangle)$. Orient $V'$ so that a positive frame followed by $\sigma$ is positive in $V_\gamma$. This is [splitting a trivial line from a nowhere-zero section](../../../../../splitting-a-trivial-line-from-a-nowhere-zero-section.md) and proves the oriented splitting

$$
\boxed{V_\gamma\cong V'\oplus\mathbb R\qquad(k>n).}
$$

Finally consider the [special orthogonal sphere fibration](../../../../../special-orthogonal-sphere-fibration.md)

$$
SO(s)\longrightarrow SO(s+1)\xrightarrow{p}S^s,
\qquad p(A)=Ae_{s+1}.
$$

The fiber over $e_{s+1}$ consists exactly of $\operatorname{diag}(B,1)$ with $B\in SO(s)$. Near any unit vector, the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) continuously completes it to an oriented orthonormal frame, giving local sections of $p$ and local product [fiber bundle](../../../../../fiber-bundle-split.md) charts. In particular $p$ has the [homotopy lifting property](../../../../../homotopy-lifting-property.md).

Let $\alpha:S^r\to SO(s+1)$ be based and suppose $r<s$. The composite $p\alpha$ is a based [null-homotopic map](../../../../../null-homotopic-map.md) by the given vanishing of $\pi_r(S^s)$. Lift a based null-homotopy of $p\alpha$, beginning at $\alpha$, to a homotopy $G:S^r\times[0,1]\to SO(s+1)$. The lift might initially move its base point $u_0$, but $G(u_0,t)$ always fixes $e_{s+1}$. Right multiplication by $G(u_0,t)^{-1}$ corrects this: the homotopy

$$
\widetilde G(u,t)=G(u,t)G(u_0,t)^{-1}
$$

still covers the same sphere homotopy, remains based, and starts at $\alpha$. At its endpoint every matrix fixes $e_{s+1}$, so $\widetilde G(-,1)$ lies in the included $SO(s)$. Thus every [homotopy class](../../../../../homotopy-class.md) in the target is represented by one from $SO(s)$:

$$
\boxed{\pi_r(SO(s))\longrightarrow\pi_r(SO(s+1))\text{ is surjective for }r<s.}
$$

This proves [surjectivity of special orthogonal stabilization below the sphere dimension](../../../../../surjectivity-of-special-orthogonal-stabilization-below-the-sphere-dimension.md). For $r=0$, this is the corresponding assertion about path components; the positive-rank [special orthogonal groups](../../../../../special-orthogonal-group.md) are connected. The lifting argument also explains the zero term $\pi_r(S^s)$ in the [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
