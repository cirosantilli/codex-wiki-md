<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [holomorphic normal bundle](../../../../../holomorphic-normal-bundle.md) is the quotient $N_V=T^{1,0}M|_V/T^{1,0}V$, of rank $r$. The tangent sequence is a [short exact sequence](../../../../../short-exact-sequence.md) of [holomorphic vector bundles](../../../../../holomorphic-vector-bundle.md):

$$
0\longrightarrow T^{1,0}V\longrightarrow T^{1,0}M|_V\longrightarrow N_V\longrightarrow0.
$$

Taking [determinant line bundles](../../../../../determinant-line-bundle.md) gives $\det(T^{1,0}M)|_V\cong\det(T^{1,0}V)\otimes\det N_V$. Dualizing and rearranging proves [adjunction for a smooth submanifold](../../../../../adjunction-for-a-smooth-submanifold.md):

$$
\boxed{K_V\cong K_M|_V\otimes\det N_V
=K_M|_V\otimes\bigwedge^rN_V.}
$$

The [determinant](../../../../../determinant.md) identity follows locally by adjoining lifts of a quotient frame to a subbundle frame; changing the lifts adds only off-diagonal blocks, so does not change the [determinant](../../../../../determinant.md).

For a smooth divisor, choose reduced local defining functions $f_i$, with $f_i=u_{ij}f_j$ and $u_{ij}$ holomorphic and nowhere zero. The [holomorphic line bundle associated to a divisor](../../../../../holomorphic-line-bundle-associated-to-a-divisor.md) $[V]=\mathcal O_M(V)$ has local frames $e_i=f_i^{-1}$, with $e_j=u_{ij}e_i$. The products $f_ie_i$ define its canonical section vanishing on $V$. Along $V$,

$$
df_i=u_{ij}\,df_j.
$$

Thus $v\mapsto df_i(v)e_i$ patches to a map $T^{1,0}M|_V\to[V]|_V$, whose kernel is $T^{1,0}V$ and which is surjective because each reduced defining function has nonzero differential there. Hence **$N_V\cong[V]|_V$**. This is the [normal bundle of a smooth analytic hypersurface](../../../../../normal-bundle-of-a-smooth-analytic-hypersurface.md). The divisor construction uses a closed hypersurface: an arbitrary nonclosed embedded hypersurface need not be a divisor. For example, a punctured line in $\mathbb C^2$ cannot be the support of a divisor, since its missing limit point would also lie in every local holomorphic zero set containing that line.

Let $s$ be the section of $E$ defining $V$. The intended hypothesis is that it is a [regular zero locus](../../../../../regular-zero-locus.md): $ds$ has rank $r$ on $V$. In a local trivialization, differentiation of the component functions defines

$$
ds:T^{1,0}M|_V\longrightarrow E|_V.
$$

This is intrinsic: differentiating a change-of-frame matrix introduces terms multiplied by $s$, which vanish on $V$. Its kernel is $T^{1,0}V$, so it induces an isomorphism of [holomorphic normal bundles](../../../../../holomorphic-normal-bundle.md). Consequently

$$
\boxed{N_V\cong E|_V,\qquad
K_V\cong\left(K_M\otimes L_1\otimes\cdots\otimes L_r\right)|_V.}
$$

This is the [normal bundle of a regular zero locus](../../../../../normal-bundle-of-a-regular-zero-locus.md). Here $\det E=L_1\otimes\cdots\otimes L_r$.

Regularity is essential if “vanishing” is read only as equality of underlying sets. On $\mathbb P^2$, the section $Z_0^2$ of $\mathcal O(2)$ vanishes set-theoretically on a smooth line $V$. Its derivative vanishes on $V$, and

$$
N_V\cong\mathcal O_{\mathbb P^1}(1)\not\cong\mathcal O_{\mathbb P^1}(2)=E|_V.
$$

Thus smoothness of the underlying zero set alone does not establish the claimed normal-bundle isomorphism. The preceding proof applies when the equations define the reduced smooth submanifold, equivalently are transverse to zero.

For [Complex projective space](../../../../../complex-projective-space.md), put $\mathcal O(a)=[aH]$. At a line $\ell\subset\mathbb C^{n+1}$, the tangent space is $\operatorname{Hom}(\ell,\mathbb C^{n+1}/\ell)$. Quotienting $\operatorname{Hom}(\ell,\mathbb C^{n+1})$ by its scalar maps into $\ell$ yields the [Euler sequence](../../../../../euler-sequence.md)

$$
0\longrightarrow\mathcal O\longrightarrow
\mathcal O(1)^{\oplus(n+1)}\longrightarrow T^{1,0}\mathbb P^n\longrightarrow0.
$$

Its [determinant](../../../../../determinant.md) gives **$K_{\mathbb P^n}\cong\mathcal O(-n-1)=[-(n+1)H]$**. For a smooth complete intersection defined regularly by the homogeneous equations, apply the normal-bundle result to $E=\bigoplus_i\mathcal O(d_i)$:

$$
\boxed{K_V\cong\mathcal O\!\left(\sum_{i=1}^r d_i-n-1\right)|_V
=\left[\left(\sum_i d_i-n-1\right)H\right]|_V.}
$$

This is the [canonical bundle of a regular projective complete intersection](../../../../../canonical-bundle-of-a-regular-projective-complete-intersection.md). The same regularity qualification is needed here: the squared-line example would otherwise predict $\mathcal O_{\mathbb P^1}(-1)$ for its [canonical bundle](../../../../../canonical-bundle.md), whereas the line has $K_V=\mathcal O_{\mathbb P^1}(-2)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
