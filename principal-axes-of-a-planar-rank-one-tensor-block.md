# Principal axes of a planar rank-one tensor block

↑ **Parent:** [Symmetric tensor](symmetric-tensor.md)

For $v=(a,b,0)$ with $r=\sqrt{a^2+b^2}>0$, the [symmetric tensor](symmetric-tensor.md) $S=vv^T+cr^2e_3e_3^T$ has [principal axes](principal-axis.md)

$$
e_r=\frac1r(a,b,0),\qquad e_\theta=\frac1r(-b,a,0),\qquad e_3=(0,0,1),
$$

with [eigenvalues](eigenvalue.md) $r^2,0,cr^2$, respectively. This follows directly from the [outer product](outer-product.md): $vv^Tv=r^2v$, while it annihilates vectors perpendicular to $v$. The orthogonal matrix with rows $e_r^T,e_\theta^T,e_3^T$ gives $MSM^T=\operatorname{diag}(r^2,0,cr^2)$.

If $a,b$ depend on position, this is a pointwise eigenframe, not necessarily one fixed Cartesian change of axes throughout space. For $v=0$, the displayed tensor vanishes and every orthonormal basis is a principal basis. Subtracting a scalar multiple of the identity leaves its eigenvectors unchanged and shifts every eigenvalue by the same amount; this is a simple case of [coaxial symmetric tensors](coaxial-symmetric-tensors.md).

## ↑ Ancestors (8)

1. [Symmetric tensor](symmetric-tensor.md)
2. [Tensor](tensor.md)
3. [Multilinear algebra](multilinear-algebra-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/6/c/solution.md)
