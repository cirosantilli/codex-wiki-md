<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose an [orthonormal basis](../../../../../orthonormal-basis.md) with $\mathbf n=\mathbf e_3$. A half-turn about $\mathbf n$ kills all mixed axial-transverse components. Commutation with a quarter-turn makes the transverse block a scalar [identity matrix](../../../../../identity-matrix.md) plus an [antisymmetric matrix](../../../../../skew-symmetric-matrix.md). The resulting [oriented-axis invariant Cartesian tensor](../../../../../oriented-axis-invariant-cartesian-tensor.md), in coordinate-free form, is

$$
\boxed{\sigma_{ij}=a(\delta_{ij}-n_in_j)+d\,n_in_j+h\epsilon_{ikj}n_k,}
$$

with real constants $a,d,h$. The [Kronecker delta](../../../../../kronecker-delta.md), the [outer product](../../../../../outer-product.md) $n_in_j$, and the displayed [Levi-Civita symbol](../../../../../levi-civita-symbol.md) contraction are invariant under every proper rotation about $\mathbf n$, so this form is also sufficient. In the chosen basis,

$$
\sigma=\begin{pmatrix}a&-h&0\\h&a&0\\0&0&d\end{pmatrix}.
$$

The antisymmetric part must be retained unless further symmetry is imposed.

Decompose the [electric field](../../../../../electric-field-split.md) as $\mathbf E=\mathbf E_\perp+\mathbf E_\parallel$, where $\mathbf E_\parallel=(\mathbf n\cdot\mathbf E)\mathbf n$. The [electric current density](../../../../../current-density.md) is

$$
\mathbf J=a\mathbf E_\perp+d\mathbf E_\parallel+h\mathbf n\times\mathbf E_\perp.
$$

For a nonzero real [electric field](../../../../../electric-field-split.md), the [alignment of current and field in an axisymmetric conductor](../../../../../alignment-of-current-and-field-in-an-axisymmetric-conductor.md) gives the complete classification of [collinearity](../../../../../collinearity.md):

- If $\mathbf E_\perp=0$, then $\boxed{\mathbf J=d\mathbf E}$, with no additional symmetry required.
- If $\mathbf E_\parallel=0$, then $\boxed{\mathbf J\parallel\mathbf E\ \Longleftrightarrow\ h=0}$. Within this family $h=0$ is exactly the condition that the [conductivity tensor](../../../../../conductivity-tensor.md) is symmetric; then $\mathbf J=a\mathbf E$. An additional half-turn symmetry about a transverse axis is one way to force $h=0$.
- If both components are nonzero, then $\boxed{\mathbf J\parallel\mathbf E\ \Longleftrightarrow\ h=0\text{ and }a=d}$. These conditions give the [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md) $\sigma=aI$, and then $\mathbf J=a\mathbf E$ for every direction.

For completeness, if $\mathbf E_\perp\ne0$ and $\mathbf J=\lambda\mathbf E$, taking the [dot product](../../../../../dot-product.md) with $\mathbf n\times\mathbf E_\perp$ forces $h=0$. The transverse equation then gives $\lambda=a$, while a nonzero axial component gives $\lambda=d$. This proves there are no missing directions. Zero current is included as the zero scalar multiple; if “parallel” requires a direction for $\mathbf J$, exclude cases where that scalar is zero. For a strictly anisotropic crystal the last possibility is absent.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
