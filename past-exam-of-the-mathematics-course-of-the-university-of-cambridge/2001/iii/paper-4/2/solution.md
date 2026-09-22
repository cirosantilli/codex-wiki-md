<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [homogeneous coordinates](../../../../../homogeneous-coordinate.md) $X_0,\ldots,X_n$. Multiplication by these degree-one sections defines the [sheaf morphism](../../../../../morphism-of-sheaves.md)

$$
\epsilon:\mathcal O(-1)^{\oplus(n+1)}\longrightarrow\mathcal O,\qquad(s_0,\ldots,s_n)\longmapsto\sum_{j=0}^n X_j s_j.
$$

On $U_i=D_+(X_i)$, write $t_j^{(i)}=X_j/X_i$, with $t_i^{(i)}=1$, and let $E_j^{(i)}$ be the standard vector in component $j$ using the local [line bundle](../../../../../line-bundle.md) frame $X_i^{-1}$ of $\mathcal O(-1)$. Then $\epsilon(E_j^{(i)})=t_j^{(i)}$, so $\epsilon$ is surjective since $\epsilon(E_i^{(i)})=1$. Its [kernel](../../../../../kernel-of-a-linear-map.md) is a [locally free sheaf](../../../../../locally-free-sheaf.md) with basis

$$
F_j^{(i)}=E_j^{(i)}-t_j^{(i)}E_i^{(i)}\qquad(j\ne i).
$$

Indeed any vector in the kernel is uniquely a sum of these vectors, by solving for its $i$-th component.

The [Kähler differential sheaf](../../../../../sheaf-of-kahler-differentials-over-a-field.md) $\Omega^1_{\mathbf P^n/k}$ has basis $dt_j^{(i)}$ on $U_i$, since this chart is a polynomial [affine scheme](../../../../../affine-scheme.md). Define the local map $dt_j^{(i)}\mapsto F_j^{(i)}$. To check that these isomorphisms glue, on $U_i\cap U_\ell$ put $u=t_i^{(\ell)}$ and $v=t_j^{(\ell)}$. Then

$$
t_j^{(i)}=\frac vu,\qquad dt_j^{(i)}=u^{-1}dt_j^{(\ell)}-vu^{-2}dt_i^{(\ell)}.
$$

The [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) frame changes by $E_j^{(i)}=u^{-1}E_j^{(\ell)}$, hence

$$
F_j^{(i)}=u^{-1}F_j^{(\ell)}-vu^{-2}F_i^{(\ell)}.
$$

For $j=\ell$, use $t_\ell^{(\ell)}=1$, $dt_\ell^{(\ell)}=0$ and $F_\ell^{(\ell)}=0$; the same formula applies. Thus the differential and kernel frames have identical transition matrices. We obtain the cotangent form of the [Euler sequence](../../../../../euler-sequence.md):

$$
\boxed{0\longrightarrow\Omega^1_{\mathbf P^n/k}\longrightarrow\mathcal O(-1)^{\oplus(n+1)}\xrightarrow{\epsilon}\mathcal O\longrightarrow0.}
$$

This construction works over any [field](../../../../../field.md), including positive characteristic.

The [Kähler differential sheaf](../../../../../sheaf-of-kahler-differentials-over-a-field.md) has rank $n$. Taking [determinant line bundles](../../../../../determinant-line-bundle.md) in this locally split [short exact sequence of sheaves](../../../../../short-exact-sequence-of-sheaves.md) gives

$$
\det(\mathcal O(-1)^{\oplus(n+1)})\cong\det(\Omega^1_{\mathbf P^n/k})\otimes\det(\mathcal O).
$$

The left side is the tensor product of $n+1$ copies of $\mathcal O(-1)$, and $\det(\mathcal O)=\mathcal O$. Consequently

$$
\boxed{\bigwedge^n\Omega^1_{\mathbf P^n/k}\cong\mathcal O(-n-1).}
$$

It is the [canonical bundle of projective space](../../../../../canonical-bundle-of-projective-space.md). The determinant identity can also be seen directly by taking the wedge of the kernel basis followed by a lift of the quotient basis; changing that lift by a kernel vector leaves the wedge unchanged.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
