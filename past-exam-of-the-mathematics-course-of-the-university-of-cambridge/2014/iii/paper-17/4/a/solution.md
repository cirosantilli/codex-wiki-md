<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The unheaded definitions use the [complex structure](../../../../../../complex-structure.md) $J$ on the real tangent bundle. Compatibility means $g(Ju,Jv)=g(u,v)$. Its [fundamental Hermitian form](../../../../../../fundamental-form-of-a-hermitian-manifold.md) is $\omega(u,v)=g(Ju,v)$; the compatibility identity makes this real, alternating and of type $(1,1)$. The metric is a [Kähler metric](../../../../../../kahler-metric.md) precisely when $d\omega=0$. In complex dimension one a real three-form is zero, so every compatible metric is a [Kähler metric](../../../../../../kahler-metric.md).

Now assume closedness and prove the [Kähler normal holomorphic coordinates](../../../../../../kahler-normal-holomorphic-coordinates.md) condition. Start with holomorphic coordinates $w$ centered at the point and make a complex-linear change so that the positive Hermitian coefficient matrix satisfies $h(0)=I$. Closedness of the $(1,1)$ form gives

$$
 \partial_{w_k}h_{i\bar j}=\partial_{w_i}h_{k\bar j}.
$$

Define $a_{i\bar j,k}=\partial_{w_k}h_{i\bar j}(0)$; it is symmetric in $i,k$. Choose new coordinates implicitly by

$$
 w_j=z_j-\frac12\sum_{i,k}a_{i\bar j,k}z_iz_k.
$$

The derivative of this [holomorphic map](../../../../../../holomorphic-map.md) at zero is the identity, so the [holomorphic inverse function theorem](../../../../../../holomorphic-inverse-function-theorem.md) makes $z$ valid local coordinates. In the new coordinates,

$$
 h'_{i\bar j}(z)=\sum_{a,b}h_{a\bar b}(w(z))
 \frac{\partial w_a}{\partial z_i}\overline{\frac{\partial w_b}{\partial z_j}}.
$$

At zero, $h'=I$, and differentiating gives

$$
 \partial_{z_k}h'_{i\bar j}(0)
 =a_{i\bar j,k}+\partial_{z_i}\partial_{z_k}w_j(0)=0.
$$

Hermitian symmetry makes all antiholomorphic first derivatives zero as well. [Taylor's theorem](../../../../../../taylor-theorem.md) for a [smooth function](../../../../../../smooth-function.md) now yields

$$
 \boxed{h'_{i\bar j}=\delta_{ij}+O(|z|^2).}
$$

Thus condition (a) implies condition (b), with the exact factor $i/2$ in the fundamental-form convention retained.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
