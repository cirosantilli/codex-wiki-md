<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A [quadratic form](../../../../../quadratic-form.md) over $\mathbb R$ or $\mathbb C$ is a function $q(x)=B(x,x)$ for a symmetric [bilinear form](../../../../../bilinear-form.md) $B$, equivalently a homogeneous polynomial of degree two. Its polarization is $B(x,y)=[q(x+y)-q(x)-q(y)]/2$. If $q$ is not identically zero, choose $v$ with $q(v)\ne0$. Every $x$ decomposes as

$$
x=\frac{B(x,v)}{q(v)}v+\left(x-\frac{B(x,v)}{q(v)}v\right),
$$

where the second term lies in $v^\perp$ and $kv\cap v^\perp=\{0\}$. The [quadratic form](../../../../../quadratic-form.md) is consequently a direct sum of its one-dimensional value on $v$ and its restriction to $v^\perp$. Induction on dimension diagonalizes it. If $q=0$, any basis suffices. Rescale every nonzero diagonal coefficient: over the reals it becomes $1$ or $-1$, while over the complexes a square root makes it $1$. Hence

$$
\boxed{q(x)=\sum_{j=1}^na_jx_j^2,\qquad a_j\in\{-1,0,1\}.}
$$

Over $\mathbb C$ the negative coefficients can all be avoided.

For a real [quadratic form](../../../../../quadratic-form.md), let $p$ and $m$ be its positive and negative indices in a diagonalization. Its [rank of a quadratic form](../../../../../rank-of-a-quadratic-form.md) is $p+m$ and its [signature of a quadratic form](../../../../../signature-of-a-quadratic-form.md) is $p-m$, or the ordered pair $(p,m)$ in the alternative convention. These indices are intrinsic: the largest dimension of a subspace where the form is positive definite is $p$, since any larger subspace intersects the nonpositive coordinate subspace nontrivially; similarly for $m$. For the form here, completing squares gives

$$
q=(x_2+x_1+x_3)^2-(2x_1+x_3)^2.
$$

The two displayed linear coordinates, together with $x_1$, form an invertible coordinate change. Therefore

$$
\boxed{\operatorname{rank}q=2,\qquad(p,m)=(1,1),\qquad\operatorname{signature}q=0.}
$$

There is one zero coordinate direction.

The PDF's final dimension condition is $n\ge2^d$, not the fraction produced by the TeX conversion. We prove the requested [common zero of complex quadratic forms](../../../../../common-zero-of-complex-quadratic-forms.md) by induction on $d$. A complex [quadratic form](../../../../../quadratic-form.md) of rank $r$ has canonical expression $x_1^2+\cdots+x_r^2$. Pair its nonzero coordinates into vectors $e_{2j-1}+ie_{2j}$ and add the $n-r$ radical coordinate vectors. Their span is a [totally isotropic subspace](../../../../../totally-isotropic-subspace.md), because the form is zero on every linear combination. This proves that [complex quadratic forms have a large isotropic subspace](../../../../../complex-quadratic-forms-have-a-large-isotropic-subspace.md): its dimension is

$$
\left\lfloor\frac r2\right\rfloor+n-r=n-\left\lceil\frac r2\right\rceil\ge\left\lfloor\frac n2\right\rfloor.
$$

For $d=0$ there is a nonzero vector whenever $n\ge1$. For $d\ge1$, take such a subspace $E$ for $q_1$. If $n\ge2^d$, then $\dim E\ge2^{d-1}$. Apply the induction hypothesis to the restrictions of $q_2,\ldots,q_d$ to $E$. It supplies a nonzero $x\in E$ annihilated by those forms, and $q_1(x)=0$ by construction. Thus

$$
\boxed{\exists x\ne0:\ q_1(x)=\cdots=q_d(x)=0\quad\text{when }n\ge2^d.}
$$

The argument makes no nondegeneracy assumption on any of the forms.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
