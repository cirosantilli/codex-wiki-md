<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Associate to $f$ the symmetric [bilinear form](../../../../../bilinear-form.md) $B(u,v)=\tfrac12(f(u+v)-f(u)-f(v))$. If $f$ is identically zero, every [basis](../../../../../basis.md) is diagonal. Otherwise choose $v$ with $f(v)\ne0$. Every $w$ has the decomposition

$$
w=\frac{B(w,v)}{B(v,v)}v+\left(w-\frac{B(w,v)}{B(v,v)}v\right),
$$

whose second term lies in $v^\perp$. Thus $V=\mathbb Rv\oplus v^\perp$, with no cross term in $f$. Induction on dimension gives a diagonal [basis](../../../../../basis.md). Rescaling its nonzero entries reduces the form to

$$
f=\sum_{i=1}^px_i^2-\sum_{j=1}^qy_j^2,
$$

with $k$ additional zero coordinates. Define the [rank of a quadratic form](../../../../../rank-of-a-quadratic-form.md) $r=p+q$ and its [signature](../../../../../signature-of-a-quadratic-form.md) $s=p-q$. Rank is intrinsic, since it is the rank of $v\mapsto B(v,\cdot)$, equivalently $n-\dim\operatorname{rad}B$. Also $p$ is the greatest dimension of a subspace on which the restriction of $f$ is a [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md): any such subspace intersects the negative-plus-zero coordinate space only at zero, so its dimension is at most $p$, while the positive coordinate space attains $p$. The corresponding negative statement identifies $q$. This proves the basis independence of $r$ and $s$, the [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) conclusion.

For a [totally isotropic subspace](../../../../../totally-isotropic-subspace.md) $W$ on which $f$ vanishes, [polarization identity](../../../../../polarization-identity.md) also makes $B$ vanish on $W\times W$. Quotient by the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md). In the resulting nondegenerate form, projection of an isotropic subspace to either the positive or negative coordinate space is injective, so its dimension is at most $\min(p,q)$. Consequently $\dim W\le k+\min(p,q)$. The [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md) together with the vectors $e_i^++e_i^-$, $1\le i\le\min(p,q)$, attains this bound. The [maximum dimension of a totally isotropic subspace](../../../../../maximum-dimension-of-a-totally-isotropic-subspace.md) is therefore

$$
\boxed{\dim W_{\max}=n-r+\frac{r-|s|}{2}=n-\frac{r+|s|}{2}.}
$$

The [criterion for membership in a diagonal basis](../../../../../criterion-for-membership-in-a-diagonal-basis.md) follows similarly: a nonzero vector can belong to a diagonal [basis](../../../../../basis.md) if it has nonzero quadratic value, by the same orthogonal splitting, or if it lies in the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md), by choosing a radical basis containing it. An [isotropic vector](../../../../../isotropic-vector.md) in a diagonal [basis](../../../../../basis.md) must be orthogonal to every basis vector, and hence must lie in that radical. For the specified form, its radical is the $z$-axis, giving exactly

$$
\boxed{v=(x,y,z)\text{ qualifies iff }(x^2\ne y^2)\text{ or }(x=y=0\text{ and }z\ne0).}
$$

The zero vector never belongs to a [basis](../../../../../basis.md).

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
