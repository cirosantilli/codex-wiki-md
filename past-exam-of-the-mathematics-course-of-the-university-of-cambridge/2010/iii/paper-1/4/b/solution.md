<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V=\mathbb C^4$ with its [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) [alternating bilinear form](../../../../../../alternating-bilinear-form.md). Its inverse-form bivector $\Omega\in\Lambda^2V$ is invariant under the [symplectic Lie algebra](../../../../../../symplectic-lie-algebra.md), and $\Omega\wedge\Omega\ne0$. Choose $\operatorname{vol}=\Omega\wedge\Omega/2$. The [exterior product](../../../../../../exterior-product.md) defines a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) on $\Lambda^2V$ by

$$
\xi\wedge\eta=B(\xi,\eta)\operatorname{vol}.
$$

It is symmetric because two-forms commute under the wedge product. It is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) because each basis wedge $e_i\wedge e_j$ pairs with its complementary basis wedge. Since $B(\Omega,\Omega)=2$, the five-dimensional [orthogonal complement](../../../../../../orthogonal-complement.md)

$$
W=\Omega^\perp=\Lambda_0^2V
$$

also has a [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md). This is the [primitive exterior square](../../../../../../primitive-exterior-square.md), equivalently the [kernel](../../../../../../kernel-of-a-linear-map.md) of [symplectic contraction of an exterior square](../../../../../../symplectic-contraction-of-an-exterior-square.md).

Every element of $\mathfrak{sp}_4$ fixes $\Omega$ and preserves volume, since its [trace](../../../../../../matrix-trace.md) is zero. The induced [exterior-power Lie algebra representation](../../../../../../exterior-power-lie-algebra-representation.md) consequently preserves $W$ and satisfies $B(A\xi,\eta)+B(\xi,A\eta)=0$. Thus it gives a [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md)

$$
\varphi:\mathfrak{sp}_4\longrightarrow\mathfrak{so}(W,B).
$$

We check [injectivity](../../../../../../injective-function.md) explicitly. If $A$ acts as zero on $W$, it also kills $\Omega$, and therefore acts as zero on all of $\Lambda^2V=W\oplus\mathbb C\Omega$. For three distinct indices $i,j,k$, the coefficient of $e_k\wedge e_j$ in $A(e_i\wedge e_j)$ is $A_{ki}$, so all off-diagonal entries of $A$ vanish. Its action on $e_i\wedge e_j$ is then $(A_{ii}+A_{jj})e_i\wedge e_j$. All these sums vanish, which in characteristic zero forces every diagonal entry to vanish. Hence $A=0$.

Finally,

$$
\dim\mathfrak{sp}_4=4+3+3=10=\frac{5\cdot4}{2}=\dim\mathfrak{so}(W,B).
$$

The injective [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md) is therefore surjective. Over $\mathbb C$, every [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) admits a basis in which its matrix is the identity, so this constructs the [exceptional isomorphism between sp4 and so5](../../../../../../exceptional-isomorphism-between-sp4-and-so5.md):

$$
\boxed{\mathfrak{sp}_4(\mathbb C)\cong\mathfrak{so}_5(\mathbb C).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
