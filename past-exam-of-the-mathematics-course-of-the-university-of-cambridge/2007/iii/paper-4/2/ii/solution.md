<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We construct the [exceptional isomorphism between sp4 and so5](../../../../../../exceptional-isomorphism-between-sp4-and-so5.md). Let $W=\mathbb C^4$ have a [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) alternating form $\Omega$ and [symplectic basis](../../../../../../symplectic-basis.md) $a_1,b_1,a_2,b_2$. Define the [symplectic contraction of an exterior square](../../../../../../symplectic-contraction-of-an-exterior-square.md)

$$
\kappa:\Lambda^2W\to\mathbb C,\qquad\kappa(u\wedge v)=\Omega(u,v),
\qquad E=\ker\kappa.
$$

It is equivariant for the [symplectic Lie algebra](../../../../../../symplectic-lie-algebra.md), and $\dim E=5$. Identify $\Lambda^4W$ with $\mathbb C$ using $a_1\wedge b_1\wedge a_2\wedge b_2$. Wedge product then gives a symmetric [bilinear form](../../../../../../bilinear-form.md) $B(\xi,\eta)=\xi\wedge\eta$ on $\Lambda^2W$. It is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md), as the wedge-basis vectors pair with their complementary pairs.

The bivector $\tau=a_1\wedge b_1+a_2\wedge b_2$ is invariant under $\mathfrak{sp}(W)$, satisfies $B(\tau,\tau)=2$, and has $B(\xi,\tau)=\kappa(\xi)$. Consequently $E=\tau^\perp$ and $B|_E$ is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md). The [exterior-power Lie algebra representation](../../../../../../exterior-power-lie-algebra-representation.md) preserves wedge product and the volume form, so restriction gives a homomorphism

$$
\Phi:\mathfrak{sp}_4\longrightarrow\mathfrak{so}(E,B).
$$

We check injectivity directly. If $X$ acts trivially on $E$, it also annihilates the invariant line $\mathbb C\tau$, hence acts trivially on all of $\Lambda^2W$. In any basis $w_1,\ldots,w_4$, the equation $X(w_i\wedge w_j)=0$ forces every off-diagonal coefficient $X_{ki}$ to vanish: choose $j$ distinct from $i,k$ and inspect the coefficient of $w_k\wedge w_j$. Thus $X$ is diagonal. Its diagonal entries $x_i$ satisfy $x_i+x_j=0$ for every pair, which forces them all to be zero. Therefore $\Phi$ is injective.

A symplectic matrix has infinitesimal block form $\left(\begin{smallmatrix}A&B\\C&-A^T\end{smallmatrix}\right)$ with $B,C$ symmetric, so $\dim\mathfrak{sp}_4=4+3+3=10$. Also $\dim\mathfrak{so}(E,B)=5\cdot4/2=10$. Injectivity and equal [dimensions](../../../../../../dimension-vector-space.md) make $\Phi$ an isomorphism. Every [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) complex symmetric form in [dimension](../../../../../../dimension-vector-space.md) five is equivalent by a change of basis to the given antidiagonal form, so

$$
\boxed{\mathfrak{so}_5\cong\mathfrak{sp}_4.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
