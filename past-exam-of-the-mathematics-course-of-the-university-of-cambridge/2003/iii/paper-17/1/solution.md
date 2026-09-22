<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [symplectic vector space](../../../../../symplectic-vector-space.md) $(V,\omega)$ and a [vector subspace](../../../../../vector-subspace.md) $W$, the [symplectic orthogonal complement](../../../../../symplectic-orthogonal-complement.md) is

$$
W^\omega=\{v\in V:\omega(v,w)=0\text{ for every }w\in W\}.
$$

[Nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md) identifies $V$ with its [dual space](../../../../../dual-space.md), so $\dim W^\omega=\dim V-\dim W$. If $W$ is a [symplectic subspace](../../../../../symplectic-subspace.md), $W\cap W^\omega=0$, and hence $V=W\oplus W^\omega$; the restriction to $W^\omega$ is also nondegenerate.

Here is an inductive construction of a [symplectic basis](../../../../../symplectic-basis.md). Choose $e_1\ne0$. [Nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md) supplies $f_1$ with $\omega(e_1,f_1)=1$. The plane $P=\operatorname{span}(e_1,f_1)$ is a [symplectic subspace](../../../../../symplectic-subspace.md), and its [symplectic orthogonal complement](../../../../../symplectic-orthogonal-complement.md) gives $V=P\oplus P^\omega$. Repeat on $P^\omega$. The process ends in dimension zero, since each step removes two dimensions and a one-dimensional alternating form is degenerate. We obtain $e_1,f_1,\ldots,e_n,f_n$ with

$$
\omega(e_i,e_j)=\omega(f_i,f_j)=0,\qquad\omega(e_i,f_j)=\delta_{ij}.
$$

The [linear map](../../../../../linear-map.md) taking the coordinate vectors of $\mathbb R^{2n}$ to this basis pulls $\omega$ back to $\sum_jdx_j\wedge dy_j$, proving the asserted normal form.

Now split $V=C\oplus D$ with $D=C^\omega$, and choose [symplectic bases](../../../../../symplectic-basis.md) on both planes. Parametrize $\Gamma_A$ by $v\mapsto(Av,v)$. Orthogonality removes the cross terms, and a two-dimensional alternating form transforms by the [determinant](../../../../../determinant.md), so

$$
\omega|_{\Gamma_A}\longleftrightarrow A^*\omega_C+\omega_D=(1+\det A)\omega_D.
$$

Consequently the correct [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md) criterion is

$$
\boxed{\Gamma_A\text{ is symplectic}\iff\det A\ne-1.}
$$

The strict inequality printed in the PDF requires an extra orientation condition: it says that the [symplectic orientation](../../../../../symplectic-orientation.md) on the graph agrees with the orientation transported from $D$. It is not equivalent to being a [symplectic subspace](../../../../../symplectic-subspace.md). For example, $A=\operatorname{diag}(-2,1)$ has [determinant](../../../../../determinant.md) $-2$ and gives a nondegenerate restriction $-\omega_D$. This is the [orientation criterion for a graph of symplectic planes](../../../../../orientation-criterion-for-a-graph-of-symplectic-planes.md).

This same map supplies the requested obstruction. Orient $C$ and $\Gamma_A$ by their restricted [symplectic forms](../../../../../symplectic-form.md). If $(d_1,d_2)$ is a positive basis of $D$, then $(Ad_1+d_1,Ad_2+d_2)$ is negatively oriented in $\Gamma_A$. The coordinate transformation from a basis of $C$ followed by these graph vectors to a basis of $C\oplus D$ has [determinant](../../../../../determinant.md) $1$. Reversing the graph basis to give its positive orientation therefore makes the oriented direct sum $C\oplus\Gamma_A$ negative relative to the ambient [symplectic orientation](../../../../../symplectic-orientation.md).

Two distinct complex lines in standard $\mathbb C^2$ have the opposite behaviour: complex bases of the two lines give a complex-linear [isomorphism](../../../../../isomorphism.md) $\mathbb C\oplus\mathbb C\to\mathbb C^2$, whose real [determinant](../../../../../determinant.md) is the positive number $|\det_{\mathbb C}|^2$. Their complex orientations are their [symplectic orientations](../../../../../symplectic-orientation.md). A [symplectic linear map](../../../../../symplectic-linear-map.md) preserves both the ambient and each plane's [symplectic orientation](../../../../../symplectic-orientation.md), so it cannot change this sign. Thus **the pair with $A=\operatorname{diag}(-2,1)$ cannot be the image of a pair of complex lines**. Interchanging the planes does not change the sign, since both dimensions are even.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
