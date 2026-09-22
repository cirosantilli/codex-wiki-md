<h1 id="20i/solution">Solution</h1>

↑ **Parent:** [20I](../20i.md)

Suppose first that $F:D^n\to X$ extends $f$. Regarding $S^{n-1}$ as the boundary of the unit disc,

$$
H(x,t)=F((1-t)x)
$$

is a [homotopy](../../../../../homotopy.md) from $f$ to the constant map with value $F(0)$. Thus $f$ is [null-homotopic](../../../../../null-homotopic-map.md). Conversely, if $H:S^{n-1}\times[0,1]\to X$ is a homotopy from $f$ to a constant, then $H$ is constant on $S^{n-1}\times\{1\}$ and hence descends to the quotient

$$
S^{n-1}\times[0,1]/(S^{n-1}\times\{1\}),
$$

which is the cone on $S^{n-1}$ and is homeomorphic to $D^n$. The descended map extends $f$. This proves the [extension-null-homotopy criterion for a sphere](../../../../../extension-null-homotopy-criterion-for-a-sphere.md).

A [universal cover](../../../../../universal-cover.md) of $X$ is a covering map $p:\widetilde X\to X$ whose total space is path-connected and simply connected. Let $p_1:(\widetilde X_1,\widetilde x_1)\to(X,x)$ and $p_2:(\widetilde X_2,\widetilde x_2)\to(X,x)$ be two universal covers. The [lifting criterion for a covering space](../../../../../lifting-criterion-for-a-covering-space.md) applies because

$$
(p_1)_*\pi_1(\widetilde X_1)=0
\subseteq(p_2)_*\pi_1(\widetilde X_2)=0,
$$

so $p_1$ has a based lift $h:\widetilde X_1\to\widetilde X_2$ satisfying $p_2h=p_1$. Similarly there is a based lift $k:\widetilde X_2\to\widetilde X_1$ of $p_2$. Both $kh$ and the identity are lifts of $p_1$ that agree at the base point, so uniqueness of lifts gives $kh=1$. Likewise $hk=1$. Hence $h$ is a homeomorphism. This is the [uniqueness of a universal covering space](../../../../../uniqueness-of-a-universal-covering-space.md).

Now let $p:\widetilde X\to X$ be universal with $\widetilde X$ contractible. If an extension $F:|K|\to X$ exists, functoriality of the [fundamental group](../../../../../fundamental-group.md) gives

$$
f_*=F_*i_*.
$$

Thus the required factorization holds with $\Phi=F_*$.

Conversely, suppose $f_*=\Phi i_*$. We extend over the simplices of $K$ by dimension. The boundary of every 2-simplex is a loop in $|K^1|$ that becomes null-homotopic in $|K|$, so its class lies in $\ker i_*$. The factorization gives

$$
f_*[\partial\sigma]=\Phi i_*[\partial\sigma]=1.
$$

Hence $f|_{\partial\sigma}$ is null-homotopic in $X$ and extends over the disc $|\sigma|$ by the first part. Since distinct 2-simplices meet along the already fixed 1-skeleton, these extensions combine to a map on $|K^2|$.

Inductively suppose the map is defined on $|K^{m-1}|$ for $m\geq3$. For an $m$-simplex $\sigma$, its boundary is $S^{m-1}$, which is simply connected. The boundary map therefore lifts through $p$ by the covering-space lifting criterion. Its lift into the [contractible space](../../../../../contractible-space.md) $\widetilde X$ is null-homotopic, so the boundary map itself is null-homotopic and extends over $|\sigma|$. Extending over every $m$-simplex and then every skeleton constructs $F:|K|\to X$. The weak topology on a simplicial complex makes the cellwise map continuous. This proves the [extension criterion into a space with contractible universal cover](../../../../../extension-criterion-into-a-space-with-contractible-universal-cover.md).

## ↑ Ancestors (10)

1. [20I](../20i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
