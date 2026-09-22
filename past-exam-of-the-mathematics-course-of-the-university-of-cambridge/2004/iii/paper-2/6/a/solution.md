<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V$ have dimension $2m$ over the [finite field](../../../../../../finite-field.md) $\mathbb F_q$, with a [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) [alternating bilinear form](../../../../../../alternating-bilinear-form.md) $B$. The [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md) is

$$
Sp(V,B)=\{g\in GL(V):B(gx,gy)=B(x,y)\text{ for all }x,y\}.
$$

It acts simply transitively on ordered [symplectic bases](../../../../../../symplectic-basis.md): a [linear map](../../../../../../linear-map.md) between two such bases is uniquely specified and preserves all pairings, hence the whole [bilinear form](../../../../../../bilinear-form.md).

Count a first [hyperbolic pair](../../../../../../hyperbolic-pair.md) $(e_1,f_1)$. There are $q^{2m}-1$ choices for $e_1\ne0$. Nondegeneracy makes $B(e_1,-)$ a nonzero [linear functional](../../../../../../linear-functional.md), so there are $q^{2m-1}$ choices of $f_1$ with $B(e_1,f_1)=1$. Their span is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md), and its [symplectic orthogonal complement](../../../../../../symplectic-orthogonal-complement.md) is a [symplectic vector space](../../../../../../symplectic-vector-space.md) of dimension $2m-2$. Recursing, with $|Sp_0(q)|=1$, yields

$$
\boxed{|Sp_{2m}(q)|=\prod_{i=1}^m(q^{2i}-1)q^{2i-1}
=q^{m^2}\prod_{i=1}^m(q^{2i}-1).}
$$

The construction also proves the existence of the required [symplectic bases](../../../../../../symplectic-basis.md), in [characteristic](../../../../../../characteristic-of-a-field.md) two as well as odd [characteristic](../../../../../../characteristic-of-a-field.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
