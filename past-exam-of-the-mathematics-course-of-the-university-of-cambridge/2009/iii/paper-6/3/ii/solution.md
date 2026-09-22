<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $U$ be a four-dimensional [symplectic vector space](../../../../../../symplectic-vector-space.md), with a [symplectic basis](../../../../../../symplectic-basis.md) $e_1,f_1,e_2,f_2$. Its invariant inverse-form bivector may be chosen as $\eta=e_1\wedge f_1+e_2\wedge f_2$. Put $\mathrm{vol}=e_1\wedge f_1\wedge e_2\wedge f_2$, so $\eta\wedge\eta=2\mathrm{vol}$. Define a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) on the six-dimensional [exterior square](../../../../../../exterior-square.md) by

$$
\xi\wedge\zeta=B(\xi,\zeta)\mathrm{vol}.
$$

It is symmetric because both factors have degree two. It is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md): in the six-element wedge [basis](../../../../../../basis.md), every $e_a\wedge e_b$ pairs nontrivially with the wedge of the complementary pair and with no other [basis](../../../../../../basis.md) vector. Since $B(\eta,\eta)=2$, the [orthogonal complement](../../../../../../orthogonal-complement.md)

$$
W=\eta^\perp\subset\Lambda^2 U
$$

has [dimension](../../../../../../dimension-vector-space.md) five and inherits a [nondegenerate bilinear form](../../../../../../nondegenerate-bilinear-form.md). It is the [primitive exterior square](../../../../../../primitive-exterior-square.md), equivalently the [kernel](../../../../../../kernel-of-a-linear-map.md) of the [symplectic contraction of an exterior square](../../../../../../symplectic-contraction-of-an-exterior-square.md).

The [symplectic Lie algebra](../../../../../../symplectic-lie-algebra.md) preserves $\eta$. It also preserves $\mathrm{vol}$, since its elements have [trace](../../../../../../matrix-trace.md) zero and the induced action on $\Lambda^4U$ is multiplication by that [trace](../../../../../../matrix-trace.md). The [exterior-power Lie algebra representation](../../../../../../exterior-power-lie-algebra-representation.md) therefore preserves $B$ and $W$, giving a [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md)

$$
\Phi:\mathfrak{sp}_4\longrightarrow\mathfrak{so}(W,B).
$$

To show injectivity, suppose $A$ acts as zero on $W$. It already acts as zero on the invariant line $\mathbb C\eta$, so it kills all of $\Lambda^2U=W\oplus\mathbb C\eta$. For any [basis](../../../../../../basis.md) $u_1,\ldots,u_4$, this means

$$
Au_i\wedge u_j+u_i\wedge Au_j=0\qquad(i\ne j).
$$

If $k\ne i$, choose $j$ distinct from $i,k$; the coefficient of $u_k\wedge u_j$ forces $A_{ki}=0$. Thus $A$ is diagonal. The same identity gives $A_{ii}+A_{jj}=0$ for every pair. Applying this to three distinct indices forces each diagonal entry to vanish. Hence $A=0$ and $\Phi$ is injective.

Finally $\dim\mathfrak{sp}_4=2(2\cdot2+1)=10$ and $\dim\mathfrak{so}(W,B)=5\cdot4/2=10$. Injectivity between these equal-dimensional [vector spaces](../../../../../../vector-space-split.md) gives surjectivity. Every [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) complex [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) on a five-dimensional space is equivalent to the standard one. We have therefore constructed the [exceptional isomorphism between sp4 and so5](../../../../../../exceptional-isomorphism-between-sp4-and-so5.md):

$$
\boxed{\mathfrak{sp}_4\cong\mathfrak{so}_5.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
