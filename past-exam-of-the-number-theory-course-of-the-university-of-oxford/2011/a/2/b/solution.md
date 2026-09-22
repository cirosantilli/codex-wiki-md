<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Fundamental theorem of Galois theory](../../../../../fundamental-theorem-of-galois-theory.md) says that for a finite [Galois extension](../../../../../finite-galois-extension.md) $L/F$ with [group](../../../../../group-split.md) $G$, the maps $H\mapsto L^H$ and $E\mapsto\operatorname{Gal}(L/E)$ are mutually inverse inclusion-reversing correspondences between subgroups and intermediate fields. They satisfy $[L:L^H]=|H|$ and $[L^H:F]=[G:H]$. An intermediate extension $E/F$ is Galois exactly when its [subgroup](../../../../../subgroup.md) is normal, in which case its [group](../../../../../group-split.md) is the quotient by that [subgroup](../../../../../subgroup.md).

Let $a=\sqrt2$, $b=\sqrt3$, $c=i$. The real [field](../../../../../field.md) $\mathbb Q(a,b)$ has degree $4$: if $\sqrt3=u+v\sqrt2$ with $u,v\in\mathbb Q$, squaring forces $uv=0$ and either $u^2=3$ or $v^2=3/2$, both impossible. Adjoining the nonreal $i$ doubles the degree. All three square-root signs can be changed independently, giving

$$
\boxed{G\cong C_2^3,\qquad [L:\mathbb Q]=8.}
$$

Write $\sigma_{uvw}$ for the [automorphism](../../../../../automorphism.md) sending $(a,b,c)$ to $((-1)^ua,(-1)^vb,(-1)^wc)$, where $(u,v,w)\in\mathbb F_2^3$. Every nonzero vector generates an order-two [subgroup](../../../../../subgroup.md), so there are $7$ such subgroups. Their fixed fields are:

| Generator | Fixed field |
| --- | --- |
| $\sigma_{100}$ | $\mathbb Q(\sqrt3,i)$ |
| $\sigma_{010}$ | $\mathbb Q(\sqrt2,i)$ |
| $\sigma_{001}$ | $\mathbb Q(\sqrt2,\sqrt3)$ |
| $\sigma_{110}$ | $\mathbb Q(\sqrt6,i)$ |
| $\sigma_{101}$ | $\mathbb Q(\sqrt3,\sqrt{-2})$ |
| $\sigma_{011}$ | $\mathbb Q(\sqrt2,\sqrt{-3})$ |
| $\sigma_{111}$ | $\mathbb Q(\sqrt6,\sqrt{-2})$ |

Each listed [field](../../../../../field.md) has degree $4$ and is fixed by the indicated sign change, which proves equality with the fixed [field](../../../../../field.md).

There are also $7$ order-four subgroups: they are the kernels of the seven nonzero linear functionals on $\mathbb F_2^3$. For $e=(e_1,e_2,e_3)\ne0$, define $H_e=\{\sigma_{uvw}:e_1u+e_2v+e_3w=0\}$. Then

$$
L^{H_e}=\mathbb Q\left(\sqrt{2^{e_1}3^{e_2}(-1)^{e_3}}\right).
$$

Thus the seven quadratic fields have radicands $2,3,-1,6,-2,-3,-6$. Their square classes are distinct, so all are different. Finally the trivial [subgroup](../../../../../subgroup.md) fixes $L$, and all of $G$ fixes $\mathbb Q$. This accounts for every [subgroup](../../../../../subgroup.md) and intermediate [field](../../../../../field.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
